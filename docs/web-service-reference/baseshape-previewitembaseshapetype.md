---
title: BaseShape (PreviewItemBaseShapeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7b9e2fdd-5678-4178-9297-7f12a3ca9d64
description: L’élément BaseShape spécifie l’aperçu par défaut avec toutes les propriétés renvoyées ou un aperçu compact avec moins de propriétés renvoyées.
ms.openlocfilehash: b30922a5f8e11200679ffe5aa813d3a0e5f4578e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545691"
---
# <a name="baseshape-previewitembaseshapetype"></a>BaseShape (PreviewItemBaseShapeType)

**L’élément BaseShape spécifie** l’aperçu par défaut avec toutes les propriétés renvoyées ou un aperçu compact avec moins de propriétés renvoyées. 
  
```XML
<BaseShape> Default | Compact</BaseShape>
```

 **PreviewItemBaseShapeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PreviewItemResponseShape](previewitemresponseshape.md) <br/> |Contient la forme de la réponse.  <br/> |
   
## <a name="text-value"></a>Valeur texte

**Valeurs de texte de l’élément BaseShape**

|**Valeur**|**Description**|
|:-----|:-----|
|Par défaut  <br/> |Indique que toutes les propriétés sont affichées.  <br/> |
|Compact  <br/> |Indique que seules les propriétés sélectionnées sont affichées.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

