---
title: Opération SetPlayOnPhoneDialString (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: L’opération SetPlayOnPhoneDialString définit la chaîne de numérotation à utiliser en tant que la valeur par défaut pour l’opération PlayOnPhone (service web de messagerie unifiée) et l’opération PlayOnPhoneGreeting (service web de messagerie unifiée).
ms.openlocfilehash: 0d1a879784740777e5eab0cbd5f85e59a6479461
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829446"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>Opération SetPlayOnPhoneDialString (service web de messagerie unifiée)

L’opération SetPlayOnPhoneDialString définit la chaîne de numérotation à utiliser en tant que la valeur par défaut pour l' [opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) et l' [opération PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md).
  
## <a name="setplayonphonedialstring-request-example"></a>Exemple de requête SetPlayOnPhoneDialString

### <a name="description"></a>Description

Une demande de SetPlayOnPhoneDialString l’exemple suivant montre comment créer une requête pour définir la chaîne de numérotation par défaut pour une boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a>Exemple de réponse SetPlayOnPhoneDialString réussie

### <a name="description"></a>Description

Une réponse SetPlayOnePhoneDialString l’exemple suivant montre une réponse à la demande SetPlayOnPhoneDialString.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[SetPlayOnPhoneDialString (service web de messagerie unifiée)](setplayonphonedialstring-um-web-service.md)
  
[SetPlayOnPhoneDialStringResponse (service web de messagerie unifiée)](setplayonphonedialstringresponse-um-web-service.md)
  
[dialString (service web de messagerie unifiée)](dialstring-um-web-service.md)

