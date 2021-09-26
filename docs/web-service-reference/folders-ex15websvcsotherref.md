---
title: Dossiers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: L’élément Folders contient un tableau de dossiers utilisés dans les opérations de dossiers.
ms.openlocfilehash: 77442965c9d372a2895404cf1c919be38e98abb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546433"
---
# <a name="folders"></a>Folders

**L’élément Folders** contient un tableau de dossiers utilisés dans les opérations de dossiers. 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

```xml
<Folders>
   <ContactsFolder/> 
</Folders>
```

```xml
<Folders>
   <TasksFolder/>
</Folders>
```

```xml
<Folders>
   <CalendarFolder/>
</Folders>
```

```xml
<Folders>
   <SearchFolder/> 
</Folders>
```

**ArrayOfFoldersType** ou **NonEmptyArrayOfFoldersType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Identifie un dossier à créer, obtenir, rechercher, synchroniser ou mettre à jour.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier qui contient principalement des éléments de calendrier.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier Contacts dans une boîte aux lettres.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche contenu dans une boîte aux lettres.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Représente un dossier Tâches dans une boîte aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération CopyFolder](copyfolder-operation.md) unique.  <br/> |
|[CreateFolder](createfolder.md) <br/> |Définit une demande de création d’un dossier dans la Exchange store.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération CreateFolder](createfolder-operation.md) unique.  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération CreateManagedFolder](createmanagedfolder-operation.md) unique.  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération GetFolder.](getfolder-operation.md)  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération MoveFolder.](movefolder-operation.md)  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Identifie le dossier dans lequel un nouveau dossier est créé.  <br/> |
|[RootFolder (FindFolderResponseMessage)](rootfolder-findfolderresponsemessage.md) <br/> |Contient les résultats de la recherche d’un dossier racine unique au cours [d’une opération FindFolder](findfolder-operation.md).  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande [d’opération UpdateFolder](updatefolder-operation.md) unique.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est un élément enfant requis de [l’élément ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md) 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)

