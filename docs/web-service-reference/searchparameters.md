---
title: SearchParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchParameters
api_type:
- schema
ms.assetid: 34602cb1-dc33-4552-a98c-3e77f614daa3
description: L’élément SearchParameters représente les paramètres qui définissent un dossier de recherche.
ms.openlocfilehash: cd9f255621b17d01113392e67a0301b01b70f326
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466667"
---
# <a name="searchparameters"></a>SearchParameters

L’élément **SearchParameters** représente les paramètres qui définissent un dossier de recherche. 
  
```xml
<SearchParameters Traversal="">
   <Restriction/>
   <BaseFolderIds/>
</SearchParameters>
```

 **SearchParametersType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Traversée** <br/> |Décrit comment un dossier de recherche parcourt la hiérarchie de dossiers. Les options sont pour une recherche **approfondie** ou **superficielle** .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Représente la collection de dossiers qui seront extraites pour déterminer le contenu d’un dossier de recherche.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche contenu dans une boîte aux lettres.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

