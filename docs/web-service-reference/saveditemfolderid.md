---
title: SavedItemFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: L’élément SavedItemFolderId identifie le dossier cible pour les opérations de mise à jour, d’envoi et de création d’éléments dans une boîte aux lettres.
ms.openlocfilehash: 8e18b8863a54aa4e9d6e65f7a54e20904f5a9599
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465274"
---
# <a name="saveditemfolderid"></a>SavedItemFolderId

L’élément **SavedItemFolderId** identifie le dossier cible pour les opérations de mise à jour, d’envoi et de création d’éléments dans une boîte aux lettres. 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

```xml
<SavedItemFolderId>
   <DistinguishedFolderId/>
</SavedItemFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient l’identificateur et la clé de modification d’un dossier cible pour les opérations de mise à jour, d’envoi et de création d’éléments dans la Banque d’Exchange.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie un dossier cible par un identificateur nommé pour les opérations de mise à jour, d’envoi et de création d’éléments dans la Banque d’aide Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Définit une demande de création d’un élément dans la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/CreateItem` <br/> |
|[UpdateItem](updateitem.md) <br/> |Définit une demande de mise à jour d’un élément dans la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/UpdateItem` <br/> |
|[SendItem](senditem.md) <br/> |Définit une demande d’envoi d’un élément dans la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

