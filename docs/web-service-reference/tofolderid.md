---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: L’élément ToFolderId représente le dossier de destination pour un dossier ou un élément copié ou déplacé.
ms.openlocfilehash: a48309f0b7f5c9bf667fc2eb653a0502832bc996
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838734"
---
# <a name="tofolderid"></a>ToFolderId

L’élément **ToFolderId** représente le dossier de destination pour un dossier ou un élément copié ou déplacé. 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

 **TargetFolderIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient l’identificateur d’un dossier de destination pour un dossier ou un élément copié ou déplacé.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie un dossier nommé pour un dossier ou un élément copié ou déplacé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MoveFolder](movefolder.md) <br/> |Définit une demande de déplacement d’un dossier dans la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Définit une demande pour copier un dossier dans la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |Définit une demande de déplacement d’un élément dans la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Définit une demande pour copier un élément dans la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération MoveFolder](movefolder-operation.md)
  
[Opération CopyFolder](copyfolder-operation.md)
  
[Opération MoveItem](moveitem-operation.md)
  
[Opération CopyItem](copyitem-operation.md)

