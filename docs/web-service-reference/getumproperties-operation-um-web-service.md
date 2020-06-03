---
title: Opération GetUMProperties (service Web de messagerie unifiée)
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
description: L’opération GetUMProperties obtient toutes les propriétés de messagerie unifiée pour la boîte aux lettres de l’utilisateur qui effectue la demande.
ms.openlocfilehash: 42176d9cd0288af6515aeea616a4f216a419410c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462471"
---
# <a name="getumproperties-operation-um-web-service"></a>Opération GetUMProperties (service Web de messagerie unifiée)

L’opération GetUMProperties obtient toutes les propriétés de messagerie unifiée pour la boîte aux lettres de l’utilisateur qui effectue la demande.
  
## <a name="getumproperties-request-example"></a>Exemple de requête GetUMProperties

### <a name="description"></a>Description

L’exemple de requête GetUMProperties suivant montre comment créer une demande pour obtenir les propriétés de messagerie unifiée d’une boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a>Exemple de réponse GetUMProperties réussi

### <a name="description"></a>Description

L’exemple suivant de réponse GetUMProperties indique une réponse à la demande GetUMProperties.
  
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



[GetUMProperties (service Web de messagerie unifiée)](getumproperties-um-web-service.md)
  
[GetUMPropertiesResponse (service Web de messagerie unifiée)](getumpropertiesresponse-um-web-service.md)

