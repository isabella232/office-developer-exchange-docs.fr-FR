---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: L’élément ArchiveTag spécifie l’identificateur de rétention de la balise d’archivage définie sur un élément ou un dossier.
ms.openlocfilehash: c3545b505dc0596d7465154e0be7d6c758b24ec9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525238"
---
# <a name="archivetag"></a>ArchiveTag

**L’élément ArchiveTag** spécifie l’identificateur de rétention de la balise d’archivage définie sur un élément ou un dossier. 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**IsExplicit** <br/> |Spécifie si la stratégie de rétention est explicitement définie sur un élément ou un dossier ou si elle est héritée d’un dossier parent.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier qui contient principalement des éléments de calendrier.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact dans la banque d'informations Exchange.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier de contacts contenu dans une boîte aux lettres.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Folder](folder.md) <br/> |Définit un dossier à créer, obtenir, rechercher, synchroniser ou mettre à jour.  <br/> |
|[Élément](item.md) <br/> |Représente un élément générique dans le magasin Exchange de données.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message Exchange Microsoft.  <br/> |
|[PostItem](postitem.md) <br/> |Représente un élément de publication dans la Exchange store.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche contenu dans une boîte aux lettres.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Représente un dossier de tâches contenu dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément ArchiveTag** est un GUID qui identifie la stratégie de rétention. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

