---
title: Folder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Folder
api_type:
- schema
ms.assetid: 812948d8-c7db-45ce-bb3a-77233a53a974
description: L’élément Folder définit un dossier à créer, obtenir, rechercher, synchroniser ou mettre à jour.
ms.openlocfilehash: 5b6b8eb1d53c84bc3d0484d1c868470137db492d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530380"
---
# <a name="folder"></a>Folder

**L’élément Folder** définit un dossier à créer, obtenir, rechercher, synchroniser ou mettre à jour. 
  
```xml
<Folder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <PermissionSet/>
   <EffectiveRights/>
</Folder>
```

 **FolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient l’identificateur et la clé de modification d’un dossier.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Représente l’identificateur du dossier parent qui contient le dossier.  <br/> |
|[FolderClass](folderclass.md) <br/> |Représente la classe de dossier pour un dossier donné.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Contient le nom complet d’un dossier.  <br/> |
|[TotalCount](totalcount.md) <br/> |Représente le nombre total d’éléments dans un dossier donné.  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |Représente le nombre de dossiers enfants contenus dans un dossier. Cette propriété est en lecture seule.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés étendues sur les dossiers.  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contient des informations sur un dossier géré.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Représente le nombre d’éléments non lus dans un dossier donné.  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Contient toutes les autorisations configurées pour un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Spécifie les données à appendre à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[Create (FolderSync)](create-foldersync.md) <br/> |Identifie un dossier unique à créer dans le magasin de client local.  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Représente une mise à jour d’une propriété unique sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[Update (FolderSync)](update-foldersync.md) <br/> |Identifie un dossier unique à mettre à jour dans le magasin de clients local.  <br/> |
|[Dossiers](folders-ex15websvcsotherref.md) <br/> |Contient un tableau de dossiers utilisés dans les opérations de dossier.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Exchange 2007 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderItems](syncfolderitems-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

