---
title: FolderChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderChange
api_type:
- schema
ms.assetid: 23279750-131b-4e1a-b7d1-be235c4e0891
description: L’élément FolderChange représente une collection des modifications à effectuer sur un seul dossier.
ms.openlocfilehash: 3f8b42ff4ac88eaef53d1d4ec1d61212bc14b8c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756447"
---
# <a name="folderchange"></a>FolderChange

L’élément **FolderChange** représente une collection des modifications à effectuer sur un seul dossier. 
  
[UpdateFolder](updatefolder.md)
  
[FolderChanges](folderchanges.md)
  
[FolderChange](folderchange.md)
  
```xml
<FolderChange>
   <FolderId/>
   <Updates/>
</FolderChange>
```

 **FolderChangeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient la clé d’identificateur et de modification d’un dossier à mettre à jour.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie les dossiers MicrosoftExchange Server 2007 qui peuvent être référencés par son nom.  <br/> |
|[Mises à jour (dossier)](updates-folder.md) <br/> |Définit le type de mise à jour est effectuée sur un dossier identifié par [l’ID FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) élément.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FolderChanges](folderchanges.md) <br/> |Représente une collection des modifications pour un dossier.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération UpdateFolder](updatefolder-operation.md)

