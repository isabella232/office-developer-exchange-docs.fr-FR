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
description: L’élément ParentItemId identifie l’élément parent qui établit un lien vers une pièce jointe associée.
ms.openlocfilehash: 4f3e33da0af2438948313f0e335cd03e076d135a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465743"
---
# <a name="parentitemid"></a>ParentItemId

L’élément **parentItemId** identifie l’élément parent qui établit un lien vers une pièce jointe associée. 
  
- [CreateAttachment](createattachment.md)
  
- [ParentItemId](parentitemid.md)
  
```xml
<ParentItemId Id="" ChangeKey="" />
```

**ItemIdType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Id** <br/> |Identifie un élément unique dans la Banque d’aide Exchange à associer à une pièce jointe. Cette valeur est une chaîne. Cet attribut est obligatoire.  <br/> |
|**ChangeKey** <br/> |Identifie une version non spécifiée d’un élément qui est identifié par l’attribut **ID** dans la Banque d’aide Exchange. Cela permet de s’assurer qu’un élément actif est utilisé lorsqu’il est mis à jour avec une pièce jointe. Cette valeur est une chaîne. Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |Définit une demande de création d’une pièce jointe à un élément dans une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est requis dans l' [opération CreateAttachment](createattachment-operation.md). Cet élément est fondamentalement le même que l’élément [ItemId](itemid.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |[https://schemas.microsoft.com/exchange/services/2006/messages](https://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération CreateAttachment](createattachment-operation.md)

