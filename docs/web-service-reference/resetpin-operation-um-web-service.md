---
title: Opération ResetPIN (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: L’opération ResetPIN modifie le code confidentiel (mot de passe TUI) en une nouvelle valeur aléatoire.
ms.openlocfilehash: 12f1e5719184df84f6c29ab3d02cc362f87abc76
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539107"
---
# <a name="resetpin-operation-um-web-service"></a>Opération ResetPIN (service web de messagerie unifiée)

L’opération ResetPIN modifie le code confidentiel (mot de passe TUI) en une nouvelle valeur aléatoire.
  
## <a name="remarks"></a>Remarques

L’opération ResetPIN crée un code confidentiel basé sur les stratégies de code confidentiel. Si l’opération réussit, un message électronique contenant le nouveau code confidentiel est envoyé à la boîte aux lettres de l’utilisateur. Si l’opération échoue, une exception contenant des informations sur l’échec est lancée.
  
## <a name="resetpin-request-example"></a>Exemple de requête ResetPIN

### <a name="description"></a>Description

L’exemple suivant d’une demande ResetPIN montre comment créer une demande de réinitialisation du code confidentiel d’une boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a>Exemple de réponse ResetPIN réussie

### <a name="description"></a>Description

L’exemple suivant d’une réponse ResetPIN montre une réponse à la demande ResetPIN.
  
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



[ResetPIN (service web de messagerie unifiée)](resetpin-um-web-service.md)
  
[ResetPINResponse (service web de messagerie unifiée)](resetpinresponse-um-web-service.md)

