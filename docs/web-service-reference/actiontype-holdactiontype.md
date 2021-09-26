---
title: ActionType (HoldActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: L’élément ActionType indique le type d’action pour la attente.
ms.openlocfilehash: 30028da4df2a53a4cd0066823872de5e586020f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546839"
---
# <a name="actiontype-holdactiontype"></a>ActionType (HoldActionType)

**L’élément ActionType** indique le type d’action pour la attente. 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 **HoldActionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément ActionType** est le type de mise en attente définie sur une boîte aux lettres. La valeur de texte **Create** indique qu’une boîte aux lettres sera créée. La valeur texte **Update** indique qu’une mise en attente de boîte aux lettres sera mise à jour. La valeur de texte **Remove** indique qu’une boîte aux lettres de la boîte aux lettres sera supprimée. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

