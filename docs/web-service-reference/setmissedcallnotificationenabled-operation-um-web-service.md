---
title: Opération SetMissedCallNotificationEnabled (service Web de messagerie unifiée)
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
description: L’opération SetMissedCallNotificationEnabled active ou désactive les notifications d’appels manqués.
ms.openlocfilehash: ca4942942a81bc187e8e18a5e6f003f8587f79d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467395"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>Opération SetMissedCallNotificationEnabled (service Web de messagerie unifiée)

L’opération SetMissedCallNotificationEnabled active ou désactive les notifications d’appels manqués.
  
## <a name="setmissedcallnotificationenabled-request-example"></a>Exemple de requête SetMissedCallNotificationEnabled

### <a name="description"></a>Description

L’exemple de requête SetMissedCallNotificationEnabled suivant montre comment créer une demande pour activer les notifications d’appels manqués.
  
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

## <a name="successful-setmissedcallnotificationenabled-response-example"></a>Exemple de réponse SetMissedCallNotificationEnabled réussi

### <a name="description"></a>Description

L’exemple suivant de réponse PlayOnPhoneGreeting indique une réponse à la demande SetMissedCallNotificationEnabled.
  
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



[SetMissedCallNotificationEnabled (service Web de messagerie unifiée)](setmissedcallnotificationenabled-um-web-service.md)
  
[SetMissedCallNotificationEnabledResponse (service Web de messagerie unifiée)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[État (service Web de messagerie unifiée-SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)

