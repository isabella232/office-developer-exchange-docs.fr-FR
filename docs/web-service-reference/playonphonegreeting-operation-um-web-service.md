---
title: Opération PlayOnPhoneGreeting (service Web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 6deafc40-290b-4bce-9914-b6bcc529f38a
description: L’opération PlayOnPhoneGreeting effectue un appel sortant et joue l’un des deux messages de salutation sur le téléphone.
ms.openlocfilehash: 3af120b9ac8d7a368742fad2850c924228488662
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528894"
---
# <a name="playonphonegreeting-operation-um-web-service"></a>Opération PlayOnPhoneGreeting (service Web de messagerie unifiée)

L’opération PlayOnPhoneGreeting effectue un appel sortant et joue l’un des deux messages de salutation sur le téléphone.
  
## <a name="playonphonegreeting-request-example"></a>Exemple de requête PlayOnPhoneGreeting

### <a name="description"></a>Description

L’exemple de requête PlayOnPhoneGreeting suivant montre comment créer une demande d’émission d’un appel sortant et lire le message d’accueil normal sur un téléphone.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhoneGreeting xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GreetingType>NormalCustom</GreetingType>
      <DialString>12345</DialString>
    </PlayOnPhoneGreeting>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphonegreeting-response-example"></a>Exemple de réponse PlayOnPhoneGreeting réussi

### <a name="description"></a>Description

L’exemple suivant de réponse PlayOnPhoneGreeting indique une réponse à la demande PlayOnPhoneGreeting.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneGreetingResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <PlayOnPhoneGreetingResponse>MjA4MTQ5MmItMTBmZC00ZGFmLThiMzEtNDllNDJjM2Y3MjIxQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneGreetingResponse> 
    </PlayOnPhoneGreetingResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-um-web-service.md)
  
[PlayOnPhoneGreetingResponse (service Web de messagerie unifiée)](playonphonegreetingresponse-um-web-service.md)
  
[GreetingType (service Web de messagerie unifiée)](greetingtype-um-web-service.md)
  
[dialString (service Web de messagerie unifiée)](dialstring-um-web-service.md)

