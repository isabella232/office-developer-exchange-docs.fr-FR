---
title: Modifications (hiérarchie)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: 918a0d1f-90a5-4eef-9592-07e15bef94e6
description: L’élément de modifications contient un tableau de types de modification qui représente le type des différences entre les dossiers sur le client et les dossiers sur l’ordinateur qui exécute Microsoft Exchange Server 2007 séquencé.
ms.openlocfilehash: 15e4f9f37c5e4a4083260dcf379a49beb2260030
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755507"
---
# <a name="changes-hierarchy"></a>Modifications (hiérarchie)

L’élément de **modifications** contient un tableau de types de modification qui représente le type des différences entre les dossiers sur le client et les dossiers sur l’ordinateur qui exécute Microsoft Exchange Server 2007 séquencé. 
  
[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
  
[Modifications (hiérarchie)](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 **SyncFolderHierarchyChangesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Créer (FolderSync)](create-foldersync.md) <br/> |Identifie un dossier unique à créer dans le magasin de client local.  <br/> |
|[Mise à jour (FolderSync)](update-foldersync.md) <br/> |Identifie un seul dossier pour mettre à jour dans le magasin de client local.  <br/> |
|[Supprimer (FolderSync)](delete-foldersync.md) <br/> |Identifie un seul dossier à supprimer dans le magasin de client local.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande SyncFolderHierarchy.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente une valeur Boolean est requise.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur Exchange 2007 ayant le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderHierarchy](syncfolderhierarchy-operation.md)


[Référence EWS pour Exchange](ews-reference-for-exchange.md)
  
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

