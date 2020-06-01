---
title: Opération SetPlayOnPhoneDialString (service Web de messagerie unifiée)
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
description: L’opération SetPlayOnPhoneDialString définit la chaîne de numérotation à utiliser par défaut pour l’opération PlayOnPhone (service Web de messagerie unifiée) et l’opération PlayOnPhoneGreeting (service Web de messagerie unifiée).
ms.openlocfilehash: 7df806eedc2d6d037394f31ec4ccbfe28aaf3372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458641"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>Opération SetPlayOnPhoneDialString (service Web de messagerie unifiée)

L’opération SetPlayOnPhoneDialString définit la chaîne de numérotation à utiliser par défaut pour l' [opération PlayOnPhone (service Web de messagerie unifiée)](playonphone-operation-um-web-service.md) et l' [opération PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md).
  
## <a name="setplayonphonedialstring-request-example"></a>Exemple de requête SetPlayOnPhoneDialString

### <a name="description"></a>Description

L’exemple de requête SetPlayOnPhoneDialString suivant montre comment créer une demande de définition de la chaîne de numérotation par défaut pour une boîte aux lettres.
  
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

## <a name="successful-setplayonphonedialstring-response-example"></a>Exemple de réponse SetPlayOnPhoneDialString réussi

### <a name="description"></a>Description

L’exemple suivant de réponse SetPlayOnePhoneDialString indique une réponse à la demande SetPlayOnPhoneDialString.
  
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



[SetPlayOnPhoneDialString (service Web de messagerie unifiée)](setplayonphonedialstring-um-web-service.md)
  
[SetPlayOnPhoneDialStringResponse (service Web de messagerie unifiée)](setplayonphonedialstringresponse-um-web-service.md)
  
[dialString (service Web de messagerie unifiée)](dialstring-um-web-service.md)

