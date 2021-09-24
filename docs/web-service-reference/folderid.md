---
title: FolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderId
api_type:
- schema
ms.assetid: 00d14e3e-4365-4f21-8f88-eaeea73b9bf7
description: L’élément FolderId contient l’identificateur et la clé de modification d’un dossier.
ms.openlocfilehash: 7348fb7342bf33d487591a9daf93a9570f7552f4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513681"
---
# <a name="folderid"></a>FolderId

**L’élément FolderId** contient l’identificateur et la clé de modification d’un dossier. 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |Contient une chaîne qui identifie un dossier dans la Exchange store. Cet attribut est obligatoire.  <br/> |
|ChangeKey  <br/> |Contient une chaîne qui identifie une version d’un dossier identifiée par l’attribut ID. Cet attribut est facultatif. Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indique le dossier ciblé pour les actions qui utilisent des dossiers.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est copié.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indique le dossier de destination pour les actions de copie et de déplacement.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Identifie le dossier dans lequel un dossier ou un nouvel élément est créé.  <br/><br/>  Les expressions XPath de cet élément sont les suivantes :<br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Représente la collection de dossiers qui seront extraits pour déterminer le contenu d’un dossier de recherche.  <br/> |
|[Delete (FolderSync)](delete-foldersync.md) <br/> |Identifie un dossier unique à supprimer dans le magasin de clients local.  <br/> |
|[Folder](folder.md) <br/> |Représente un dossier dans une boîte aux lettres.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier de calendrier dans une boîte aux lettres.  <br/> |
|[FolderChange](folderchange.md) <br/> |Représente une collection de modifications à effectuer sur un seul dossier.  <br/> Voici l’expression XPath de cet élément :  `/UpdateFolder/FolderChanges/FolderChange` <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier de contacts dans une boîte aux lettres.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche dans une boîte aux lettres.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Représente un dossier de tâches dans une boîte aux lettres.  <br/> |
|[ToFolderId](tofolderid.md) <br/> | Représente le dossier de destination d’un élément ou dossier copié ou déplacé. <br/> <br/>  Les expressions XPath de cet élément sont les suivantes : <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Identifie le dossier cible pour les opérations de mise à jour, d’envoi et de création d’éléments dans Exchange store.  <br/><br/>  Les expressions XPath de cet élément sont les suivantes : <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Représente le dossier qui contient les éléments à synchroniser.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Représente le nom d’un objet de configuration utilisateur. Le nom de l’objet de configuration utilisateur est l’identificateur d’un objet de configuration utilisateur.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Identifie l’ID du dossier dans qui les éléments de messagerie seront copiés.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Identifie l’ID du dossier vers qui les éléments de messagerie seront déplacés.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Tous **les éléments FolderId** sont de type **FolderIdType.** **L’élément FolderId** est requis dans tous les cas sauf dans les éléments dont le type étend **baseFolderType** ou où l’élément **FolderId** fait partie d’un choix. Pour plus d’informations, examinez le schéma. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Création de dossiers (Exchange Web Services)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

