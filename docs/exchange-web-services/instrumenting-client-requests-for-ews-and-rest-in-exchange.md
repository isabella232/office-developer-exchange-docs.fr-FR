---
title: L’instrumentation les demandes des clients pour EWS et reste dans Exchange
manager: sethgros
ms.date: 4/13/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 330de503-498d-447e-b4a9-c20fc1699fd1
description: En savoir plus sur les en-têtes HTTP dans les services EWS et des requêtes REST et les réponses qui peuvent vous aider à surveiller et dépanner votre application Exchange.
ms.openlocfilehash: bcf362952c29956729c44397043a56bf3603d0af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754968"
---
# <a name="instrumenting-client-requests-for-ews-and-rest-in-exchange"></a>L’instrumentation les demandes des clients pour EWS et reste dans Exchange

En savoir plus sur les en-têtes HTTP dans les services EWS et des requêtes REST et les réponses qui peuvent vous aider à surveiller et dépanner votre application Exchange.
  
Cela jamais arrivé à vous ? Un utilisateur de votre application indique une erreur inattendue. Vous souhaitez examiner, mais vous ne pouvez pas le reproduire. L’erreur a disparu de l’utilisateur, et il reste très peu de données pertinentes. Frustrant, non ? Voyons comment vous pouvez anticiper ce scénario et espère éviter frustration à l’avenir.
  
## <a name="add-instrumentation-to-requests"></a>Ajouter l’instrumentation aux demandes

Nous vous recommandons d’ajouter des en-têtes HTTP supplémentaires à vos demandes afin de faciliter la résolution des problèmes. Vous devez garder une trace de ces informations en cours (par exemple, dans un fichier journal) afin que vous pouvez le récupérer ultérieurement si vous avez besoin. Cela est utile lors de l’examen du trafic réseau et est également utile si vous contactez le support technique Microsoft pour obtenir une assistance.
  
**Le tableau 1. En-têtes de requête pour la résolution des problèmes**

|**En-tête HTTP (EWS)**|**Équivalent de l’API managée EWS**|**Remarques**|
|:-----|:-----|:-----|
|Agent utilisateur  <br/> |[ExchangeService.UserAgent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.useragent%28v=exchg.80%29.aspx) <br/> |Définir une valeur unique qui identifie l’application cliente.<br/><br/> À l’aide de la même valeur pour toutes les demandes de votre application envoie permet à Microsoft de résoudre les échecs des appels, ils surviendrait.  <br/> |
|id de demande client  <br/> |[ExchangeService.ClientRequestId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.clientrequestid%28v=exchg.80%29.aspx) <br/> |Définir une autre valeur unique pour chaque demande de que votre application envoie.<br/><br/> Nous recommandons d’utiliser un GUID. Cet identificateur unique est destiné à être utilisé pour mettre en corrélation les activités entre deux systèmes dans le cas où quelque chose ne fonctionnerait pas.  <br/> |
|retour-client--id de demande  <br/> |[ExchangeService.ReturnClientRequestId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.returnclientrequestid%28v=exchg.80%29.aspx) <br/> |Définir sur **true** pour signaler sur le serveur Exchange qu’elle doit retourner la valeur de votre id de demande de client dans la réponse correspondante.<br/><br/> Vous pouvez utiliser ce pour faire correspondre les demandes et réponses dans les suivis réseau ou des traces de l’API managée EWS.  <br/> |
|X-ClientStatistics  <br/> |[ExchangeService.SendClientLatencies](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) <br/> |Utilisé pour [les latences EWS rapport](#bk_ReportLatency) à Microsoft si votre application accède à Exchange Online ou Exchange Online dans le cadre d’Office 365.  <br/> |
   
## <a name="log-information-from-responses"></a>Informations du journal des réponses

Comme votre client peut ajouter instrumentation supplémentaires pour les demandes, qu'il envoie, Exchange ajoute instrumentation supplémentaires pour les réponses sous la forme d’en-têtes HTTP. Votre client doit capturer ces informations pour accéder ainsi que les informations d’instrumentation de demande.
  
> [!NOTE]
> Si vous utilisez l’API managée EWS, il n’existe aucun équivalent direct pour les en-têtes HTTP. Toutefois, tous les en-têtes de réponse HTTP est accessible via la propriété [ExchangeService.HttpResponseHeaders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.httpresponseheaders%28v=exchg.80%29.aspx) . 
  
**Le tableau 2. En-têtes de réponse HTTP**

|**En-tête HTTP**|**Description**|
|:-----|:-----|
|id de la demande  <br/> |Un ID généré par le serveur pour la demande qui correspond à cette réponse.  <br/> |
|id de demande client  <br/> |La valeur de l’en-tête de l’id de demande de client dans la demande.<br/><br/> Cet en-tête est présent uniquement si la requête contient l’en-tête de retour-client-demande-id avec la valeur **true**.  <br/> |
|X-FEServer  <br/> |Le nom de domaine complet du serveur d’accès Client qui ont traité la demande.  <br/> |
|X-TargetBEServer  <br/> |Le nom de domaine complet du serveur de boîtes aux lettres qui ont traité la demande.  <br/> |
|X-DiagInfo  <br/> |Informations de diagnostic supplémentaires, en fonction de la demande.  <br/> |
|x-ms-diagnostics  <br/> | Cet en-tête s’applique uniquement si l’authentification OAuth est utilisée dans la demande.<br/><br/> Il contient un code d’erreur explicites qui spécifie la raison de l’échec d’authentification OAuth.<br/><br/> Elle prend le format suivant :`errorId;reason="reason"error_type="error type"`<br/><br/> Le champ **raison** est une description explicite de l’erreur.<br/><br/> Le champ **code d’erreur** est un entier et le **erreur\_type** champ est la représentation sous forme de chaîne de cet entier, comme suit :<ul><li>2000000 : non valide\_signature</li><li>2000001 : non valide\_jeton</li><li>  2000002 : jeton\_a expiré</li><li>2000003 : non valide\_ressource</li><li>2000004 : non valide\_client  </li><li>2000005 : non valide\_utilisateur</li><li>2000006 : non valide\_client</li><li>2000007 : interne\_erreur</li><li>2000008 : non valide\_accorder</li></ul> |
   
## <a name="report-ews-latency-to-microsoft"></a>Latence EWS rapport à Microsoft
<a name="bk_ReportLatency"> </a>

Si votre application utilise les API managées EWS pour se connecter à Exchange Online, vous pouvez signaler la latence des demandes EWS directement à Microsoft. Les informations sont transmises par le biais de l’en-tête de demande X-ClientStatistics. Si vous utilisez l’API managée EWS, il vous est définie à la propriété [ExchangeService.SendClientLatencies](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) sur **true**. Si vous utilisez EWS, vous devez mesurer le délai entre l’émission d’une demande et recevoir une réponse, puis ajoutez l’en-tête X-ClientStatistics à la prochaine demande EWS votre application envoie, en utilisant le format suivant.
  
`X-ClientStatistics: MessageId=<value of request-id header>,ResponseTime=<time in milliseconds>,SoapAction=<EWS operation>`
  
Nous tenir à jour des rapports pour ces latences et les utiliser pour améliorer en continu les services EWS dans Exchange Online.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_ReportLatency"> </a>

Après avoir ajouté instrumentation client à votre application, vous êtes mieux si quelque chose ne fonctionnerait pas. Dans ce cas, vous pouvez utiliser vos données WMI pour [résoudre les problèmes de votre application](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md).
  
## <a name="see-also"></a>Voir aussi

- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
- [Suivi des demandes et réponses pour dépanner les applications de l’API managée EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
- [Outils et ressources pour la résolution des applications EWS pour Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

