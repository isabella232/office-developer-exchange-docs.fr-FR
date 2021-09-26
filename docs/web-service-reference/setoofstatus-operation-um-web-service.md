---
title: Opération SetOofStatus (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: L’opération SetOofStatus définit une valeur qui indique si le message d’accueil d’absence du Office doit être lus pour l’utilisateur qui effectue la demande.
ms.openlocfilehash: ce736e7d7bea39f65843923187af3ae616ae1c86
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544751"
---
# <a name="setoofstatus-operation-um-web-service"></a>Opération SetOofStatus (service web de messagerie unifiée)

L’opération SetOofStatus définit une valeur qui indique si le message d’accueil d’absence du Office doit être lus pour l’utilisateur qui effectue la demande.
  
## <a name="setoofstatus-request-example"></a>Exemple de requête SetOofStatus

### <a name="description"></a>Description

L’exemple suivant d’une demande SetOofStatus montre comment former une demande pour activer le message d’accueil Office d’une boîte aux lettres.
  
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

## <a name="successful-setoofstatus-response-example"></a>Exemple de réponse SetOofStatus réussie

### <a name="description"></a>Description

L’exemple suivant d’une réponse SetOofStatus affiche une réponse à la demande SetOofStatus.
  
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



[SetOofStatus (service web de messagerie unifiée)](setoofstatus-um-web-service.md)
  
[SetOofStatusResponse (service web de messagerie unifiée)](setoofstatusresponse-um-web-service.md)
  
[Statut (service web de messagerie unifiée - SetOofStatus)](status-um-web-servicesetoofstatus.md)

