---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: L’élément ParentItemId identifie l’élément parent qui lie à une pièce jointe associée.
ms.openlocfilehash: 9bd875ee5ead8b87996288a640e1bb14e3a5e8b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828703"
---
# <a name="parentitemid"></a>ParentItemId

L’élément **ParentItemId** identifie l’élément parent qui lie à une pièce jointe associée. 
  
- [CreateAttachment](createattachment.md)
  
- [ParentItemId](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

**ItemIdType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|
  **Id** <br/> |Identifie un seul élément dans la banque d’informations Exchange à associer à une pièce jointe. Cette valeur est une chaîne. Cet attribut est requis.  <br/> |
|**ChangeKey** <br/> |Identifie une version non spécifiée d’un élément identifié par l’attribut **Id** de la banque d’informations Exchange. Cela permet de vous assurer qu’un élément en cours est utilisé lorsqu’il est mis à jour avec une pièce jointe. Cette valeur est une chaîne. Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |Définit une demande pour créer une pièce jointe à un élément dans une boîte aux lettres.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est requis dans l' [opération CreateAttachment](createattachment-operation.md). Cet élément est identique à l’élément [ItemId](itemid.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |[http://schemas.microsoft.com/exchange/services/2006/messages](http://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération CreateAttachment](createattachment-operation.md)

