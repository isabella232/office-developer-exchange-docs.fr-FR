---
title: ParentItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentItemId
api_type:
- schema
ms.assetid: 72dc4391-72db-44d2-85d9-4718d59886a7
description: L’élément ParentItemId identifie l’élément parent qui est lié à une pièce jointe associée.
ms.openlocfilehash: d8072e86d8bd989d4baf6b0f29385dc955b83de8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515361"
---
# <a name="parentitemid"></a>ParentItemId

**L’élément ParentItemId** identifie l’élément parent qui est lié à une pièce jointe associée. 
  
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
|**Id** <br/> |Identifie un seul élément dans la Exchange à associer à une pièce jointe. Cette valeur est une chaîne. Cet attribut est obligatoire.  <br/> |
|**ChangeKey** <br/> |Identifie une version non spécifiée d’un élément identifié par **l’attribut ID** dans la Exchange store. Cela est utilisé pour s’assurer qu’un élément actuel est utilisé lorsqu’il est mis à jour avec une pièce jointe. Cette valeur est une chaîne. Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateAttachment](createattachment.md) <br/> |Définit une demande de création d’une pièce jointe à un élément dans une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/CreateAttachment` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est requis dans [l’opération CreateAttachment](createattachment-operation.md). Cet élément est fondamentalement identique à [l’élément ItemId.](itemid.md) 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |[https://schemas.microsoft.com/exchange/services/2006/messages](https://schemas.microsoft.com/exchange/services/2006/messages) <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération CreateAttachment](createattachment-operation.md)

