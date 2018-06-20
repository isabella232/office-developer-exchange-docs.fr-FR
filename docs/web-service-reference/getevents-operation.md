---
title: Opération GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: f268efe5-9a1a-41a2-b6a6-51fcde7720a1
description: L’opération GetEvents est utilisée par les clients d’abonnement extrait pour demander des notifications à partir du serveur d’accès au Client. La réponse d’opération GetEvents renvoie un tableau d’éléments et les événements qui se sont produites dans une boîte aux lettres depuis le dernier la notification.
ms.openlocfilehash: 1a23a9d570a4554e54becb7927f25dff89888c74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756589"
---
# <a name="getevents-operation"></a>Opération GetEvents

L’opération **GetEvents** est utilisée par les clients d’abonnement extrait pour demander des notifications à partir du serveur d’accès au Client. La réponse d’opération **GetEvents** renvoie un tableau d’éléments et les événements qui se sont produites dans une boîte aux lettres depuis le dernier la notification. 
  
> [!IMPORTANT]
> L’opération **DeleteUserConfiguration** déclenche un événement de déplacement pour le système de notification d’événement. L’objet de configuration utilisateur est déplacée vers la benne. 
  
## <a name="remarks"></a>Remarques

Modifications apportées aux éléments de calendrier peuvent entraîner la génération de plusieurs événements. Ces événements sont le résultat d’éléments temporaires en cours de création dans la boîte aux lettres, les éléments de stockage et de disponibilité des données en cours de modification dans le cadre des opérations de calendrier normales, ou les deux. Événements d’élément de classe « IPM. SchedulePlus.FreeBusy.BinaryData » doit être ignorée par les clients de service Web. Ces éléments temporaires sont supprimés après leur création ; Par conséquent, si une tentative est effectuée pour récupérer ces éléments, une erreur sera renvoyée qui indique que l’élément est introuvable.
  
## <a name="getevents-request-example"></a>Exemple de requête GetEvents

### <a name="description"></a>Description

L’exemple suivant montre comment demander les événements et les éléments qui sont associés à un abonnement est identifié par l’identificateur d’abonnement et filigrane.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a>Éléments de demandes GetEvents

Les éléments suivants sont utilisés dans la demande :
  
- [GetEvents](getevents.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Filigrane](watermark.md)
    
## <a name="successful-getevents-response-example"></a>Exemple de réponse GetEvents réussie

### <a name="description"></a>Description

Une réponse de l’exemple suivant montre une notification de l’existence de deux nouveaux messages électroniques depuis la dernière demande de notification a été envoyée au serveur.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:PreviousWatermark>AAAAAMAGAAAAAAAAAQ==</t:PreviousWatermark>
            <t:MoreEvents>false</t:MoreEvents>
            <t:NewMailEvent>
              <t:Watermark>AAAAAM4GAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T00:36:29Z</t:TimeStamp>
              <t:ItemId Id="AQApAHR" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:NewMailEvent>
              <t:Watermark>AAAAAOQGAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T01:00:50Z</t:TimeStamp>
              <t:ItemId Id="AQApAHRw" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
          </m:Notification>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

> [!NOTE]
> Les identificateurs d’éléments et dossiers ont été réduits afin de préserver la lisibilité. 
  
### <a name="getevents-response-elements"></a>Éléments de réponse GetEvents

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetEventsResponse](geteventsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetEventsResponseMessage](geteventsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Notification](notification-ex15websvcsotherref.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [PreviousWatermark](previouswatermark.md)
    
- [MoreEvents](moreevents.md)
    
- [NewMailEvent](newmailevent.md)
    
- [Filigrane](watermark.md)
    
- [Horodatage](timestamp.md)
    
- [ID d’élément](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
Pour trouver d’autres options pour le message de réponse de l’opération **GetEvents** , explorez la hiérarchie de schéma. Démarrez au niveau de l’élément de [Notification](notification-ex15websvcsotherref.md) . 
  
## <a name="getevents-error-response-example"></a>Exemple de réponse d’erreur GetEvents

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande **GetEvents** . 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Error">
          <m:MessageText>Access is denied. Only the subscription owner may access the subscription.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionAccessDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a>Remarques

Lors du traitement d’une demande **GetEvents** , le serveur d’accès au Client effectue les étapes suivantes : 
  
1. L’ID d’abonnement de la demande est confirmé comme étant un abonnement valide qui est hébergé sur le serveur d’accès au Client. S’il n’est pas le cas, l’appel **GetEvents** échoue. 
    
2. L’adresse SMTP de l’utilisateur authentifié pour la demande est comparé à l’adresse SMTP de l’utilisateur qui a créé l’abonnement. Si elles ne correspondent pas, la demande **GetEvents** échoue. 
    
3. La file d’attente de l’abonnement est interrogé pour les événements qui sont en attente d’être envoyées au client. Si la file d’attente n’est pas vide, les 50 premiers événements à partir de la file d’attente sont extraites de la file d’attente et codés dans une notification.
    
4. Si aucun événement n’est détectée dans la file d’attente, un StatusEvent est généré et codé en réponse à une notification.
    
5. La réponse de notification est retournée au client.
    
6. Les événements qui sont inclus dans la notification sont supprimés de la file d’attente de l’abonnement et le Client Access server local dernière filigrane pour l’abonnement est défini sur la limite du dernier événement qui est renvoyé.
    
7. Le délai d’expiration de l’abonnement est réinitialisé.
    
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)


[À l’aide d’abonnement](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

