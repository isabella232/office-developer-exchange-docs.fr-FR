---
title: Utilisateurs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20ef18c2-daa0-4f65-a515-e84e9993a77f
description: L’élément assigner spécifie les personnes auxquelles une tâche est affectée.
ms.openlocfilehash: 3e98273e859dbe2128b0ad3b4df42c8016fd3bc5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464713"
---
# <a name="assignees"></a>Utilisateurs

L’élément **assigner** spécifie les personnes auxquelles une tâche est affectée. 
  
```XML
<Assignees>
    <Name></Name>
    <UserID></UserID>
</Assignees>
```

 **EmailUserType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Nom (EmailAddress)](name-emailaddress.md) <br/> |Représente le nom complet de l’utilisateur de boîte aux lettres.  <br/> |
|[UserId (String)](userid-string.md) <br/> |Spécifie l’identificateur d’utilisateur d’un utilisateur de messagerie.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TaskSuggestion](tasksuggestion.md) <br/> |Spécifie une tâche proposée.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

