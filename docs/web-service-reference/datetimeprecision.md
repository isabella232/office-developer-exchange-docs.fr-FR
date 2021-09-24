---
title: DateTimePrecision
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: L’élément DateTimePrecision spécifie la précision des valeurs de date/heure renvoyées.
ms.openlocfilehash: 075e37bfdd2c61f56352e000ef6cc5810dd81bbb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535709"
---
# <a name="datetimeprecision"></a>DateTimePrecision

**L’élément DateTimePrecision** spécifie la précision des valeurs de date/heure renvoyées. 
  
```XML
<DateTimePrecision />
```

**DateTimePrecisionType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

**L’élément DateTimePrecision** se trouve dans l’en-tête SOAP. 
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Les valeurs possibles sont les suivantes :
  
- Secondes
    
- Millisecondes
    
## <a name="remarks"></a>Remarques

Lorsqu’un en-tête SOAP avec l’élément **DateTimePrecision** sur « Seconds » est utilisé, les valeurs de date/heure sont renvoyées aux secondes les plus proches (00:00:00). Lorsque la valeur « Millisecondes » est utilisée, les valeurs de date/heure sont renvoyées à la milliseconde la plus proche (00:00:00.0000). 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

