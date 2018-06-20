---
title: Opération SetMissedCallNotificationEnabled (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetMissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 6693b5db-ac6b-43bc-af83-a9c94fc425bf
description: L’opération SetMissedCallNotificationEnabled Active ou désactive les notifications d’appels manqués.
ms.openlocfilehash: be9479d6ed2c5238ed19c3d22e028fca62b8deed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829434"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>Opération SetMissedCallNotificationEnabled (service web de messagerie unifiée)

L’opération SetMissedCallNotificationEnabled Active ou désactive les notifications d’appels manqués.
  
## <a name="setmissedcallnotificationenabled-request-example"></a>Exemple de requête SetMissedCallNotificationEnabled

### <a name="description"></a>Description

L’exemple suivant d’une demande SetMissedCallNotificationEnabled montre comment former une demande pour activer les notifications d’appels manqués.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a>Exemple de réponse SetMissedCallNotificationEnabled réussie

### <a name="description"></a>Description

Une réponse PlayOnPhoneGreeting l’exemple suivant montre une réponse à la demande SetMissedCallNotificationEnabled.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[SetMissedCallNotificationEnabled (service web de messagerie unifiée)](setmissedcallnotificationenabled-um-web-service.md)
  
[SetMissedCallNotificationEnabledResponse (service web de messagerie unifiée)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[État (service web de messagerie unifiée - SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)

