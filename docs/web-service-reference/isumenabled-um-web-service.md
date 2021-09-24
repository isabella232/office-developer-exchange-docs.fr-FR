---
title: IsUMEnabled (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: 33810bbd-837f-4a71-9ed9-cb4b8c52186d
description: L’élément IsUMEnabled indique si une boîte aux lettres est activée pour la messagerie unifiée.
ms.openlocfilehash: 43632c28c5fb0c526dcf2ad936784953b00cc14a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524118"
---
# <a name="isumenabled-um-web-service"></a>IsUMEnabled (service web de messagerie unifiée)

**L’élément IsUMEnabled** indique si une boîte aux lettres est activée pour la messagerie unifiée. 
  
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

Une valeur de texte qui représente une valeur boolé américaine est requise si cet élément est inclus. La valeur **true indique** que la boîte aux lettres est activée pour la messagerie unifiée. La valeur **false signifie** que la boîte aux lettres n’est pas activée pour la messagerie unifiée. 
  
## <a name="remarks"></a>Remarques

Pour déterminer si une boîte aux lettres est activée pour la messagerie unifiée, utilisez l’opération [IsUMEnabled (service web de messagerie unifiée).](isumenabled-operation-um-web-service.md)
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération IsUMEnabled (service web de messagerie unifiée)](isumenabled-operation-um-web-service.md)


[Éléments XML du service web de messagerie unifiée pour Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

