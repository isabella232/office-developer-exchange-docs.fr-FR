---
title: BaseShape (PreviewItemBaseShapeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b9e2fdd-5678-4178-9297-7f12a3ca9d64
description: L’élément BaseShape Spécifie l’aperçu avec toutes les propriétés renvoyées par défaut ou un aperçu compact avec moins de propriétés retournés.
ms.openlocfilehash: 1f060ae9adf52cc2916a634e3d954e3fc0903941
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755375"
---
# <a name="baseshape-previewitembaseshapetype"></a>BaseShape (PreviewItemBaseShapeType)

L’élément **BaseShape** Spécifie l’aperçu avec toutes les propriétés renvoyées par défaut ou un aperçu compact avec moins de propriétés retournés. 
  
```XML
<BaseShape> Default | Compact</BaseShape>
```

 **PreviewItemBaseShapeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PreviewItemResponseShape](previewitemresponseshape.md) <br/> |Contient la forme de la réponse.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

**Valeurs de texte des éléments BaseShape**

|**Valeur**|**Description**|
|:-----|:-----|
|Default (Défaut)  <br/> |Indique que toutes les propriétés sont affichées.  <br/> |
|Compacter  <br/> |Indique que seules les propriétés sélectionnées sont affichées.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

