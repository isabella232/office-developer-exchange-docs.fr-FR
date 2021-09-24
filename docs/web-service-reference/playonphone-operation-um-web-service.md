---
title: Opération PlayOnPhone (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 7d55be55-f8b6-4e96-a61e-26fa190217fd
description: L’opération PlayOnPhone effectue un appel sortant et lit un message spécifié par téléphone, spécifié par l’élément DialString.
ms.openlocfilehash: 4d18727da18c36e6410c3cc6ab3bbf873993be72
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516563"
---
# <a name="playonphone-operation-um-web-service"></a>Opération PlayOnPhone (service web de messagerie unifiée)

L’opération PlayOnPhone effectue un appel sortant et lit un message spécifié par téléphone, spécifié par **l’élément DialString.** 
  
## <a name="playonphone-request-example"></a>Exemple de requête PlayOnPhone

### <a name="description"></a>Description

L’exemple suivant d’une demande PlayOnPhone montre comment former une demande pour passer un appel sortant et lire un message.
  
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

## <a name="successful-playonphone-response-example"></a>Exemple de réponse PlayOnPhone réussie

### <a name="description"></a>Description

L’exemple suivant d’une réponse PlayOnPhone affiche une réponse à la demande PlayOnPhone.
  
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



[PlayOnPhone (service web de messagerie unifiée)](playonphone-um-web-service.md)
  
[PlayOnPhoneResponse (service web de messagerie unifiée)](playonphoneresponse-um-web-service.md)
  
[Opération PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md)

