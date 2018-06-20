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
description: L’élément FindFolder définit une requête pour rechercher les dossiers dans une boîte aux lettres.
ms.openlocfilehash: d41283547c443e38e2e87379a7224df9c89f901d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756385"
---
# <a name="findfolder"></a>FindFolder

L’élément **FindFolder** définit une requête pour rechercher les dossiers dans une boîte aux lettres. 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

 **FindFolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Traversée du contenu  <br/> |Définit la façon dont une recherche est effectuée. Cet attribut est requis.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valeurs d’attribut Traversal

|**Valeur**|**Description**|
|:-----|:-----|
|Peu profond  <br/> |Indique à l’opération FindFolder recherche uniquement le dossier identifié et renvoyer uniquement l’ID de dossier pour les éléments qui n’ont pas été supprimés. Il s’agit d’un parcours en surface.  <br/> |
|Profond  <br/> |Indique à l’opération FindFolder pour la recherche dans tous les dossiers enfants du dossier parent identifié et renvoyer uniquement l’ID de dossier pour les éléments qui n’ont pas été supprimés. Il s’agit d’une longue traversée.  <br/> |
|SoftDeleted  <br/> |Indique à l’opération FindFolder pour effectuer une recherche parcours en surface des éléments supprimés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Identifie les propriétés du dossier à inclure dans une réponse FindFolder.  <br/> |
|[IndexedPageFolderView](indexedpagefolderview.md) <br/> |Décrit comment paginé informations sont retournées dans une réponse FindFolder. Cet élément est facultatif.  <br/> |
|[FractionalPageFolderView](fractionalpagefolderview.md) <br/> |Décrit où l’affichage paginé démarre et le nombre maximal de dossiers renvoyées dans une requête FindFolder. Cet élément est facultatif.  <br/> |
|[Restriction](restriction.md) <br/> |Définit une restriction ou une requête qui est utilisé pour filtrer les dossiers dans une opération FindFolder. Cet élément est facultatif.  <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Identifie les dossiers pour l’opération FindFolder à rechercher.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant d’une demande FindFolder indique comment former une requête pour rechercher tous les dossiers situés dans une boîte de réception.
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindFolder](findfolder-operation.md)

