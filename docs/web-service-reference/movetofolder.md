---
title: MoveToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveToFolder
api_type:
- schema
ms.assetid: 991673b9-b627-4848-bfba-59a187b8575f
description: L’élément MoveToFolder spécifie l’identificateur du dossier vers lequel les éléments de courrier électronique peuvent être déplacés.
ms.openlocfilehash: e323b2ac5390855b3db0b5495af667cdf2da5596
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530005"
---
# <a name="movetofolder"></a>MoveToFolder

L’élément **MoveToFolder** spécifie l’identificateur du dossier vers lequel les éléments de courrier électronique peuvent être déplacés. 
  
```XML
<MoveToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</MoveToFolder>
```

 **TargetFolderIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient l’identificateur d’un dossier de destination pour un élément ou un dossier copié ou déplacé.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie un dossier de destination nommé pour un élément ou un dossier copié ou déplacé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Actions](actions.md) <br/> |Représente l’ensemble des actions pouvant être effectuées sur un message lorsque les conditions sont remplies..  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[CopyToFolder](copytofolder.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

