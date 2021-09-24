---
title: IsNotSupported
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsNotSupported
api_type:
- schema
ms.assetid: 4db469ae-1515-47ea-9905-6aabf199febd
description: L’élément IsNotSupported indique si la règle ne peut pas être modifiée à l’aide des API de code géré.
ms.openlocfilehash: 4a123acbce3019d9ac5fcdb4cbfa2b60dd4529fe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514542"
---
# <a name="isnotsupported"></a>IsNotSupported

**L’élément IsNotSupported** indique si la règle ne peut pas être modifiée à l’aide des API de code géré. 
  
```XML
<IsNotSupported/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Règle (RuleType)](rule-ruletype.md) <br/> |Représente une règle dans la boîte aux lettres de l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** indique que la règle ne peut pas être modifiée à l’aide des API de code géré. La valeur **false indique** que la règle peut être modifiée à l’aide des API de code géré. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

