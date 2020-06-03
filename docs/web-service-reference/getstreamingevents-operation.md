---
title: Opération de GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: 8da95423-72bc-4034-90a8-162eedcd059b
description: Trouvez des informations sur l’opération EWS GetStreamingEvents.
ms.openlocfilehash: 27744ec40d7c7cb551f35ed5f6fcb726f23d4865
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530168"
---
# <a name="getstreamingevents-operation"></a>Opération de GetStreamingEvents

Trouvez des informations sur l’opération EWS **GetStreamingEvents** . 
  
L’opération **GetStreamingEvents** est utilisée par les clients d’abonnements de diffusion en continu pour demander des notifications à partir du serveur d’accès au client. La réponse **GetStreamingEvents** renvoie un tableau d’éléments et d’événements qui se sont produits dans une boîte aux lettres depuis la dernière notification. 
  
## <a name="getstreamingevents-request-example"></a>Exemple de requête GetStreamingEvents

### <a name="description"></a>Description

L’exemple suivant d’une opération **GetStreamingEvents** indique comment demander les événements et les éléments qui sont associés à un abonnement identifié par l’identificateur d’abonnement. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
  xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Body>
    <GetStreamingEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <ConnectionTimeout>30</ConnectionTimeout>
    </GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getstreamingevents-request-elements"></a>Éléments de requête GetStreamingEvents

Les éléments suivants sont utilisés dans la demande :
  
- [GetStreamingEvents](getstreamingevents.md)
    
- [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md)
    
- [ConnectionTimeout](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a>Exemple de réponse GetStreamingEvents réussi

### <a name="description"></a>Description

L’exemple suivant de réponse **GetStreamingEvents** indique les notifications envoyées au client lors de la réception d’un nouveau message électronique. Elle inclut des notifications pour les événements suivants : CreatedEvent, NewMail et ModifiedEvent. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Header xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <ServerVersionInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
</soap:Header>
<soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseMessages>
      <m:GetStreamingEventsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Notifications>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:CreatedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:CreatedEvent>
            <t:NewMailEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:ModifiedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:FolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgEJAAAA" ChangeKey="AQAAAA==" />
              <t:UnreadCount>1</t:UnreadCount>
            </t:ModifiedEvent>
          </m:Notification>
        </m:Notifications>
      </m:GetStreamingEventsResponseMessage>
    </m:ResponseMessages>
  </m:GetStreamingEventsResponse>
</soap:Body>
```

### <a name="getstreamingevents-response-elements"></a>Éléments Response GetStreamingEvents

Les éléments suivants sont utilisés dans la réponse :
  
- [GetStreamingEventsResponse](getstreamingeventsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md)
    
- [NotesFolderPermissionLevel](notesfolderpermissionlevel.md)
    
- [Notification](notification-ex15websvcsotherref.md)
    
- [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md)
    
Pour trouver d’autres options pour le message de réponse de l’opération **GetStreamingEvents** , explorez la hiérarchie du schéma. Commencez par l’élément [notification](notification-ex15websvcsotherref.md) . 
  
## <a name="getstreamingevents-error-response-example"></a>Exemple de réponse d’erreur GetStreamingEvents

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une requête **GetStreamingEvents** . 
  
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
    <GetStreamingEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetStreamingEventsResponseMessage ResponseClass="Error">
        <m:MessageText></m:MessageText>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        <m:ResponseCode>ErrorInvalidSubscription</m:ResponseCode>
        <m:ConnectionStatus>Closed</m:ConnectionStatus>
      </m:ResponseMessages>
    </GetStreamingEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a>Remarques

Lors du traitement d’une demande **GetStreamingEvents** , le serveur d’accès au client effectue les étapes suivantes : 
  
1. Le [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) de la demande est confirmé comme étant un abonnement valide hébergé sur le serveur d’accès au client. Si ce n’est pas le cas, l’appel **GetStreamingEvents** échoue. 
    
2. L’adresse SMTP de l’utilisateur authentifié pour la demande est validée pour disposer des droits d’emprunt d’identité. Si ce n’est pas le cas, la demande **GetStreamingEvents** échoue. 
    
3. La file d’attente d’abonnement est interrogée pour les événements qui attendent d’être envoyés au client. Si la file d’attente n’est pas vide, les premiers événements 50 de la file d’attente sont extraits de la file d’attente et codés dans une notification.
    
4. Si aucun événement n’est trouvé dans la file d’attente, une [StatusEvent](statusevent.md) est générée et codée dans une réponse de notification. 
    
5. La réponse de notification est renvoyée au client.
    
6. Les événements inclus dans la notification sont supprimés de la file d’attente d’abonnement et le dernier filigrane local du serveur d’accès au client pour l’abonnement est défini sur le filigrane du dernier événement renvoyé.
    
7. Le délai d’expiration de l’abonnement est réinitialisé.
    
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

