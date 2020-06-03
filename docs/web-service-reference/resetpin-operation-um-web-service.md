---
title: Opération ResetPIN (service Web de messagerie unifiée)
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
description: L’opération ResetPIN modifie le code confidentiel (mot de passe de la TUI) en une nouvelle valeur aléatoire.
ms.openlocfilehash: 8de64ce7a47e9c426f8eb9298e1ca00508fb616c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465491"
---
# <a name="resetpin-operation-um-web-service"></a>Opération ResetPIN (service Web de messagerie unifiée)

L’opération ResetPIN modifie le code confidentiel (mot de passe de la TUI) en une nouvelle valeur aléatoire.
  
## <a name="remarks"></a>Remarques

L’opération ResetPIN crée un nouveau code confidentiel basé sur les stratégies de code confidentiel. Si l’opération réussit, un message électronique contenant le nouveau code confidentiel est envoyé à la boîte aux lettres de l’utilisateur. Si l’opération échoue, elle génère une exception qui contient des informations sur l’échec.
  
## <a name="resetpin-request-example"></a>Exemple de requête ResetPIN

### <a name="description"></a>Description

L’exemple de requête ResetPIN suivant indique comment créer une demande de réinitialisation du code confidentiel d’une boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a>Exemple de réponse ResetPIN réussi

### <a name="description"></a>Description

L’exemple suivant de réponse ResetPIN indique une réponse à la demande ResetPIN.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



[ResetPIN (service Web de messagerie unifiée)](resetpin-um-web-service.md)
  
[ResetPINResponse (service Web de messagerie unifiée)](resetpinresponse-um-web-service.md)

