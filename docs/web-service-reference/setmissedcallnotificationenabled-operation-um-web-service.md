---
title: Opération SetMissedCallNotificationEnabled (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetMissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 6693b5db-ac6b-43bc-af83-a9c94fc425bf
description: L’opération SetMissedCallNotificationEnabled active ou désactive les notifications d’appels manqués.
ms.openlocfilehash: 31f59887041aac02e5876b596931902373870203
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521416"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>Opération SetMissedCallNotificationEnabled (service web de messagerie unifiée)

L’opération SetMissedCallNotificationEnabled active ou désactive les notifications d’appels manqués.
  
## <a name="setmissedcallnotificationenabled-request-example"></a>Exemple de requête SetMissedCallNotificationEnabled

### <a name="description"></a>Description

L’exemple suivant d’une demande SetMissedCallNotificationEnabled montre comment former une demande pour activer les notifications d’appels en manque.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a>Exemple de réponse SetMissedCallNotificationEnabled réussie

### <a name="description"></a>Description

L’exemple suivant d’une réponse PlayOnPhoneGreeting montre une réponse à la demande SetMissedCallNotificationEnabled.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[SetMissedCallNotificationEnabled (service web de messagerie unifiée)](setmissedcallnotificationenabled-um-web-service.md)
  
[SetMissedCallNotificationEnabledResponse (service web de messagerie unifiée)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[Statut (service web de messagerie unifiée - SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)

