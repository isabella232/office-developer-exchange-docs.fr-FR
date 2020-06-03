---
title: PersonaShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 61d87cd5-3270-40d1-bab7-d0d5bf938607
description: L’élément PersonaShape spécifie l’ensemble de propriétés Persona à renvoyer à partir d’une demande FindPeople.
ms.openlocfilehash: 49cbae714a3b854496dc91ea6102f4b676623690
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457570"
---
# <a name="personashape"></a>PersonaShape

L’élément **PersonaShape** spécifie l’ensemble de propriétés Persona à renvoyer à partir d’une demande **FindPeople** . 
  
```XML
<PersonaShape>
   <BaseShape/>
   <AdditionalProperties/>
</PersonaShape>
```

 **PersonaResponseShapeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[BaseShape](baseshape.md)  |  [AdditionalProperties](additionalproperties.md)
  
### <a name="parent-elements"></a>Éléments parents

[FindPeople](findpeople.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

