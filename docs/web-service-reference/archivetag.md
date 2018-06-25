---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: L’élément ArchiveTag Spécifie l’identificateur de rétention de la balise archive définie sur un élément ou un dossier.
ms.openlocfilehash: ae9c7d512981af3bf564bcb73a9a27c5c78217fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755319"
---
# <a name="archivetag"></a>ArchiveTag

L’élément **ArchiveTag** Spécifie l’identificateur de rétention de la balise archive définie sur un élément ou un dossier. 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**IsExplicit** <br/> |Spécifie si la stratégie de rétention est définie sur un élément ou d’un dossier ou si elle est héritée d’un dossier parent.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier contenant principalement des éléments de calendrier.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact dans la banque d'informations Exchange.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier de contacts qui se trouve dans une boîte aux lettres.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Folder](folder.md) <br/> |Définit un dossier pour créer, obtenir, recherchez, synchroniser ou mettre à jour.  <br/> |
|[Item](item.md) <br/> |Représente un élément générique dans la banque d’informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique de Microsoft Exchange.  <br/> |
|[Objet postItem](postitem.md) <br/> |Représente un élément de publication dans la banque d’informations Exchange.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche qui se trouve dans une boîte aux lettres.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
|[Dossier tâches](tasksfolder.md) <br/> |Représente un dossier de tâches qui se trouve dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **ArchiveTag** est un GUID qui identifie la stratégie de rétention. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

