---
title: Opération ResetPIN (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: L’opération ResetPIN modifie le code confidentiel (via le mot de passe) avec une nouvelle valeur aléatoire.
ms.openlocfilehash: e6417b86ce17c0d34fe857cf1209a18972cbef63
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829146"
---
# <a name="resetpin-operation-um-web-service"></a>Opération ResetPIN (service web de messagerie unifiée)

L’opération ResetPIN modifie le code confidentiel (via le mot de passe) avec une nouvelle valeur aléatoire.
  
## <a name="remarks"></a>Remarques

L’opération ResetPIN crée un nouveau code confidentiel basé sur les stratégies de code confidentiel. Si l’opération réussit, un message électronique qui contient le nouveau code confidentiel est envoyé à la boîte aux lettres de l’utilisateur. Si l’opération échoue, elle lève une exception qui contient des informations sur l’échec.
  
## <a name="resetpin-request-example"></a>Exemple de requête ResetPIN

### <a name="description"></a>Description

L’exemple suivant d’une demande ResetPIN montre comment former une demande pour réinitialiser le code confidentiel pour une boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a>Exemple de réponse ResetPIN réussie

### <a name="description"></a>Description

Une réponse ResetPIN l’exemple suivant montre une réponse à la demande ResetPIN.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[ResetPIN (service web de messagerie unifiée)](resetpin-um-web-service.md)
  
[ResetPINResponse (service web de messagerie unifiée)](resetpinresponse-um-web-service.md)

