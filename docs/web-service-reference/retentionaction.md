---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: L’élément RetentionAction spécifie l’action effectuée sur les éléments à l’aide de la balise de rétention.
ms.openlocfilehash: c16988413e732ddc3cd6ebc355cb73c4d96550c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465232"
---
# <a name="retentionaction"></a>RetentionAction

L’élément **RetentionAction** spécifie l’action effectuée sur les éléments à l’aide de la balise de rétention. 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 **RetentionActionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **RetentionAction** est l’action effectuée sur les éléments. La liste suivante contient les valeurs de texte de l’élément **RetentionAction** . 
  
> **None** : aucune action n’est effectuée sur l’élément. 
    
> **MoveToDeletedItems** -l’élément est déplacé vers le dossier éléments supprimés par défaut. 
    
> **MoveToFolder** : l’élément est déplacé vers un dossier spécifié. 
    
> **DeleteAndAllowRecovery** : l’élément est supprimé et placé dans la benne. 
    
> **PermanentlyDelete** : l’élément est définitivement supprimé de la boîte aux lettres. 
    
> **MarkAsPastRetentionLimit** -l’élément est marqué comme ayant dépassé la limite de temps de rétention. 
    
> **MoveToArchive** : l’élément est déplacé vers la boîte aux lettres d’archivage. 
    
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
   

