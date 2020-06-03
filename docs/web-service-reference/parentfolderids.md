---
title: ParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderIds
api_type:
- schema
ms.assetid: e7998023-e5e0-465c-91fa-2aa6d1559f64
description: L’élément ParentFolderIds identifie les dossiers pour les opérations FindItem et FindFolder à rechercher.
ms.openlocfilehash: 6bc4b9cfe96c6c83cbeb623ec176e33177356bbc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465428"
---
# <a name="parentfolderids"></a>ParentFolderIds

L’élément **ParentFolderIds** identifie les dossiers pour les opérations FindItem et FindFolder à rechercher. 
  
```xml
<ParentFolderIds>
   <DistinguishedFolderId/>
<ParentFolderIds>
```

```xml
<ParentFolderIds>
   <FolderId/> 
<ParentFolderIds>
```

**NonEmptyArrayOfBaseFolderIdsType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient l’identificateur et la clé de modification d’un dossier. L’élément **ParentFolderIds** doit utiliser cet élément ou l’élément [DistinguishedFolderId](distinguishedfolderid.md) .  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie les dossiers Microsoft Exchange Server 2007 qui peuvent être référencés par leur nom. L’élément **ParentFolderIds** doit utiliser cet élément ou l’élément [FolderId](folderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Définit une demande pour identifier les dossiers d’une boîte aux lettres.  <br/> |
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher des éléments dans une boîte aux lettres.  <br/> |
|[ResolveNames](resolvenames.md) <br/> |Définit une demande de résolution de noms ambigus.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **ParentFolderIds** doit utiliser l’élément [FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) . Un nombre illimité de dossiers peut être défini pour la recherche. 
  
## <a name="example"></a>Exemple

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération FindFolder](findfolder-operation.md)  
- [Opération FindItem](finditem-operation.md) 
- [Opération ResolveNames](resolvenames-operation.md)

