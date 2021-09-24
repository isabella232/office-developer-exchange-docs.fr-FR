---
title: BaseFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- BaseFolderIds
api_type:
- schema
ms.assetid: bdaa6093-f960-469a-b338-0e75aaa536c6
description: L’élément BaseFolderIds représente la collection de dossiers qui seront extraits pour déterminer le contenu d’un dossier de recherche.
ms.openlocfilehash: 3a108e6215c6a444117aa65c756352b9800f6948
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518945"
---
# <a name="basefolderids"></a>BaseFolderIds

**L’élément BaseFolderIds** représente la collection de dossiers qui seront extraits pour déterminer le contenu d’un dossier de recherche. 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient l’identificateur et la clé de modification d’un dossier.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie les dossiers MicrosoftExchange Server 2007 qui peuvent être référencés par leur nom.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SearchParameters](searchparameters.md) <br/> |Représente les paramètres qui définissent un dossier de recherche.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément BaseFolderIds doit** contenir au moins un [élément FolderId](folderid.md) ou [DistinguishedFolderId.](distinguishedfolderid.md) 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Exchange Server 2007 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

