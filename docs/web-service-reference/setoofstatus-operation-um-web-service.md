---
title: Opération SetOofStatus (service Web de messagerie unifiée)
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
description: L’opération SetOofStatus définit une valeur qui indique si le message d’accueil de l’absence du Bureau doit être lu pour l’utilisateur qui effectue la demande.
ms.openlocfilehash: 2311b6137ac25d15ad3d06668450c1d0f7ec1fad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467353"
---
# <a name="setoofstatus-operation-um-web-service"></a>Opération SetOofStatus (service Web de messagerie unifiée)

L’opération SetOofStatus définit une valeur qui indique si le message d’accueil de l’absence du Bureau doit être lu pour l’utilisateur qui effectue la demande.
  
## <a name="setoofstatus-request-example"></a>Exemple de requête SetOofStatus

### <a name="description"></a>Description

L’exemple de requête SetOofStatus suivant montre comment créer une demande pour activer le message d’accueil d’absence du Bureau pour une boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a>Exemple de réponse SetOofStatus réussi

### <a name="description"></a>Description

L’exemple suivant de réponse SetOofStatus indique une réponse à la demande SetOofStatus.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[SetOofStatus (service Web de messagerie unifiée)](setoofstatus-um-web-service.md)
  
[SetOofStatusResponse (service Web de messagerie unifiée)](setoofstatusresponse-um-web-service.md)
  
[État (service Web de messagerie unifiée-SetOofStatus)](status-um-web-servicesetoofstatus.md)

