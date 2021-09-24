---
title: PersonaShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 61d87cd5-3270-40d1-bab7-d0d5bf938607
description: L’élément PersonaShape spécifie l’ensemble des propriétés de personnage à retourner à partir d’une demande FindPeople.
ms.openlocfilehash: 41c37be586a033965f5102e7e14af7d7fe205e8f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524580"
---
# <a name="personashape"></a>PersonaShape

**L’élément PersonaShape** spécifie l’ensemble des propriétés de personnage à retourner à partir d’une **demande FindPeople.** 
  
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
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

