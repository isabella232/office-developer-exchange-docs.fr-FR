---
title: SortOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SortOrder
api_type:
- schema
ms.assetid: c2413f0b-8c03-46ae-9990-13338b3c53a6
description: L’élément SortOrder définit le mode de tri des éléments dans une requête FindItem ou FindConversation.
ms.openlocfilehash: b520bb3ca6daadc777e7235b2b7420a12e425048
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468368"
---
# <a name="sortorder"></a>SortOrder

L’élément **SortOrder** définit le mode de tri des éléments dans une requête **FindItem** ou **FindConversation** . 
  
```xml
<SortOrder>
   <FieldOrder/>
</SortOrder>
```

 **NonEmptyArrayOfFieldOrdersType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldOrder](fieldorder.md) <br/> |Représente un champ unique par lequel trier les résultats et indique le sens du tri. Un ou plusieurs de ces éléments peuvent être inclus. Les éléments [FieldOrder](fieldorder.md) sont appliqués dans l’ordre spécifié pour le tri.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher des éléments dans une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :`/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |Définit une requête pour rechercher des conversations dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)
  
[Opération FindConversation](findconversation-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

