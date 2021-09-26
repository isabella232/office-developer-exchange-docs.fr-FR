---
title: SMTPLast (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: L’élément SMTPLast spécifie si le serveur SMTP (Simple Mail Transfer Protocol) requiert que le courrier électronique soit téléchargé avant d’envoyer des messages électroniques à l’aide du serveur SMTP.
ms.openlocfilehash: ff1e47fa1e3ebd0267879cd596a3a559f2702943
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544681"
---
# <a name="smtplast-pox"></a>SMTPLast (POX)

**L’élément SMTPLast** spécifie si le serveur SMTP (Simple Mail Transfer Protocol) requiert que le courrier électronique soit téléchargé avant d’envoyer des messages électroniques à l’aide du serveur SMTP. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [Protocol (POX)](protocol-pox.md)
  
- [SMTPLast (POX)](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contient les spécifications de connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 où le rôle serveur d’accès au client est installé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte spécifie si le serveur SMTP requiert que le courrier électronique soit téléchargé avant d’envoyer des messages électroniques à l’aide du serveur SMTP. Les valeurs possibles sont **en cours** et **hors.** La valeur par défaut est **off**.
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

