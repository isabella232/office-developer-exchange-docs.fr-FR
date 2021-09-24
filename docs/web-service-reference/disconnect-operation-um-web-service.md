---
title: Opération de déconnexion (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- Disconnect
api_type:
- schema
ms.assetid: a987000b-d6e6-49d7-944c-e9c278d0236f
description: L’opération Disconnect met fin à l’appel identifié par le callid spécifié (service web de um).
ms.openlocfilehash: 42e069233fbfc255d43983571c0bb28475a1fe90
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522011"
---
# <a name="disconnect-operation-um-web-service"></a>Opération de déconnexion (service web de messagerie unifiée)

L’opération Disconnect met fin à l’appel identifié par le [CallId spécifié (service web de la um).](callid-um-web-service.md)
  
## <a name="disconnect-request-example"></a>Exemple de demande de déconnexion

### <a name="description"></a>Description

L’exemple suivant d’une demande de déconnexion montre comment former une demande pour déconnecter un appel.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a>Exemple de réponse Déconnexion réussie

### <a name="description"></a>Description

L’exemple suivant de réponse Disconnect affiche une réponse à la demande Disconnect.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi

- [Disconnect (service web de messagerie unifiée)](disconnect-um-web-service.md) 
- [DisconnectResponse (service web de messagerie unifiée)](disconnectresponse-um-web-service.md) 
- [CallId (service web de messagerie unifiée)](callid-um-web-service.md)

