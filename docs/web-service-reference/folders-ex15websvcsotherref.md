---
title: Dossiers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: L’élément dossiers contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.
ms.openlocfilehash: e1b9e337f633dbf6fda159c28725d3fb8dcd55a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756454"
---
# <a name="folders"></a>Dossiers

L’élément **dossiers** contient un tableau des dossiers qui sont utilisés dans les opérations de dossier. 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

 **ArrayOfFoldersType** ou **NonEmptyArrayOfFoldersType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Identifie un dossier pour créer, obtenir, recherchez, synchroniser ou mettre à jour.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier contenant principalement des éléments de calendrier.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier Contacts dans une boîte aux lettres.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche contenu dans une boîte aux lettres.  <br/> |
|[Dossier tâches](tasksfolder.md) <br/> |Représente un dossier de tâches dans une boîte aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération CopyFolder](copyfolder-operation.md) .  <br/> |
|[CreateFolder](createfolder.md) <br/> |Définit une demande pour créer un dossier dans la banque d’informations Exchange.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération CreateFolder](createfolder-operation.md) .  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération CreateManagedFolder](createmanagedfolder-operation.md) .  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération GetFolder](getfolder-operation.md) .  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération MoveFolder](movefolder-operation.md) .  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Identifie le dossier dans lequel un nouveau dossier est créé.  <br/> |
|[RootFolder (FindFolderResponseMessage)](rootfolder-findfolderresponsemessage.md) <br/> |Contient les résultats de recherche dans un dossier racine unique lors d’une [opération FindFolder](findfolder-operation.md).  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande [d’opération UpdateFolder](updatefolder-operation.md) .  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est un élément enfant requis de l’élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)

