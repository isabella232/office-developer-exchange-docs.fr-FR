---
title: TrackingPropertyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TrackingPropertyType
api_type:
- schema
ms.assetid: 1d0f219b-1063-4eaa-9d3b-da384a544f89
description: L’élément TrackingPropertyType représente une paire nom/valeur de chaînes utilisée pour créer des propriétés pour les rapports de suivi des messages.
ms.openlocfilehash: f26f2a2f512d0816ac34d801169972c670e5ff25
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517538"
---
# <a name="trackingpropertytype"></a>TrackingPropertyType

**L’élément TrackingPropertyType** représente une paire nom/valeur de chaînes utilisée pour créer des propriétés pour les rapports de suivi des messages. 
  
[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md)
  
[TrackingPropertyType](trackingpropertytype.md)
  
```xml
<TrackingPropertyType>
   <Name/>
   <Value/>
</TrackingPropertyType>
```

 **TrackingPropertyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Name (MessageTracking)](name-message-tracking.md) <br/> |Définit un nom pour la propriété du rapport de suivi des messages.  <br/> |
|[Value (MessageTracking)](value-message-tracking.md) <br/> |Définit une valeur pour la propriété du rapport de suivi des messages. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contient une liste d’une ou plusieurs propriétés de suivi.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

