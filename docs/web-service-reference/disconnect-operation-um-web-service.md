---
title: (Service web de messagerie unifiée) de l’opération de déconnexion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: a987000b-d6e6-49d7-944c-e9c278d0236f
description: L’opération de déconnexion met fin à l’appel est identifié par l’ID d’appel (service web de messagerie unifiée) spécifié.
ms.openlocfilehash: 1e04e65fa1951a6aa46e2c8b6dd5fe524c84a8fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755960"
---
# <a name="disconnect-operation-um-web-service"></a>(Service web de messagerie unifiée) de l’opération de déconnexion

L’opération de déconnexion met fin à l’appel est identifié par [l’ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md)de spécifié.
  
## <a name="disconnect-request-example"></a>Exemple de requête de déconnexion

### <a name="description"></a>Description

Une demande de déconnexion l’exemple suivant montre comment former une demande de déconnexion d’un appel.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a>Exemple de réponse de déconnexion réussie

### <a name="description"></a>Description

L’exemple suivant d’une réponse de déconnexion montre une réponse à la demande de déconnexion.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi

- [Déconnecter (service web de messagerie unifiée)](disconnect-um-web-service.md) 
- [DisconnectResponse (service web de messagerie unifiée)](disconnectresponse-um-web-service.md) 
- [ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md)

