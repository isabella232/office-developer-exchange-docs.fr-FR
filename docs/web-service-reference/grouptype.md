---
title: GroupType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c31552f-22b8-4bf0-8cac-046fd92ac0d4
description: L’élément GroupType spécifie la classe de groupe d’un groupe (IM) de messagerie instantanée.
ms.openlocfilehash: 330a1567ce85877ba73c6205898ea66b59585e16
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827800"
---
# <a name="grouptype"></a>GroupType

L’élément **GroupType** spécifie la classe de groupe d’un groupe (IM) de messagerie instantanée. 
  
```XML
<GroupType></GroupType>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ImGroup](imgroup.md) <br/> |Représente un groupe de messagerie instantané.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **GroupType** est une valeur de type string qui spécifie le type du groupe. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

