---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: L’élément RetentionAction spécifie l’action effectuée sur les éléments avec la balise de rétention.
ms.openlocfilehash: ecea4326f0e50460635966991cd55badf8946993
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517944"
---
# <a name="retentionaction"></a>RetentionAction

**L’élément RetentionAction** spécifie l’action effectuée sur les éléments avec la balise de rétention. 
  
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

La valeur de texte de **l’élément RetentionAction** est l’action effectuée sur les éléments. La liste suivante contient les valeurs de texte de **l’élément RetentionAction.** 
  
> **Aucun** : aucune action n’est effectuée sur l’élément. 
    
> **MoveToDeletedItems** : l’élément est déplacé vers le dossier Éléments supprimés par défaut. 
    
> **MoveToFolder** : l’élément est déplacé vers un dossier spécifié. 
    
> **DeleteAndAllowRecovery** : l’élément est supprimé et placé dans le benne. 
    
> **PermanentlyDelete** : l’élément est définitivement supprimé de la boîte aux lettres. 
    
> **MarkAsPastRetentionLimit** : l’élément est marqué comme ayant dépassé la limite de temps de rétention. 
    
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
   

