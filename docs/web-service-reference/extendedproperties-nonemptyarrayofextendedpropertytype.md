---
title: ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a7034730-210d-4916-b992-dda342f890f8
description: L’élément ExtendedProperties spécifie un tableau de propriétés supplémentaires.
ms.openlocfilehash: b92108ecde63d4a3ac3cc80861c204c4d1950cc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756296"
---
# <a name="extendedproperties-nonemptyarrayofextendedpropertytype"></a>ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)

L’élément **ExtendedProperties** spécifie un tableau de propriétés supplémentaires. 
  
```XML
<ExtendedProperties>
    <ExtendedProperty/>
</ExtendedProperties>
```

 **NonEmptyArrayOfExtendedPropertyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |Identifie les propriétés MAPI étendues sur les dossiers et éléments.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ImGroup](imgroup.md) <br/> |Représente un groupe de messagerie instantané.  <br/> |
|[SearchPreviewItem](searchpreviewitem.md) <br/> |Spécifie les 256 premiers caractères d’un élément de boîte aux lettres pour l’aperçu sans ouvrir l’élément.  <br/> |
   
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

