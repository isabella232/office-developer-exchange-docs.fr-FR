---
title: AttachmentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: L’élément AttachmentId identifie un élément ou fichier des pièces jointes. Cet élément est utilisé dans les réponses CreateAttachment.
ms.openlocfilehash: 2910503d1661ca3aaeeb4e319deb39f6b57c5c0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755335"
---
# <a name="attachmentid"></a>AttachmentId

L’élément **AttachmentId** identifie un élément ou fichier des pièces jointes. Cet élément est utilisé dans les réponses CreateAttachment. 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 **AttachmentIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|
  **Id** <br/> |Identifie l’identificateur unique de la pièce jointe.  <br/> |
|**RootItemId** <br/> |Identifie l’identificateur unique de l’élément racine du magasin à laquelle la pièce jointe est associée.  <br/> |
|**RootItemChangeKey** <br/> |Identifie la touche de modification de l’élément racine du magasin à laquelle la pièce jointe est associée.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Représente un élément Exchange qui est joint à un autre élément Exchange.  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Représente un fichier qui est attaché à un élément dans la banque d’informations Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

Il est important de noter que lorsqu’une pièce jointe est créée, la modifier la clé de l’élément racine est modifiée.
  
L’élément [AttachmentId (GetAttachment et DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) est utilisé dans les requêtes DeleteAttachment et GetAttachment. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

