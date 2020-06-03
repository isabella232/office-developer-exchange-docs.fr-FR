---
title: Instrumentation des demandes de client pour EWS et REST dans Exchange
manager: sethgros
ms.date: 4/13/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 330de503-498d-447e-b4a9-c20fc1699fd1
description: Découvrez les en-têtes HTTP dans EWS et les requêtes REST et les réponses qui peuvent vous aider à surveiller et à dépanner votre application Exchange.
ms.openlocfilehash: 3a8ce889ec7a6b9e70ec25a95ac248902f48ca6c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456303"
---
# <a name="instrumenting-client-requests-for-ews-and-rest-in-exchange"></a>Instrumentation des demandes de client pour EWS et REST dans Exchange

Découvrez les en-têtes HTTP dans EWS et les requêtes REST et les réponses qui peuvent vous aider à surveiller et à dépanner votre application Exchange.
  
Vous êtes-vous déjà passé ? Un utilisateur de votre application signale une erreur inattendue. Vous souhaitez examiner, mais vous ne pouvez pas le reproduire. L’erreur a disparu pour l’utilisateur et vous n’avez pas de données exploitables. Frustrant, n’est-ce pas ? Examinons comment vous pouvez vous préparer de manière proactive à ce scénario et éviter ainsi toute frustration à l’avenir.
  
## <a name="add-instrumentation-to-requests"></a>Ajouter l’instrumentation aux requêtes

Nous vous recommandons d’ajouter des en-têtes HTTP supplémentaires à vos demandes pour faciliter la résolution des problèmes. Vous devez conserver un enregistrement de ces informations quelque part (par exemple, dans un fichier journal) afin de pouvoir les récupérer plus tard si vous le souhaitez. Cela est utile lors de l’examen du trafic réseau et est également utile si vous contactez le support Microsoft pour obtenir de l’aide.
  
**Tableau 1. En-têtes de demande pour la résolution des problèmes**

|**En-tête HTTP (EWS)**|**Équivalent de l’API managée EWS**|**Remarques**|
|:-----|:-----|:-----|
|Agent utilisateur  <br/> |[ExchangeService. UserAgent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.useragent%28v=exchg.80%29.aspx) <br/> |Définissez cette valeur sur une valeur unique qui identifie votre application cliente.<br/><br/> L’utilisation de la même valeur pour toutes les demandes envoyées par votre application permet à Microsoft d’aider à résoudre les problèmes d’appel, le cas échéant.  <br/> |
|client-Request-ID  <br/> |[ExchangeService. ClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.clientrequestid%28v=exchg.80%29.aspx) <br/> |Affectez une valeur unique différente à chaque demande envoyée à votre application.<br/><br/> Nous vous recommandons d’utiliser un GUID. Cet identificateur unique est destiné à être utilisé pour corréler les activités entre deux systèmes en cas de problème.  <br/> |
|Return-client-Request-ID  <br/> |[ExchangeService. ReturnClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.returnclientrequestid%28v=exchg.80%29.aspx) <br/> |Affectez à cet argument la valeur **true** pour signaler au serveur Exchange qu’il doit retourner la valeur de votre client-Request-ID dans la réponse correspondante.<br/><br/> Vous pouvez l’utiliser pour corréler les demandes et les réponses dans les traces réseau ou les traces de l’API managée EWS.  <br/> |
|X-ClientStatistics  <br/> |[ExchangeService. SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) <br/> |Utilisé pour [signaler les latences EWS](#bk_ReportLatency) à Microsoft si votre application accède à Exchange Online ou Exchange Online dans le cadre d’Office 365.  <br/> |
   
## <a name="log-information-from-responses"></a>Enregistrer les informations des réponses

Tout comme votre client peut ajouter une instrumentation supplémentaire aux demandes qu’il envoie, Exchange ajoute des instruments supplémentaires aux réponses sous la forme d’en-têtes HTTP. Votre client doit capturer ces informations à l’aide des informations d’instrumentation de demande.
  
> [!NOTE]
> Si vous utilisez l’API managée EWS, il n’existe aucun équivalent direct pour les en-têtes HTTP. Toutefois, tous les en-têtes de réponse HTTP sont accessibles via la propriété [ExchangeService. HttpResponseHeaders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.httpresponseheaders%28v=exchg.80%29.aspx) . 
  
**Tableau 2. En-têtes de réponse HTTP**

|**En-tête HTTP**|**Description**|
|:-----|:-----|
|demande-ID  <br/> |ID généré par le serveur pour la demande correspondant à cette réponse.  <br/> |
|client-Request-ID  <br/> |Valeur de l’en-tête client-Request-ID dans la demande.<br/><br/> Cet en-tête est présent uniquement si la demande contient l’en-tête Return-client-Request-ID avec la valeur **true**.  <br/> |
|X-FEServer  <br/> |Nom de domaine complet (FQDN) du serveur d’accès au client qui a traité la demande.  <br/> |
|X-TargetBEServer  <br/> |Nom de domaine complet (FQDN) du serveur de boîtes aux lettres qui a traité la demande.  <br/> |
|X-DiagInfo  <br/> |Informations de diagnostic supplémentaires, en fonction de la demande.  <br/> |
|x-ms-Diagnostics  <br/> | Cet en-tête n’est applicable que si l’authentification OAuth est utilisée dans la demande.<br/><br/> Elle contient un code d’erreur explicite qui indique pourquoi une authentification OAuth a échoué.<br/><br/> Il prend le format suivant :`errorId;reason="reason"error_type="error type"`<br/><br/> Le champ **raison** est une description explicite de l’erreur.<br/><br/> Le champ **errorId** est un entier et le champ ** \_ type d’erreur** est la représentation sous forme de chaîne de cet entier, comme suit :<ul><li>2 millions : signature non valide \_</li><li>2000001 : jeton non valide \_</li><li>  2000002 : le jeton \_ a expiré</li><li>2000003 : ressource incorrecte \_</li><li>2000004 : locataire non valide \_  </li><li>2000005 : utilisateur non valide \_</li><li>2000006 : client non valide \_</li><li>2000007 : \_ erreur interne</li><li>2000008 : attribution non valide \_</li></ul> |
   
## <a name="report-ews-latency-to-microsoft"></a>Signalement de la latence EWS à Microsoft
<a name="bk_ReportLatency"> </a>

Si votre application utilise l’API managée EWS ou EWS pour se connecter à Exchange Online, vous pouvez signaler la latence dans les demandes EWS directement à Microsoft. Les informations sont transmises via l’en-tête de requête X-ClientStatistics. Si vous utilisez l’API managée EWS, tout ce que vous avez à faire est de définir la propriété [ExchangeService. SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) sur **true**. Si vous utilisez EWS, vous devez mesurer le temps entre l’émission d’une demande et la réception d’une réponse, puis l’ajout de l’en-tête X-ClientStatistics à la prochaine requête EWS envoyée par votre application, en utilisant le format suivant.
  
`X-ClientStatistics: MessageId=<value of request-id header>,ResponseTime=<time in milliseconds>,SoapAction=<EWS operation>`
  
Nous mettons à jour des rapports pour ces latences et les utilisent pour améliorer en permanence les services EWS dans Exchange Online.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_ReportLatency"> </a>

Une fois que vous avez ajouté l’instrumentation client à votre application, vous êtes mieux préparé en cas de problème. Dans ce cas, vous pouvez utiliser vos données d’instrumentation pour [résoudre les problèmes de votre application](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md).
  
## <a name="see-also"></a>Voir aussi

- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
- [Suivi des demandes et des réponses pour dépanner les applications API managées EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
- [Outils et ressources pour la résolution des applications EWS pour Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

