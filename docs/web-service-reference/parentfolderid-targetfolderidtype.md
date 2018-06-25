---
title: ParentFolderId (TargetFolderIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: L’élément ParentFolderId identifie le dossier dans lequel un nouveau dossier est créé ou du dossier de recherche pour l’opération FindConversation.
ms.openlocfilehash: 61072e1dd3321beb5f3b76d9accf20530b443796
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828686"
---
# <a name="parentfolderid-targetfolderidtype"></a>ParentFolderId (TargetFolderIdType)

L’élément **ParentFolderId** identifie le dossier dans lequel un nouveau dossier est créé ou du dossier de recherche pour l' [opération FindConversation](findconversation-operation.md).
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Attributs et éléments

L’élément **ParentFolderId** contient deux éléments enfants. Les éléments enfants s’excluent mutuellement dans le schéma. 
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient l’identificateur et la clé de changement facultatif d’un dossier dans lequel un nouveau dossier est créé ou le dossier est recherché dans l' [opération FindConversation](findconversation-operation.md). À l’aide de cet élément exclut l’utilisation de l’élément [DistinguishedFolderId](distinguishedfolderid.md) .  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie les dossiers de Microsoft Exchange Server 2007 par défaut. À l’aide de cet élément exclut l’utilisation de l’élément [FolderId](folderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateFolder](createfolder.md) <br/> |Définit une demande pour créer un dossier dans la base de données Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :`/CreateFolder` <br/> |
|[FindConversation](findconversation.md) <br/> |Définit une requête pour rechercher les conversations dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Les deux éléments enfants sont utilisés pour définir le dossier qui contiendra le nouveau dossier. Vous devez sélectionner le [FolderId](folderid.md) ou l’élément [DistinguishedFolderId](distinguishedfolderid.md) pour identifier le dossier parent du nouveau dossier. Vous ne pouvez pas utiliser les deux éléments en même temps. Cet élément est nécessaire pour créer des dossiers. 
  
L’élément [ParentFolderId](parentfolderid.md) décrit l’emplacement des éléments et dossiers existants. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération CreateFolder](createfolder-operation.md)
- [FindConversation Operation](findconversation-operation.md)
- [Création de dossiers (Exchange Web Services)](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

