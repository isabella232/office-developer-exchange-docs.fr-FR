---
title: Nom (le suivi des messages)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: a1669f6d-53f3-4849-9b30-56909aaeac82
description: L’élément Name représente le nom de propriété pour un rapport de suivi des messages.
ms.openlocfilehash: c905df03842de47b2bcbd62897aa9a8cf464cc6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828501"
---
# <a name="name-message-tracking"></a>Nom (le suivi des messages)

L’élément **Name** représente le nom de propriété pour un rapport de suivi des messages. 
  
```xml
<Name/>
```

**Chaîne**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |Représente une paire nom / valeur de chaînes qui sert à créer des propriétés pour les rapports de suivi des messages.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte est obligatoire si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Cet élément peut se produire au maximum une seule fois dans l’élément [TrackingPropertyType](trackingpropertytype.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

