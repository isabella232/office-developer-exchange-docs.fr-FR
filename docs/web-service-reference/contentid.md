---
title: ContentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ContentId
api_type:
- schema
ms.assetid: bc59100d-6079-414b-a6e0-7c15feaa3184
description: L’élément ContentId représente un identificateur pour le contenu d’une pièce jointe. ContentId peut être définie sur n’importe quelle valeur de chaîne. Les applications peuvent utiliser ContentId pour implémenter leurs propres mécanismes d’identification.
ms.openlocfilehash: 786a76d312e4b8f276a9b5c7082754b873b0061c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519911"
---
# <a name="contentid"></a>ContentId

**L’élément ContentId** représente un identificateur pour le contenu d’une pièce jointe. **ContentId peut** être définie sur n’importe quelle valeur de chaîne. Les applications peuvent utiliser **ContentId** pour implémenter leurs propres mécanismes d’identification. 
  
```xml
<ContentId/>
```

 **String**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemAttachment](itemattachment.md) <br/> |Représente un élément Exchange qui est joint à un autre élément Exchange.  <br/> |
|[FileAttachment](fileattachment.md) <br/> |Représente un fichier joint à un élément dans la Exchange store.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de chaîne représente l’identificateur du contenu d’une pièce jointe.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

