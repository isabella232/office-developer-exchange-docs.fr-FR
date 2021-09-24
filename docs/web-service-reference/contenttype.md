---
title: ContentType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ContentType
api_type:
- schema
ms.assetid: f91ff0df-0d8a-43ea-a188-d80f0e885f19
description: L’élément ContentType décrit le type MIME (Multipurpose Internet Mail Extensions) du contenu de la pièce jointe.
ms.openlocfilehash: 3f00aaa2f3b93ab7a8a3ccc4905b1353dce6b083
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526650"
---
# <a name="contenttype"></a>ContentType

**L’élément ContentType** décrit le type MIME (Multipurpose Internet Mail Extensions) du contenu de la pièce jointe. 
  
```xml
<ContentType/>
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

La valeur de texte est une valeur de chaîne qui représente le type de contenu de la pièce jointe.
  
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

