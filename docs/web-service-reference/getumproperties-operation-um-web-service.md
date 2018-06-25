---
title: Opération GetUMProperties (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMProperties
api_type:
- schema
ms.assetid: 301fb9a3-67df-44c4-8ffe-0600237fc344
description: L’opération GetUMProperties Obtient toutes les propriétés de la messagerie unifiée pour la boîte aux lettres de l’utilisateur qui effectue la demande.
ms.openlocfilehash: 8878099bbd907fe0648f7d64dde3cd9600c2c45f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827678"
---
# <a name="getumproperties-operation-um-web-service"></a>Opération GetUMProperties (service web de messagerie unifiée)

L’opération GetUMProperties Obtient toutes les propriétés de la messagerie unifiée pour la boîte aux lettres de l’utilisateur qui effectue la demande.
  
## <a name="getumproperties-request-example"></a>Exemple de requête GetUMProperties

### <a name="description"></a>Description

L’exemple suivant d’une demande GetUMProperties montre comment former une demande pour obtenir les propriétés d’une boîte aux lettres de messagerie unifiée.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a>Exemple de réponse GetUMProperties réussie

### <a name="description"></a>Description

Une réponse GetUMProperties l’exemple suivant montre une réponse à la demande GetUMProperties.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetUMPropertiesResponse>
        <OofStatus>false</OofStatus> 
        <MissedCallNotificationEnabled>true</MissedCallNotificationEnabled> 
        <PlayOnPhoneDialString>12345</PlayOnPhoneDialString> 
        <TelephoneAccessNumbers>54321</TelephoneAccessNumbers> 
        <TelephoneAccessFolderEmail>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</TelephoneAccessFolderEmail> 
      </GetUMPropertiesResponse>
    </GetUMPropertiesResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[GetUMProperties (service web de messagerie unifiée)](getumproperties-um-web-service.md)
  
[GetUMPropertiesResponse (service web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md)

