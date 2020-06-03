---
title: Type (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: L’élément type spécifie le type de dossier utilisé dans une stratégie de rétention.
ms.openlocfilehash: f6fcc7942a530ada2d6e72c3e38286a7595b09ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465106"
---
# <a name="type-elcfoldertype"></a>Type (ElcFolderType)

L’élément **type** spécifie le type de dossier utilisé dans une stratégie de rétention. 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 **ElcFolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **type** est le type de dossier utilisé dans une stratégie de rétention. La valeur de texte peut être une des valeurs suivantes qui représentent un type de dossier par défaut : calendrier, contacts, DeletedItems, brouillons, boîte de réception, JunkEmail, Journal, notes, boîte d’envoi, éléments envoyés, tâches, tout, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, personnel, RecoverableItems ou NonIpmRoot 
  
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
   

