---
title: Opération PlayOnPhone (service Web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 7d55be55-f8b6-4e96-a61e-26fa190217fd
description: L’opération PlayOnPhone effectue un appel sortant et lit un message spécifié sur le téléphone spécifié par l’élément DialString.
ms.openlocfilehash: c5ff82bcd822aa2c659d1782ea4a1349d198bc80
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466233"
---
# <a name="playonphone-operation-um-web-service"></a>Opération PlayOnPhone (service Web de messagerie unifiée)

L’opération PlayOnPhone effectue un appel sortant et lit un message spécifié sur le téléphone spécifié par l’élément **DialString** . 
  
## <a name="playonphone-request-example"></a>Exemple de requête PlayOnPhone

### <a name="description"></a>Description

L’exemple de requête PlayOnPhone suivant montre comment créer une demande pour passer un appel sortant et émettre un message.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhone xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <entryId>AAAAAGsd2rbQLVtLobUGbrq/9IUHAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAACxVpEl+KVVLl957wp//x6UAGAetcDUAAA==</entryId>
      <DialString>12345</DialString>
    </PlayOnPhone>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphone-response-example"></a>Exemple de réponse PlayOnPhone réussi

### <a name="description"></a>Description

L’exemple suivant de réponse PlayOnPhone indique une réponse à la demande PlayOnPhone.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <PlayOnPhoneResponse>NDEzYjEzNmMtZTE2Zi00NTJlLWI3YzctNDhkMTE3MDE3YjlmQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneResponse> 
    </PlayOnPhoneResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[PlayOnPhone (service Web de messagerie unifiée)](playonphone-um-web-service.md)
  
[PlayOnPhoneResponse (service Web de messagerie unifiée)](playonphoneresponse-um-web-service.md)
  
[Opération PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md)

