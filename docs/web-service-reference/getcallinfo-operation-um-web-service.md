---
title: Opération GetCallInfo (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 6bccd418-caf7-4eb9-8a6f-410e56a635c3
description: L’opération GetCallInfo renvoie l’état de l’appel sortant qui est spécifiée par l’ID d’appel (service web de messagerie unifiée).
ms.openlocfilehash: 36f9cba3690520ebb457a4cb2bfbcde3fea4b8dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756533"
---
# <a name="getcallinfo-operation-um-web-service"></a>Opération GetCallInfo (service web de messagerie unifiée)

L’opération GetCallInfo renvoie l’état de l’appel sortant qui est spécifiée par [l’ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md).
  
## <a name="getcallinfo-request-example"></a>Exemple de requête GetCallInfo

### <a name="description"></a>Description

L’exemple suivant d’une demande GetCallInfo montre comment former une demande pour obtenir des informations relatives à un appel sortant spécifié.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a>Exemple de réponse GetCallInfo réussie

### <a name="description"></a>Description

Une réponse GetCallInfo l’exemple suivant montre une réponse à une demande de GetCallInfo.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[GetCallInfo (service web de messagerie unifiée)](getcallinfo-um-web-service.md)
  
[GetCallInfoResponse (service web de messagerie unifiée)](getcallinforesponse-um-web-service.md)
  
[ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md)
  
[CallState (service web de messagerie unifiée)](callstate-um-web-service.md)
  
[EventCause (service web de messagerie unifiée)](eventcause-um-web-service.md)

