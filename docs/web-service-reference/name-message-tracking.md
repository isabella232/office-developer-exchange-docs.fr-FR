---
title: Name (MessageTracking)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Name
api_type:
- schema
ms.assetid: a1669f6d-53f3-4849-9b30-56909aaeac82
description: L’élément Name représente le nom de propriété d’un rapport de suivi des messages.
ms.openlocfilehash: b57c109cfbcb2744ae6854e0afce52e240d22b30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515452"
---
# <a name="name-message-tracking"></a>Name (MessageTracking)

**L’élément Name** représente le nom de propriété d’un rapport de suivi des messages. 
  
```xml
<Name/>
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
|[TrackingPropertyType](trackingpropertytype.md) <br/> |Représente une paire nom/valeur de chaînes utilisée pour créer des propriétés pour les rapports de suivi des messages.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Cet élément peut se produire au plus une fois dans [l’élément TrackingPropertyType.](trackingpropertytype.md) 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

