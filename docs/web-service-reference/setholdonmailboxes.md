---
title: SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fd5b9f0e-23e8-428c-8168-2d6b4ecd6beb
description: L’élément SetHoldOnMailboxes contient une demande SetHoldOnMailboxes.
ms.openlocfilehash: 82ebbbdce04a5b70eae790a899ca089e38aa76d9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516372"
---
# <a name="setholdonmailboxes"></a>SetHoldOnMailboxes

**L’élément SetHoldOnMailboxes contient** une **demande SetHoldOnMailboxes.** 
  
```XML
<SetHoldOnMailboxes>
   <ActionType/>
   <HoldId/>
   <Query/>
   <Mailboxes/>
   <Language/>
   <IncludeNonIndexableItems/>
   <Deduplication/>
   <InPlaceHoldIdentity/>
</SetHoldOnMailboxes>
```

 **SetHoldOnMailboxesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[ActionType (HoldActionType)](actiontype-holdactiontype.md)  |  [HoldId](holdid.md)  |  [Requête](query.md)  |  [Boîtes aux lettres (ArrayOfStringsType)](mailboxes-arrayofstringstype.md)  |  [Langue](language.md)  |  [IncludeNonIndexableItems](includenonindexableitems.md)  |  [Déduplication](deduplication.md)  |  [InPlaceHoldIdentity](inplaceholdidentity.md)
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
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
   

