---
title: Opération PlayOnPhone (service web de messagerie unifiée)
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
description: L’opération PlayOnPhone effectue un appel sortant et lit un message spécifié par téléphone qui est spécifié par l’élément DialString.
ms.openlocfilehash: b55bb45d6654f57503879f33e1cd5013ddb69a2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828818"
---
# <a name="playonphone-operation-um-web-service"></a>Opération PlayOnPhone (service web de messagerie unifiée)

L’opération PlayOnPhone effectue un appel sortant et lit un message spécifié par téléphone qui est spécifié par l’élément **DialString** . 
  
## <a name="playonphone-request-example"></a>Exemple de requête PlayOnPhone

### <a name="description"></a>Description

L’exemple suivant d’une demande PlayOnPhone montre comment former une demande pour émettre un appel et lire un message.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhone xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <entryId>AAAAAGsd2rbQLVtLobUGbrq/9IUHAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAACxVpEl+KVVLl957wp//x6UAGAetcDUAAA==</entryId>
      <DialString>12345</DialString>
    </PlayOnPhone>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphone-response-example"></a>Exemple de réponse PlayOnPhone réussie

### <a name="description"></a>Description

Une réponse PlayOnPhone l’exemple suivant montre une réponse à la demande PlayOnPhone.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <PlayOnPhoneResponse>NDEzYjEzNmMtZTE2Zi00NTJlLWI3YzctNDhkMTE3MDE3YjlmQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneResponse> 
    </PlayOnPhoneResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[PlayOnPhone (service web de messagerie unifiée)](playonphone-um-web-service.md)
  
[PlayOnPhoneResponse (service web de messagerie unifiée)](playonphoneresponse-um-web-service.md)
  
[Opération PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md)

