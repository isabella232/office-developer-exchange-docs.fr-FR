---
title: Opération GetCallInfo (service Web de messagerie unifiée)
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
description: L’opération GetCallInfo renvoie l’état de l’appel sortant spécifié par CallId (service Web de messagerie unifiée).
ms.openlocfilehash: 6b5664dfe16f9c74cc7175098145141b815a6355
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461239"
---
# <a name="getcallinfo-operation-um-web-service"></a>Opération GetCallInfo (service Web de messagerie unifiée)

L’opération GetCallInfo renvoie l’état de l’appel sortant spécifié par [CallId (service Web de messagerie unifiée)](callid-um-web-service.md).
  
## <a name="getcallinfo-request-example"></a>Exemple de requête GetCallInfo

### <a name="description"></a>Description

L’exemple de requête GetCallInfo suivant montre comment créer une demande pour obtenir des informations sur un appel sortant spécifié.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a>Exemple de réponse GetCallInfo réussi

### <a name="description"></a>Description

L’exemple suivant de réponse GetCallInfo indique une réponse à une demande GetCallInfo.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[GetCallInfo (service Web de messagerie unifiée)](getcallinfo-um-web-service.md)
  
[GetCallInfoResponse (service Web de messagerie unifiée)](getcallinforesponse-um-web-service.md)
  
[CallId (service Web de messagerie unifiée)](callid-um-web-service.md)
  
[CallState (service Web de messagerie unifiée)](callstate-um-web-service.md)
  
[EventCause (service Web de messagerie unifiée)](eventcause-um-web-service.md)

