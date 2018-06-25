---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: L’élément RetentionAction Spécifie l’action effectuée sur les éléments avec la balise de rétention.
ms.openlocfilehash: 54a1038f2e56aad66f89522423ccfbd69dc44a80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829215"
---
# <a name="retentionaction"></a>RetentionAction

L’élément **RetentionAction** Spécifie l’action effectuée sur les éléments avec la balise de rétention. 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 **RetentionActionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **RetentionAction** est l’action exécutée sur les éléments. La liste suivante contient les valeurs de texte de l’élément **RetentionAction** . 
  
> **Aucun** - aucune action n’est effectuée sur l’élément. 
    
> **MoveToDeletedItems** - l’élément est déplacé vers le dossier éléments supprimés par défaut. 
    
> **MoveToFolder** - l’élément est déplacé vers un dossier spécifié. 
    
> **DeleteAndAllowRecovery** - l’élément est supprimé et placer dans la benne. 
    
> **PermanentlyDelete** - l’élément est définitivement supprimé de la boîte aux lettres. 
    
> **MarkAsPastRetentionLimit** - l’élément est marqué comme ayant dépassé la limite de temps de rétention. 
    
> **MoveToArchive** - l’élément est déplacé vers la boîte aux lettres d’archive. 
    
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

