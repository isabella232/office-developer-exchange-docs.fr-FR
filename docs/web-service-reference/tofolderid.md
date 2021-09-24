---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: L’élément ToFolderId représente le dossier de destination d’un élément ou dossier copié ou déplacé.
ms.openlocfilehash: b58192aa4d1ffe609da78dfdf1b5c86522fc45c8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515165"
---
# <a name="tofolderid"></a>ToFolderId

**L’élément ToFolderId représente** le dossier de destination d’un élément ou dossier copié ou déplacé. 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

```xml
<ToFolderId>
   <DistinguishedFolderId/>
</ToFolderId>
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
|[MoveFolder](movefolder.md) <br/> |Définit une demande de déplacement d’un dossier dans la Exchange store.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Définit une demande de copie d’un dossier dans la Exchange store.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |Définit une demande de déplacement d’un élément dans la Exchange store.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Définit une demande de copie d’un élément dans la Exchange store.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération MoveFolder](movefolder-operation.md)  
- [Opération CopyFolder](copyfolder-operation.md) 
- [Opération MoveItem](moveitem-operation.md) 
- [Opération CopyItem](copyitem-operation.md)

