---
title: Type (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: L’élément de Type spécifie le type de dossier utilisé dans une stratégie de rétention.
ms.openlocfilehash: f679a9237a577d26d4b28e1b25f3e135f7193903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838780"
---
# <a name="type-elcfoldertype"></a>Type (ElcFolderType)

L’élément de **Type** Spécifie le type de dossier utilisé dans une stratégie de rétention. 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 **ElcFolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **Type** est le type de dossier utilisé dans une stratégie de rétention. La valeur de texte peut être une des valeurs suivantes qui représentent un type de dossier par défaut : calendrier, Contacts, DeletedItems, Brouillons, boîte de réception, JunkEmail, Journal, Notes, boîte d’envoi, éléments envoyés, tâches, All, ManagedCustomFolder, RssSubscriptions, SyncIssues, ConversationHistory, personnel, RecoverableItems ou NonIpmRoot 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

