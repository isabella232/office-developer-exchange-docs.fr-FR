---
title: RetentionPolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: L’élément RetentionPolicyTag spécifie la stratégie de rétention pour un élément de boîte aux lettres.
ms.openlocfilehash: 3ece841e14e6cf11ab15e4a4d8b83a778ae32e46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465176"
---
# <a name="retentionpolicytag"></a>RetentionPolicyTag

L’élément **RetentionPolicyTag** spécifie la stratégie de rétention pour un élément de boîte aux lettres. 
  
```XML
<RetentionPolicyTag>
   <DisplayName/>
   <RetentionId/>
   <RetentionPeriod/>
   <Type/>
   <RetentionAction/>
   <Description/>
   <IsVisible/>
   <OptedInto/>
   <IsArchive/>
</RetentionPolicyTag>
```

 **RetentionPolicyTagType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[DisplayName (String)](displayname-string.md)  |  [RetentionId](retentionid.md)  |  [RetentionPeriod](retentionperiod.md)  |  [Type (ElcFolderType)](type-elcfoldertype.md)  |  [RetentionAction](retentionaction.md)  |  [Description](description.md)  |  [IsVisible](isvisible.md)  |  [OptedInto](optedinto.md)  |  [IsArchive](isarchive.md)
  
### <a name="parent-elements"></a>Éléments parents

[RetentionPolicyTags](retentionpolicytags.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

