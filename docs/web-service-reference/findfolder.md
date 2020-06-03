---
title: FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: b8a59740-d978-454c-9629-a10792385ba0
description: L’élément FindFolder définit une demande de recherche de dossiers dans une boîte aux lettres.
ms.openlocfilehash: 248047206a661afe723543e52c51b57847148423
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462576"
---
# <a name="findfolder"></a>FindFolder

L’élément **FindFolder** définit une demande de recherche de dossiers dans une boîte aux lettres. 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <FractionalPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

**FindFolderType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Traversée  <br/> |Définit le mode d’exécution d’une recherche. Cet attribut est obligatoire.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valeurs d’attribut transversal

|**Valeur**|**Description**|
|:-----|:-----|
|Partielle  <br/> |Indique à l’opération FindFolder de rechercher uniquement le dossier identifié et de renvoyer uniquement les ID de dossier pour les éléments qui n’ont pas été supprimés. Il s’agit d’un parcours superficiel.  <br/> |
|Développée  <br/> |Indique à l’opération FindFolder d’effectuer une recherche dans tous les dossiers enfants du dossier parent identifié et de renvoyer uniquement les ID de dossier pour les éléments qui n’ont pas été supprimés. Il s’agit d’un parcours approfondi.  <br/> |
|SoftDeleted  <br/> |Indique à l’opération FindFolder d’effectuer une recherche de parcours superficiel pour les éléments supprimés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Identifie les propriétés de dossier à inclure dans une réponse FindFolder.  <br/> |
|[IndexedPageFolderView](indexedpagefolderview.md) <br/> |Décrit comment les informations d’élément paginé sont renvoyées dans une réponse FindFolder. Cet élément est facultatif.  <br/> |
|[FractionalPageFolderView](fractionalpagefolderview.md) <br/> |Décrit l’emplacement où l’affichage paginé démarre et le nombre maximal de dossiers renvoyés dans une demande FindFolder. Cet élément est facultatif.  <br/> |
|[Restriction](restriction.md) <br/> |Définit une restriction ou une requête utilisée pour filtrer les dossiers dans une opération FindFolder. Cet élément est facultatif.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifie les dossiers pour l’opération FindFolder à rechercher.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple de requête FindFolder suivant montre comment créer une requête pour rechercher tous les dossiers situés dans une boîte de réception.
  
```xml
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

