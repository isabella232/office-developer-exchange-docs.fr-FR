---
title: Instrumentation des demandes de client pour EWS et REST dans Exchange
manager: sethgros
ms.date: 4/13/2016
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 330de503-498d-447e-b4a9-c20fc1699fd1
description: Découvrez les en-têtes HTTP dans les requêtes et réponses EWS et REST qui peuvent vous aider à surveiller et résoudre les problèmes de votre application Exchange web.
ms.openlocfilehash: f32a164436a1f8ab06192e71a287f5092fe9a6c4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520989"
---
# <a name="instrumenting-client-requests-for-ews-and-rest-in-exchange"></a>Instrumentation des demandes de client pour EWS et REST dans Exchange

Découvrez les en-têtes HTTP dans les requêtes et réponses EWS et REST qui peuvent vous aider à surveiller et résoudre les problèmes de votre application Exchange web.
  
Cela vous est-il déjà arrivé ? Un utilisateur de votre application signale une erreur inattendue. Vous souhaitez examiner, mais vous ne pouvez pas le reproduire. L’erreur a disparu pour l’utilisateur et vous ne disposez que de très peu de données actionnables. Frustrant, n’est-ce pas ? Examinons comment vous pouvez préparer ce scénario de manière proactive et, espérons-le, éviter toute frustration à l’avenir.
  
## <a name="add-instrumentation-to-requests"></a>Ajouter de l’instrumentation aux demandes

Nous vous recommandons d’ajouter des en-têtes HTTP supplémentaires à vos demandes pour faciliter le dépannage. Vous devez conserver un enregistrement de ces informations quelque part (par exemple, dans un fichier journal) afin de pouvoir les récupérer ultérieurement si nécessaire. Cela est utile lors de l’examen du trafic réseau et est également utile si vous contactez le support Microsoft pour obtenir de l’aide.
  
**Tableau 1. Demander des en-têtes pour la résolution des problèmes**

|**En-tête HTTP (EWS)**|**Équivalent d’API gérée EWS**|**Remarques**|
|:-----|:-----|:-----|
|User-Agent  <br/> |[ExchangeService.UserAgent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.useragent%28v=exchg.80%29.aspx) <br/> |Définissez cette valeur sur une valeur unique qui identifie votre application cliente.<br/><br/> L’utilisation de la même valeur pour toutes les demandes que votre application envoie permet à Microsoft de résoudre les problèmes d’appel, s’ils surviennent.  <br/> |
|client-request-id  <br/> |[ExchangeService.ClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.clientrequestid%28v=exchg.80%29.aspx) <br/> |Définissez cette valeur sur une valeur unique différente pour chaque demande que votre application envoie.<br/><br/> Nous vous recommandons d’utiliser un GUID. Cet identificateur unique est destiné à être utilisé pour corréler les activités entre deux systèmes en cas de problème.  <br/> |
|return-client-request-id  <br/> |[ExchangeService.ReturnClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.returnclientrequestid%28v=exchg.80%29.aspx) <br/> |Définissez cette valeur sur **true** pour signaler au serveur Exchange qu’il doit renvoyer la valeur de votre client-request-id dans la réponse correspondante.<br/><br/> Vous pouvez l’utiliser pour corréler les demandes et les réponses dans les suivis réseau ou les suivis d’API gérées EWS.  <br/> |
|X-ClientStatistics  <br/> |[ExchangeService.SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) <br/> |Permet de [signaler des latencies EWS](#bk_ReportLatency) à Microsoft si votre application accède à Exchange Online ou Exchange Online dans le cadre de Office 365.  <br/> |
   
## <a name="log-information-from-responses"></a>Journal des informations à partir des réponses

Tout comme votre client peut ajouter une instrumentation supplémentaire aux demandes qu’il envoie, Exchange ajoute une instrumentation supplémentaire aux réponses sous la forme d’en-têtes HTTP. Votre client doit capturer ces informations pour aller de même que les informations d’instrumentation de la demande.
  
> [!NOTE]
> Si vous utilisez l’API gérée EWS, il n’existe pas d’équivalent direct pour les en-têtes HTTP. Toutefois, tous les en-têtes de réponse HTTP sont accessibles via la [propriété ExchangeService.HttpResponseHeaders.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.httpresponseheaders%28v=exchg.80%29.aspx) 
  
**Tableau 2. En-têtes de réponse HTTP**

|**En-tête HTTP**|**Description**|
|:-----|:-----|
|request-id  <br/> |ID généré par le serveur pour la demande qui correspond à cette réponse.  <br/> |
|client-request-id  <br/> |Valeur de l’en-tête client-request-id dans la demande.<br/><br/> Cet en-tête est uniquement présent si la requête contient l’en-tête return-client-request-id avec la valeur **true**.  <br/> |
|X-FEServer  <br/> |Nom deqdn du serveur d’accès au client qui a traitée la demande.  <br/> |
|X-TargetBEServer  <br/> |Nom deqdn du serveur de boîtes aux lettres qui a traitée la demande.  <br/> |
|X-DiagInfo  <br/> |Informations de diagnostic supplémentaires, en fonction de la demande.  <br/> |
|x-ms-diagnostics  <br/> | Cet en-tête n’est applicable que si l’authentification OAuth est utilisée dans la demande.<br/><br/> Il contient un code d’erreur explicite qui spécifie pourquoi une authentification OAuth a échoué.<br/><br/> Elle prend le format suivant : `errorId;reason="reason"error_type="error type"`<br/><br/> Le **champ raison** est une description lisible de l’erreur.<br/><br/> Le **champ errorId** est un nombre integer et le **champ \_ type** d’erreur est la représentation sous forme de chaîne de cet nombre, comme suit :<ul><li>2000000 : \_ signature non valide</li><li>2000001 : jeton \_ non valide</li><li>  2000002 : le jeton a \_ expiré</li><li>2000003 : ressource \_ non valide</li><li>2000004 : client \_ non valide  </li><li>2000005 : utilisateur \_ non valide</li><li>2000006 : \_ client non valide</li><li>2000007 : erreur \_ interne</li><li>2000008 : octroi \_ non valide</li></ul> |
   
## <a name="report-ews-latency-to-microsoft"></a>Signaler la latence EWS à Microsoft
<a name="bk_ReportLatency"> </a>

Si votre application utilise l’API gérée EWS ou EWS pour se connecter à Exchange Online, vous pouvez signaler la latence dans les demandes EWS directement à Microsoft. Les informations sont transmises via l’en-tête de requête X-ClientStatistics. Si vous utilisez l’API gérée EWS, il vous s agit de définir la propriété [ExchangeService.SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) sur **true**. Si vous utilisez EWS, vous devez mesurer le temps entre l’émission d’une demande et la réception d’une réponse, puis ajouter l’en-tête X-ClientStatistics à la demande EWS suivante que votre application envoie, en utilisant le format suivant.
  
`X-ClientStatistics: MessageId=<value of request-id header>,ResponseTime=<time in milliseconds>,SoapAction=<EWS operation>`
  
Nous tenez à jour des rapports pour ces latencies et les utilisons pour améliorer en permanence les services EWS dans Exchange Online.
  
## <a name="next-steps"></a>Étapes suivantes
<a name="bk_ReportLatency"> </a>

Une fois que vous avez ajouté l’instrumentation client à votre application, vous êtes mieux préparé en cas de problème. Si cela se produit, vous pouvez utiliser vos données d’instrumentation pour [résoudre les problèmes de votre application.](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
  
## <a name="see-also"></a>Voir aussi

- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
- [Suivi des demandes et des réponses pour dépanner les applications API managées EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
- [Outils et ressources pour la résolution des applications EWS pour Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

