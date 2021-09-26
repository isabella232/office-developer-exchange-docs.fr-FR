---
title: Opération PlayOnPhoneGreeting (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 6deafc40-290b-4bce-9914-b6bcc529f38a
description: L’opération PlayOnPhoneGreeting effectue un appel sortant et lit l’un des deux messages d’accueil au téléphone.
ms.openlocfilehash: 540cd44d35e70e2588446996aec19aeab17f83e9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543134"
---
# <a name="playonphonegreeting-operation-um-web-service"></a>Opération PlayOnPhoneGreeting (service web de messagerie unifiée)

L’opération PlayOnPhoneGreeting effectue un appel sortant et lit l’un des deux messages d’accueil au téléphone.
  
## <a name="playonphonegreeting-request-example"></a>Exemple de requête PlayOnPhoneGreeting

### <a name="description"></a>Description

L’exemple suivant d’une demande PlayOnPhoneGreeting montre comment former une demande pour passer un appel sortant et lire le message d’accueil normal sur un téléphone.
  
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

## <a name="successful-playonphonegreeting-response-example"></a>Exemple de réponse PlayOnPhoneGreeting réussie

### <a name="description"></a>Description

L’exemple suivant d’une réponse PlayOnPhoneGreeting affiche une réponse à la demande PlayOnPhoneGreeting.
  
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



[PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-um-web-service.md)
  
[PlayOnPhoneGreetingResponse (service web de messagerie unifiée)](playonphonegreetingresponse-um-web-service.md)
  
[GreetingType (service web de messagerie unifiée)](greetingtype-um-web-service.md)
  
[dialString (service web de messagerie unifiée)](dialstring-um-web-service.md)

