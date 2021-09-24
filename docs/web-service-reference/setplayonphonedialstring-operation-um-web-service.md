---
title: Opération SetPlayOnPhoneDialString (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: L’opération SetPlayOnPhoneDialString définit la chaîne de numérotation à utiliser comme valeur par défaut pour l’opération PlayOnPhone (service web de um) et l’opération PlayOnPhoneGreeting (service web de um).
ms.openlocfilehash: 89f83d7b0a1d56cb0adeccbf4fa0bb67f1197253
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531908"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>Opération SetPlayOnPhoneDialString (service web de messagerie unifiée)

L’opération SetPlayOnPhoneDialString définit la chaîne de numérotation à utiliser comme valeur par défaut pour l’opération [PlayOnPhone (service web](playonphone-operation-um-web-service.md) de la um) et l’opération [PlayOnPhoneGreeting (service web](playonphonegreeting-operation-um-web-service.md)de um).
  
## <a name="setplayonphonedialstring-request-example"></a>Exemple de requête SetPlayOnPhoneDialString

### <a name="description"></a>Description

L’exemple suivant d’une demande SetPlayOnPhoneDialString montre comment former une demande pour définir la chaîne de numérotation par défaut d’une boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a>Exemple de réponse SetPlayOnPhoneDialString réussie

### <a name="description"></a>Description

L’exemple suivant d’une réponse SetPlayOnePhoneDialString affiche une réponse à la demande SetPlayOnPhoneDialString.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[SetPlayOnPhoneDialString (service web de messagerie unifiée)](setplayonphonedialstring-um-web-service.md)
  
[SetPlayOnPhoneDialStringResponse (service web de messagerie unifiée)](setplayonphonedialstringresponse-um-web-service.md)
  
[dialString (service web de messagerie unifiée)](dialstring-um-web-service.md)

