---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: L’élément DateTimePrecision spécifie la précision des valeurs de date/heure renvoyée.
ms.openlocfilehash: 4d11598628228b41adf021adbbaa77e6348534bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755802"
---
# <a name="datetimeprecision"></a>DateTimePrecision

L’élément **DateTimePrecision** spécifie la précision des valeurs de date/heure renvoyée. 
  
```XML
<DateTimePrecision />
```

**DateTimePrecisionType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

L’élément **DateTimePrecision** se trouve dans l’en-tête SOAP. 
  
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Les valeurs possibles sont les suivantes :
  
- Secondes
    
- Millisecondes
    
## <a name="remarks"></a>Remarques

Date/heure lorsqu’un en-tête SOAP avec l’élément **DateTimePrecision** défini sur « Secondes » est utilisé, les valeurs sont renvoyées aux plus proche secondes (00 : 00:00). Date/heure lorsque « Millisecondes » sont utilisées, les valeurs sont renvoyées à la milliseconde (00:00:00.0000). 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

