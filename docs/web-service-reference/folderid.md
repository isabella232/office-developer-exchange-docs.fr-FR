---
title: FolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderId
api_type:
- schema
ms.assetid: 00d14e3e-4365-4f21-8f88-eaeea73b9bf7
description: L’élément FolderId contient la clé d’identificateur et de modification d’un dossier.
ms.openlocfilehash: 5764a164d5af183b8f313955ace5274dc6023a6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756451"
---
# <a name="folderid"></a>FolderId

L’élément **FolderId** contient la clé d’identificateur et de modification d’un dossier. 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |Contient une chaîne qui identifie un dossier dans la banque d’informations Exchange. Cet attribut est requis.  <br/> |
|ChangeKey  <br/> |Contient une chaîne qui identifie une version d’un dossier qui est identifié par l’attribut Id. Cet attribut est facultatif. Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Indique le dossier qui est ciblé pour les actions qui utilisent des dossiers.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Représente un événement dans lequel un élément ou un dossier est copié.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indique le dossier de destination de copie et les actions de déplacement.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Identifie le dossier dans lequel un nouveau dossier ou un élément est créé.  <br/><br/>  Les expressions XPath pour cet élément sont les suivantes :<br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Représente la collection de dossiers qui seront être interrogées pour déterminer le contenu d’un dossier de recherche.  <br/> |
|[Supprimer (FolderSync)](delete-foldersync.md) <br/> |Identifie un seul dossier à supprimer dans le magasin de client local.  <br/> |
|[Folder](folder.md) <br/> |Représente un dossier dans une boîte aux lettres.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier de calendrier dans une boîte aux lettres.  <br/> |
|[FolderChange](folderchange.md) <br/> |Représente une collection des modifications à effectuer sur un seul dossier.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :`/UpdateFolder/FolderChanges/FolderChange` <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier de contacts dans une boîte aux lettres.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche dans une boîte aux lettres.  <br/> |
|[Dossier tâches](tasksfolder.md) <br/> |Représente un dossier de tâches dans une boîte aux lettres.  <br/> |
|[ToFolderId](tofolderid.md) <br/> | Représente le dossier de destination pour un dossier ou un élément copié ou déplacé. <br/> <br/>  Les expressions XPath pour cet élément sont les suivantes : <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.  <br/><br/>  Les expressions XPath pour cet élément sont les suivantes : <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Représente le dossier qui contient les éléments à synchroniser.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Représente le nom d’un objet de configuration utilisateur. Le nom d’objet de configuration utilisateur est l’identificateur pour un objet de configuration utilisateur.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Identifie l’ID du dossier qui sont copiées dans les éléments de courrier électronique.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Identifie l’ID du dossier qui seront déplacées vers des éléments de courrier électronique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Tous les éléments **FolderId** sont du type **FolderIdType** . L’élément **FolderId** est requis dans chaque cas, à l’exception des éléments dont le type étend la **BaseFolderType** ou où l’élément **FolderId** fait partie d’un choix. Passez en revue le schéma pour plus d’informations. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Création de dossiers (Exchange Web Services)](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

