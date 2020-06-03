---
title: Opération de déconnexion (service Web de messagerie unifiée)
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
description: L’opération de déconnexion met fin à l’appel identifié par le CallId spécifié (service Web de messagerie unifiée).
ms.openlocfilehash: a1268f9ea3d879f472e019bf1847fc13d65d1819
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529069"
---
# <a name="disconnect-operation-um-web-service"></a>Opération de déconnexion (service Web de messagerie unifiée)

L’opération de déconnexion met fin à l’appel identifié par le [CallId spécifié (service Web de messagerie unifiée)](callid-um-web-service.md).
  
## <a name="disconnect-request-example"></a>Exemple de demande de déconnexion

### <a name="description"></a>Description

L’exemple de demande de déconnexion ci-dessous montre comment créer une demande de déconnexion d’un appel.
  
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

## <a name="successful-disconnect-response-example"></a>Exemple de réponse de déconnexion réussie

### <a name="description"></a>Description

L’exemple suivant de réponse de déconnexion affiche une réponse à la demande de déconnexion.
  
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

- [Disconnect (service Web de messagerie unifiée)](disconnect-um-web-service.md) 
- [DisconnectResponse (service Web de messagerie unifiée)](disconnectresponse-um-web-service.md) 
- [CallId (service Web de messagerie unifiée)](callid-um-web-service.md)

