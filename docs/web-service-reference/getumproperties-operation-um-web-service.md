---
title: Opération GetUMProperties (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetUMProperties
api_type:
- schema
ms.assetid: 301fb9a3-67df-44c4-8ffe-0600237fc344
description: L’opération GetUMProperties obtient toutes les propriétés de messagerie unifiée de la boîte aux lettres de l’utilisateur qui fait la demande.
ms.openlocfilehash: 8d051196e83e1f927692b517e1ab3e95bb0060db
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515816"
---
# <a name="getumproperties-operation-um-web-service"></a>Opération GetUMProperties (service web de messagerie unifiée)

L’opération GetUMProperties obtient toutes les propriétés de messagerie unifiée de la boîte aux lettres de l’utilisateur qui fait la demande.
  
## <a name="getumproperties-request-example"></a>Exemple de requête GetUMProperties

### <a name="description"></a>Description

L’exemple suivant d’une demande GetUMProperties montre comment former une demande pour obtenir les propriétés de messagerie unifiée d’une boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a>Exemple de réponse GetUMProperties réussie

### <a name="description"></a>Description

L’exemple suivant d’une réponse GetUMProperties affiche une réponse à la demande GetUMProperties.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

