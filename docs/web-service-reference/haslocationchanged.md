---
title: HasLocationChanged
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5fd465b4-6070-4cd0-9ac3-ed9d2bfd5951
description: L’élément HasLocationChanged spécifie si la propriété d’emplacement d’une réunion a changé.
ms.openlocfilehash: f59bca138d0baee87afd12470d9c50704edc75bd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519547"
---
# <a name="haslocationchanged"></a>HasLocationChanged

**L’élément HasLocationChanged** spécifie si la propriété d’emplacement d’une réunion a changé. 
  
```XML
<HasLocationChanged> true | false </HasLocationChanged>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ChangeHighlights](changehighlights.md) <br/> |Spécifie ce qui a changé entre deux versions d’un message de demande de réunion.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true pour** **l’élément HasLocationChanged** indique que la propriété d’emplacement d’une réunion a changé. Une valeur **false** indique que la propriété d’emplacement d’une réunion n’a pas changé. 
  
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

