---
title: Modifications (hiérarchie)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Changes
api_type:
- schema
ms.assetid: 918a0d1f-90a5-4eef-9592-07e15bef94e6
description: L’élément Changes contient un tableau séquentif de types de modifications qui représentent le type de différences entre les dossiers sur le client et les dossiers sur l’ordinateur qui exécute Microsoft Exchange Server 2007.
ms.openlocfilehash: 1ecb43e37258ad5d8e12619436f14992cc2f788b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512120"
---
# <a name="changes-hierarchy"></a>Modifications (hiérarchie)

L’élément **Changes** contient un tableau séquenquent des types de modifications qui représentent le type de différences entre les dossiers sur le client et les dossiers sur l’ordinateur qui exécute Microsoft Exchange Server 2007. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Create (FolderSync)](create-foldersync.md) <br/> |Identifie un dossier unique à créer dans le magasin de client local.  <br/> |
|[Update (FolderSync)](update-foldersync.md) <br/> |Identifie un dossier unique à mettre à jour dans le magasin de clients local.  <br/> |
|[Delete (FolderSync)](delete-foldersync.md) <br/> |Identifie un dossier unique à supprimer dans le magasin de clients local.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande SyncFolderHierarchy.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une valeur Boolean est requise.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur Exchange 2007 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderHierarchy](syncfolderhierarchy-operation.md)


[Référence EWS pour Exchange](ews-reference-for-exchange.md)
  
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

