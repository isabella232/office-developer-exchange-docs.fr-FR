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
description: L’élément Folders contient un tableau de dossiers utilisés dans les opérations de dossier.
ms.openlocfilehash: b087be0501f04390b80458458e7e7ccc24bf27bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530978"
---
# <a name="folders"></a>Folders

L’élément **Folders** contient un tableau de dossiers utilisés dans les opérations de dossier. 
  
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
|[Folder](folder.md) <br/> |Identifie un dossier à créer, obtenir, Rechercher, synchroniser ou mettre à jour.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier qui contient principalement des éléments de calendrier.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier de contacts dans une boîte aux lettres.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche contenu dans une boîte aux lettres.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Représente un dossier tâches dans une boîte aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération CopyFolder](copyfolder-operation.md) .  <br/> |
|[CreateFolder](createfolder.md) <br/> |Définit une demande de création d’un dossier dans la Banque d’Exchange.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération CreateFolder](createfolder-operation.md) .  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération CreateManagedFolder](createmanagedfolder-operation.md) .  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération GetFolder](getfolder-operation.md) .  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération MoveFolder](movefolder-operation.md) .  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Identifie le dossier dans lequel un nouveau dossier est créé.  <br/> |
|[RootFolder (FindFolderResponseMessage)](rootfolder-findfolderresponsemessage.md) <br/> |Contient les résultats de la recherche dans un dossier racine unique pendant une [opération FindFolder](findfolder-operation.md).  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une seule demande d' [opération UpdateFolder](updatefolder-operation.md) .  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est un élément enfant obligatoire de l’élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)

