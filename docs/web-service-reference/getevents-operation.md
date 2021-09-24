---
title: Opération GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetEvents
api_type:
- schema
ms.assetid: f268efe5-9a1a-41a2-b6a6-51fcde7720a1
description: L’opération GetEvents est utilisée par les clients d’abonnement pull pour demander des notifications au serveur d’accès au client. La réponse de l’opération GetEvents renvoie un tableau d’éléments et d’événements qui se sont produits dans une boîte aux lettres depuis la dernière notification.
ms.openlocfilehash: 72d99a654921794115d56d28327a39a21c9ea378
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511599"
---
# <a name="getevents-operation"></a>Opération GetEvents

**L’opération GetEvents est** utilisée par les clients d’abonnement pull pour demander des notifications au serveur d’accès au client. La **réponse de l’opération GetEvents** renvoie un tableau d’éléments et d’événements qui se sont produits dans une boîte aux lettres depuis la dernière notification. 
  
> [!IMPORTANT]
> **L’opération DeleteUserConfiguration** déclenche un événement de déplacement pour le système de notification d’événement. L’objet de configuration utilisateur sera déplacé vers la benne. 
  
## <a name="notes"></a>Remarques

Les modifications apportées aux éléments de calendrier peuvent entraîner la génération de plusieurs événements. Ces événements sont le résultat de la création d’éléments temporaires dans la boîte aux lettres, de la changement des éléments de stockage des données de libre/occupé dans le cadre des opérations normales du calendrier, ou des deux. Événements pour la classe d’élément « IPM. SchedulePlus.FreeBusy.BinaryData » doit être ignoré par les clients de service Web. Ces éléments temporaires sont supprimés après leur création . par conséquent, si une tentative de récupération de ces éléments est réalisée, une erreur est renvoyée qui indique que l’élément est in trouvé.
  
## <a name="getevents-request-example"></a>Exemple de requête GetEvents

### <a name="description"></a>Description

L’exemple suivant montre comment demander les événements et les éléments associés à un abonnement identifié par l’identificateur et le filigrane de l’abonnement.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a>Éléments de requête GetEvents

Les éléments suivants sont utilisés dans la demande :
  
- [GetEvents](getevents.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Watermark](watermark.md)
    
## <a name="successful-getevents-response-example"></a>Exemple de réponse GetEvents réussie

### <a name="description"></a>Description

L’exemple de réponse suivant montre une notification de l’existence de deux nouveaux messages électroniques depuis que la dernière demande de notification a été envoyée au serveur.
  
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
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
> Les identificateurs d’élément et de dossier ont été raccourcis pour préserver la lisibilité. 
  
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
    
- [Watermark](watermark.md)
    
- [TimeStamp](timestamp.md)
    
- [ItemId](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
Pour rechercher d’autres options pour le message de réponse de l’opération **GetEvents,** explorez la hiérarchie de schéma. Commencez à [l’élément Notification.](notification-ex15websvcsotherref.md) 
  
## <a name="getevents-error-response-example"></a>Exemple de réponse d’erreur GetEvents

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à **une demande GetEvents.** 
  
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
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Lors du traitement **d’une demande GetEvents,** le serveur d’accès au client effectue les étapes suivantes : 
  
1. L’subscriptionID de la demande est confirmé comme un abonnement valide hébergé sur le serveur d’accès au client. Si ce n’est pas le cas, **l’appel GetEvents** échoue. 
    
2. L’adresse SMTP de l’utilisateur authentifié pour la demande est comparée à l’adresse SMTP de l’utilisateur qui a créé l’abonnement. Si elles ne correspondent pas, la **demande GetEvents** échoue. 
    
3. La file d’attente des abonnements est interrogé pour les événements en attente d’envoi au client. Si la file d’attente n’est pas vide, les 50 premiers événements de la file d’attente sont retirés de la file d’attente et codés dans une notification.
    
4. Si aucun événement n’est trouvé dans la file d’attente, un événement StatusEvent est généré et codé dans une réponse de notification.
    
5. La réponse de notification est renvoyée au client.
    
6. Les événements inclus dans la notification sont supprimés de la file d’attente d’abonnement et le dernier filigrane local du serveur d’accès au client pour l’abonnement est définie sur le filigrane du dernier événement renvoyé.
    
7. Le délai d’heure de l’abonnement est réinitialisé.
    
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)


[Utilisation des abonnements Pull](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

