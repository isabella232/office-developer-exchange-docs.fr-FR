---
title: State (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: L’élément State contient l’état de cycle de vie qui est définie sur une boîte aux lettres de site.
ms.openlocfilehash: 5189ee8573fd33d2265fd60c47bb40d17b16b8fe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538967"
---
# <a name="state-teammailboxlifecyclestatetype"></a>State (TeamMailboxLifecycleStateType)

**L’élément State** contient l’état de cycle de vie qui est définie sur une boîte aux lettres de site. 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

**TeamMailboxLifecycleStateType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SetTeamMailbox](setteammailbox.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément State** est l’état de cycle de vie qui est définie sur une boîte aux lettres de site. La valeur texte **Active** indique qu’une boîte aux lettres de site est en cours d’utilisation. La valeur de texte **Closed** indique qu’une boîte aux lettres de site a été fermée et qu’elle n’est pas en cours d’utilisation. La valeur texte **Unlinked** indique qu’une boîte aux lettres de site n’est pas liée à un environnement de collaboration web. Les **valeurs Active**, **Closed** et **PendingDelete** s’excluent mutuellement, mais la valeur **Unlinked** n’est pas mutuellement exclusive des autres valeurs. La valeur de texte **PendingDelete** indique qu’une boîte aux lettres de site est en attente de suppression. Une boîte aux lettres de site doit être fermée avant de pouvoir être définie comme **PendingDelete**.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

