---
title: MoveToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MoveToFolder
api_type:
- schema
ms.assetid: 991673b9-b627-4848-bfba-59a187b8575f
description: L’élément MoveToFolder spécifie l’identificateur du dossier vers lequel les éléments de courrier électronique peuvent être déplacés.
ms.openlocfilehash: 811184da8ba3513e94950b44cff15953f690cf70
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515529"
---
# <a name="movetofolder"></a>MoveToFolder

**L’élément MoveToFolder** spécifie l’identificateur du dossier vers lequel les éléments de courrier électronique peuvent être déplacés. 
  
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
|[FolderId](folderid.md) <br/> |Contient l’identificateur d’un dossier de destination pour un élément ou dossier copié ou déplacé.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie un dossier de destination nommé pour un élément ou dossier copié ou déplacé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Actions](actions.md) <br/> |Représente l’ensemble des actions qui peuvent être prises sur un message lorsque les conditions sont remplies.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[CopyToFolder](copytofolder.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

