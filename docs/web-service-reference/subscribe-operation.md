---
title: Opération d’abonnement
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Subscribe
api_type:
- schema
ms.assetid: f17c3d08-c79e-41f1-ba31-6e41e7aafd87
description: L’opération d’abonnement est utilisée pour abonner des applications clientes aux notifications Push ou Pull. Il est important de savoir que la structure des messages et réponses de la demande est différente en fonction du type de notification d’événement.
ms.openlocfilehash: 546f7ab252c7d3a201130cd48e2b30ca52d00088
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544534"
---
# <a name="subscribe-operation"></a>Opération d’abonnement

L’opération d’abonnement est utilisée pour abonner des applications clientes aux notifications Push ou Pull. Il est important de savoir que la structure des messages et réponses de la demande est différente en fonction du type de notification d’événement. 
  
## <a name="pull-subscription-subscribe-request-example"></a>Exemple de requête Pull Subscription Subscribe

### <a name="description"></a>Description

L’exemple de code suivant montre comment s’abonner à un abonnement de notification d’événement pull. L’abonnement informe l’application cliente si de nouveaux messages sont ajoutés à la boîte de réception et si un élément est supprimé de la boîte de réception. L’abonnement prend fin si le client ne demande pas d’informations sur les événements dans un délai de dix minutes. Si l’abonnement expire, un nouvel abonnement doit être établi pour continuer à demander des notifications.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <PullSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox"/>
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
          <t:EventType>DeletedEvent</t:EventType>
        </t:EventTypes>
        <t:Timeout>10</t:Timeout>
      </PullSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-request-elements"></a>Éléments de demande d’abonnement pull

Les éléments suivants sont utilisés dans la demande :
  
- [Subscribe](subscribe.md)
    
- [PullSubscriptionRequest](pullsubscriptionrequest.md)
    
- [FolderIds](folderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [EventTypes](eventtypes.md)
    
- [EventType](eventtype.md)
    
- [Timeout](timeout.md)
    
Pour rechercher d’autres options pour le message de demande de l’opération Subscribe, explorez la hiérarchie de schéma. Commencez par [l’élément PullSubscriptionRequest.](pullsubscriptionrequest.md) 
  
## <a name="successful-pull-subscription-subscribe-response-example"></a>Exemple de réponse Pull Subscription Subscribe réussie

### <a name="description"></a>Description

L’exemple suivant illustre une réponse d’abonnement pull réussie. La réponse contient l’identificateur d’abonnement et le filigrane utilisés pour obtenir le tableau des événements associés à un abonnement. L’identificateur d’abonnement est également utilisé pour désabonner un client d’un abonnement.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>39ea5d0f-f062-455e-a1e9-89c0304390f4</m:SubscriptionId>
          <m:Watermark>AAAAAHgGAAAAAAAAAQ==</m:Watermark>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-response-elements"></a>Éléments de réponse Pull Subscription Subscribe

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SubscribeResponse](subscriberesponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SubscribeResponseMessage](subscriberesponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Watermark](watermark.md)
    
## <a name="pull-subscription-subscribe-error-response-example"></a>Exemple de réponse d’erreur d’abonnement Pull Subscription

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande d’abonnement. L’erreur est due à une tentative d’abonnement aux notifications à l’aide de l’accès délégué.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>Subscriptions are not supported for delegate user access.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionDelegateAccessNotSupported</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-error-response-elements"></a>Éléments de réponse d’erreur d’abonnement pull

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SubscribeResponse](subscriberesponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SubscribeResponseMessage](subscriberesponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="push-subscription-request-example"></a>Exemple de demande d’abonnement Push

### <a name="description"></a>Description

L’exemple de code suivant montre comment s’abonner à un abonnement à une notification d’événement Push. La demande identifie les dossiers à surveiller, les types d’événements à surveiller, la fréquence des notifications d’état et l’URL du service Web client qui écoute les notifications Push.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <PushSubscriptionRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <FolderIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <DistinguishedFolderId Id="inbox" />
        </FolderIds>
        <EventTypes xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EventType>NewMailEvent</EventType>
          <EventType>CopiedEvent</EventType>
          <EventType>CreatedEvent</EventType>
          <EventType>DeletedEvent</EventType>
          <EventType>ModifiedEvent</EventType>
          <EventType>MovedEvent</EventType>
        </EventTypes>
        <StatusFrequency xmlns="https://schemas.microsoft.com/exchange/services/2006/types">1</StatusFrequency>
        <URL xmlns="https://schemas.microsoft.com/exchange/services/2006/types">http://clientWebService/Service.asmx</URL>
      </PushSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Le service Web client doit être installé avant l’envoi de la demande d’abonnement aux notifications Push . Sinon, la première notification ne sera pas envoyée à un point de terminaison valide et la notification Push échouera. Pour plus d’informations, voir [l’exemple d’application de notification Push.](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)
  
Un nouvel [SubscriptionId (GetEvents)](subscriptionid-getevents.md) est créé lorsque vous vous réabonner. Utilisez le filigrane d’un abonnement précédent pour vous réabonner au point où l’abonnement précédent a pris fin. 
  
### <a name="push-subscription-request-elements"></a>Éléments de demande d’abonnement Push

Les éléments suivants sont utilisés dans la demande :
  
- [Subscribe](subscribe.md)
    
- [PushSubscriptionRequest](pushsubscriptionrequest.md)
    
- [FolderIds](folderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [EventTypes](eventtypes.md)
    
- [EventType](eventtype.md)
    
- [StatusFrequency](statusfrequency.md)
    
- [URL ](url-ex15websvcsotherref.md)
    
## <a name="successful-push-subscription-response-example"></a>Exemple de réponse d’abonnement Push réussie

### <a name="description"></a>Description

L’exemple suivant illustre une réponse d’abonnement Push réussie. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <SubscribeResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <SubscriptionId>83826921-afdf-48be-b469-628cc02b5f49</SubscriptionId>
          <Watermark>AQAAAOpvG0LURVdOhQkPOWZLPcI8EgAAAAAAAAE=</Watermark>
        </SubscribeResponseMessage>
      </ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="push-subscription-response-elements"></a>Éléments de réponse d’abonnement Push

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SubscribeResponse](subscriberesponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SubscribeResponseMessage](subscriberesponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Watermark](watermark.md)
    
## <a name="see-also"></a>Voir aussi



[Opération de résiliation d'abonnement](unsubscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)


[Utilisation des abonnements Pull](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[Exemple d'application de notification Push](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

