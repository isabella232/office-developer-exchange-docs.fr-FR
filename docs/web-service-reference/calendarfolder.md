---
title: CalendarFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarFolder
api_type:
- schema
ms.assetid: 48687a78-e757-4c04-9641-bf4302c6b565
description: L’élément CalendarFolder représente un dossier contenant principalement des éléments de calendrier.
ms.openlocfilehash: 7dc90706eb45eb4617a68b9fdcf37669921af966
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755467"
---
# <a name="calendarfolder"></a>CalendarFolder

L’élément **CalendarFolder** représente un dossier contenant principalement des éléments de calendrier. 
  
```xml
<CalendarFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <EffectiveRights/>
   <SharingEffectiveRights/>
   <PermissionSet/>
</CalendarFolder>
```

 **CalendarFolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient la clé d’identificateur et de modification d’un dossier.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Représente l’identificateur du dossier qui contient le dossier parent.  <br/> |
|[Classe FolderClass](folderclass.md) <br/> |Représente la classe de dossier pour un dossier donné.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Contient le nom complet d’un dossier.  <br/> |
|[TotalCount](totalcount.md) <br/> |Représente le nombre total d’éléments dans un dossier donné.  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |Représente le nombre de dossiers enfants qui sont contenues dans un dossier. Cette propriété est en lecture seule.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés étendues dans les dossiers.  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contient des informations sur un dossier géré.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.  <br/> |
|[SharingEffectiveRights (CalendarPermissionReadAccessType)](sharingeffectiverights-calendarpermissionreadaccesstype.md) <br/> |Indique les autorisations dont dispose l’utilisateur pour les données de calendrier qui sont partagées.  <br/> |
|[PermissionSet (CalendarPermissionSetType)](permissionset-calendarpermissionsettype.md) <br/> |Contient toutes les autorisations configurées pour un dossier de calendrier.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[Créer (FolderSync)](create-foldersync.md) <br/> |Identifie un dossier unique à créer dans le magasin de client local.  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Représente une mise à jour d’une propriété donnée sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[Mise à jour (FolderSync)](update-foldersync.md) <br/> |Identifie un seul dossier pour mettre à jour dans le magasin de client local.  <br/> |
|[Dossiers](folders-ex15websvcsotherref.md) <br/> |Contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.  <br/> |
   
## <a name="remarks"></a>Remarques

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

