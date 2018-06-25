---
title: Opération IsUMEnabled (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: fbe6cd95-f7a5-42b9-8a9d-b6159a269d55
description: L’opération IsUMEnabled détermine si une boîte aux lettres est activé pour la messagerie unifiée.
ms.openlocfilehash: 9d94a359d6b11e41762d21aa2fe5501bd9f7b577
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828107"
---
# <a name="isumenabled-operation-um-web-service"></a>Opération IsUMEnabled (service web de messagerie unifiée)

L’opération IsUMEnabled détermine si une boîte aux lettres est activé pour la messagerie unifiée.
  
## <a name="isumenabled-request-example"></a>Exemple de requête IsUMEnabled

### <a name="description"></a>Description

L’exemple suivant d’une demande IsUMEnabled montre comment former une demande pour déterminer si une boîte aux lettres est activée pour la messagerie unifiée.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a>Exemple de réponse IsUMEnabled réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse positive à une demande de IsUMEnabled.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[IsUMEnabled (service web de messagerie unifiée)](isumenabled-um-web-service.md)
  
[IsUMEnabledResponse (service web de messagerie unifiée)](isumenabledresponse-um-web-service.md)


[Unified Messaging service XML des éléments web pour Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

