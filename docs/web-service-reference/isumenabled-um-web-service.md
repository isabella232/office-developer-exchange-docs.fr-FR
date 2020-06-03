---
title: IsUMEnabled (service Web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: 33810bbd-837f-4a71-9ed9-cb4b8c52186d
description: L’élément IsUMEnabled indique si une boîte aux lettres est activée pour la messagerie unifiée.
ms.openlocfilehash: ea5bde677c62664acad8afd5c8142e96d82b7a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458228"
---
# <a name="isumenabled-um-web-service"></a>IsUMEnabled (service Web de messagerie unifiée)

L’élément **IsUMEnabled** indique si une boîte aux lettres est activée pour la messagerie unifiée. 
  
```xml
<IsUMEnabled/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une valeur booléenne est requise si cet élément est inclus. La valeur **true** indique que la boîte aux lettres est activée pour la messagerie unifiée. La valeur **false** signifie que la boîte aux lettres n’est pas activée pour la messagerie unifiée. 
  
## <a name="remarks"></a>Remarques

Pour déterminer si une boîte aux lettres est activée pour la messagerie unifiée, utilisez l' [opération IsUMEnabled (service Web de messagerie unifiée)](isumenabled-operation-um-web-service.md).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération IsUMEnabled (service Web de messagerie unifiée)](isumenabled-operation-um-web-service.md)


[Éléments XML de service Web de messagerie unifiée pour Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

