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
description: L’élément SavedItemFolderId identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans une boîte aux lettres.
ms.openlocfilehash: 3f46070a538f5e03007925565a8888efe06b62b7
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354161"
---
# <a name="saveditemfolderid"></a>SavedItemFolderId

L’élément **SavedItemFolderId** identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans une boîte aux lettres. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient la clé d’identificateur et de modification d’un dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie un dossier cible par un identificateur nommé pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Définit une demande pour créer un élément dans la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/CreateItem` <br/> |
|[UpdateItem](updateitem.md) <br/> |Définit une demande de mise à jour d’un élément dans la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/UpdateItem` <br/> |
|[SendItem](senditem.md) <br/> |Définit une demande d’envoi d’un élément dans la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

