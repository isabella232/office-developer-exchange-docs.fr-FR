---
title: Opération IsUMEnabled (service Web de messagerie unifiée)
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
description: L’opération IsUMEnabled détermine si une boîte aux lettres est activée pour la messagerie unifiée.
ms.openlocfilehash: b1478f5a113059251fe1b036ac7d77e5a4ab4f50
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458235"
---
# <a name="isumenabled-operation-um-web-service"></a>Opération IsUMEnabled (service Web de messagerie unifiée)

L’opération IsUMEnabled détermine si une boîte aux lettres est activée pour la messagerie unifiée.
  
## <a name="isumenabled-request-example"></a>Exemple de requête IsUMEnabled

### <a name="description"></a>Description

L’exemple de requête IsUMEnabled suivant montre comment créer une demande pour déterminer si une boîte aux lettres est activée pour la messagerie unifiée.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a>Exemple de réponse IsUMEnabled réussi

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à une demande IsUMEnabled.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[IsUMEnabled (service Web de messagerie unifiée)](isumenabled-um-web-service.md)
  
[IsUMEnabledResponse (service Web de messagerie unifiée)](isumenabledresponse-um-web-service.md)


[Éléments XML de service Web de messagerie unifiée pour Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

