---
title: État (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: L’élément State contient l’état du cycle de vie qui est défini sur une boîte aux lettres de site.
ms.openlocfilehash: 597946b48649d997f8dd57823b4e0fcc091a6f84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465162"
---
# <a name="state-teammailboxlifecyclestatetype"></a>État (TeamMailboxLifecycleStateType)

L’élément **State** contient l’état du cycle de vie qui est défini sur une boîte aux lettres de site. 
  
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

La valeur de texte de l’élément **State** est l’état de cycle de vie défini sur une boîte aux lettres de site. Une valeur de texte **active** indique qu’une boîte aux lettres de site est en cours d’utilisation. Une valeur de texte **fermé** indique qu’une boîte aux lettres de site a été fermée et qu’elle n’est pas en cours d’utilisation. Une valeur de texte non **liée indique qu'** une boîte aux lettres de site n’est pas liée à un environnement de collaboration Web. Les valeurs **active**, **Closed**et **PendingDelete** s’excluent mutuellement, mais la valeur non **liée** n’est pas mutuellement exclusive par les autres valeurs. Une valeur de texte de **PendingDelete** indique qu’une boîte aux lettres de site est en attente de suppression. Une boîte aux lettres de site doit être fermée pour pouvoir être définie comme **PendingDelete**.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> ||
   

