---
title: Dossier tâches
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolder
api_type:
- schema
ms.assetid: 5a9a4612-8064-4986-b467-c44f268c64df
description: L’élément du dossier tâches représente un dossier de tâches qui se trouve dans une boîte aux lettres.
ms.openlocfilehash: b2151c68519a6ff15fbc74b48fc93a7e06af9e76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838674"
---
# <a name="tasksfolder"></a>Dossier tâches

L’élément du **dossier tâches** représente un dossier de tâches qui se trouve dans une boîte aux lettres. 
  
```xml
<TasksFolder>
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
</TasksFolder>
```

**TasksFolderType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient la clé d’identificateur et de modification d’un dossier tâches.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Représente l’identificateur du dossier parent qui contient le dossier tâches.  <br/> |
|[Classe FolderClass](folderclass.md) <br/> |Représente la classe de dossier pour un dossier tâches.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Contient le nom complet d’un dossier tâches.  <br/> |
|[TotalCount](totalcount.md) <br/> |Représente le nombre total d’éléments dans un dossier tâches.  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |Représente le nombre de dossiers enfants qui sont contenues dans un dossier tâches. Cette propriété est en lecture seule.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés étendues sur un dossier tâches.  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Contient des informations sur un dossier géré.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Représente le nombre d’éléments non lus dans un dossier tâches.  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Contient toutes les autorisations configurées pour un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule. Cet élément a été introduit dans Microsoft Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Spécifie les données à ajouter à une propriété de dossier lors d’une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[Créer (FolderSync)](create-foldersync.md) <br/> |Identifie un dossier unique à créer dans le magasin de client local.  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Représente une mise à jour d’une propriété donnée sur un dossier dans une [opération UpdateFolder](updatefolder-operation.md).  <br/> |
|[Mise à jour (FolderSync)](update-foldersync.md) <br/> |Identifie un seul dossier pour mettre à jour dans le magasin de client local.  <br/> |
|[Dossiers](folders-ex15websvcsotherref.md) <br/> |Contient un tableau des dossiers qui sont utilisés dans les opérations de dossier.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

