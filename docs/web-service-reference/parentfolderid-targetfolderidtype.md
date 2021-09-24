---
title: ParentFolderId (TargetFolderIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: L’élément ParentFolderId identifie le dossier dans lequel un nouveau dossier est créé ou le dossier à rechercher pour l’opération FindConversation.
ms.openlocfilehash: 53a5721b2c20c211a61b7e71b2e4f636700456b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524622"
---
# <a name="parentfolderid-targetfolderidtype"></a>ParentFolderId (TargetFolderIdType)

**L’élément ParentFolderId** identifie le dossier dans lequel un nouveau dossier est créé ou le dossier à rechercher pour l’opération [FindConversation](findconversation-operation.md).
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

```xml
<ParentFolderId>
   <FolderId/> 
</ParentFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Attributs et éléments

**L’élément ParentFolderId** contient deux éléments enfants. Les éléments enfants s’excluent mutuellement dans le schéma. 
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient l’identificateur requis et la clé de modification facultative d’un dossier dans lequel un nouveau dossier est créé ou le dossier recherché pour l’opération [FindConversation](findconversation-operation.md). L’utilisation de cet élément exclut l’utilisation de [l’élément DistinguishedFolderId.](distinguishedfolderid.md)  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie les dossiers Microsoft Exchange Server 2007 par défaut. L’utilisation de cet élément exclut l’utilisation de [l’élément FolderId.](folderid.md)  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateFolder](createfolder.md) <br/> |Définit une demande de création d’un dossier dans la base de données Exchange données.  <br/> Voici l’expression XPath de cet élément :  `/CreateFolder` <br/> |
|[FindConversation](findconversation.md) <br/> |Définit une demande de recherche de conversations dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Les deux éléments enfants sont utilisés pour définir le dossier qui contiendra le nouveau dossier. Vous devez sélectionner [l’élément FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) pour identifier le dossier parent du nouveau dossier. Vous ne pouvez pas utiliser les deux éléments en même temps. Cet élément est requis pour créer des dossiers. 
  
[L’élément ParentFolderId](parentfolderid.md) décrit l’emplacement des éléments et dossiers existants. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération CreateFolder](createfolder-operation.md)
- [Opération FindConversation](findconversation-operation.md)
- [Création de dossiers (Exchange Web Services)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

