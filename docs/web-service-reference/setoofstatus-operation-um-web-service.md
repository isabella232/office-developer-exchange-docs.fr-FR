---
title: Opération SetOofStatus (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: L’opération SetOofStatus définit une valeur qui indique si le message d’accueil d’absence du bureau (OOF) doit être lu de l’utilisateur qui effectue la demande.
ms.openlocfilehash: 2bb1deeec8ddb5be56979bfb2fae3396672298a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829445"
---
# <a name="setoofstatus-operation-um-web-service"></a>Opération SetOofStatus (service web de messagerie unifiée)

L’opération SetOofStatus définit une valeur qui indique si le message d’accueil d’absence du bureau (OOF) doit être lu de l’utilisateur qui effectue la demande.
  
## <a name="setoofstatus-request-example"></a>Exemple de requête SetOofStatus

### <a name="description"></a>Description

Une demande de SetOofStatus l’exemple suivant montre comment créer une requête pour activer le message d’accueil d’absence du bureau pour une boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a>Exemple de réponse SetOofStatus réussie

### <a name="description"></a>Description

Une réponse SetOofStatus l’exemple suivant montre une réponse à la demande SetOofStatus.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[SetOofStatus (service web de messagerie unifiée)](setoofstatus-um-web-service.md)
  
[SetOofStatusResponse (service web de messagerie unifiée)](setoofstatusresponse-um-web-service.md)
  
[État (service web de messagerie unifiée - SetOofStatus)](status-um-web-servicesetoofstatus.md)

