---
title: État (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: L’élément d’état contient l’état du cycle de vie est définie sur une boîte aux lettres du site.
ms.openlocfilehash: accd70d36cc34e7364387b98a2e94c56b91f012f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829571"
---
# <a name="state-teammailboxlifecyclestatetype"></a>État (TeamMailboxLifecycleStateType)

L’élément **d’état** contient l’état du cycle de vie est définie sur une boîte aux lettres du site. 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

**TeamMailboxLifecycleStateType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SetTeamMailbox](setteammailbox.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **d’état** est l’état du cycle de vie est définie sur une boîte aux lettres du site. Une valeur texte **actif** indique qu’une boîte aux lettres du site est en cours d’utilisation. Une valeur texte **fermé** indique qu’une boîte aux lettres de site a été fermée et n’est pas en cours d’utilisation. Une valeur texte **non liés** indique qu’une boîte aux lettres du site n’est pas liée à un environnement de collaboration basée sur le web. Les valeurs **actives**, **fermé**et **PendingDelete** s’excluent mutuellement, mais la valeur **non liés** n’est pas mutuellement, sans compter les autres valeurs. Une valeur texte **PendingDelete** indique qu’une boîte aux lettres du site est en attente de suppression. Une boîte aux lettres de site doit être fermé avant qu’il peut être définie en tant que **PendingDelete**.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

