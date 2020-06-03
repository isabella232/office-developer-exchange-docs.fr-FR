---
title: MergedFreeBusyIntervalInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusyIntervalInMinutes
api_type:
- schema
ms.assetid: 481cdbc6-d5aa-49fa-a3fa-9d119d3dca99
description: L’élément MergedFreeBusyIntervalInMinutes représente la différence de temps entre deux slots successifs dans la vue FreeBusyMerged.
ms.openlocfilehash: 6228ee5b66202634e6bb3b6c1ad6b8897a109d58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468788"
---
# <a name="mergedfreebusyintervalinminutes"></a>MergedFreeBusyIntervalInMinutes

L’élément **MergedFreeBusyIntervalInMinutes** représente la différence de temps entre deux slots successifs dans la vue **FreeBusyMerged** . 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md)
  
```xml
<MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |Spécifie le type d’informations de disponibilité renvoyées dans la réponse.  <br/> Voici le XPath de cet élément :  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur texte représente le temps en minutes. La valeur par défaut est 30 minutes. Six minutes est l’intervalle minimum et un jour (1440 minutes) est l’intervalle maximal de cet élément.
  
## <a name="remarks"></a>Remarques

Cette valeur est utilisée uniquement si l’élément [RequestedView](requestedview.md) est égal à **MergedOnly**, **FreeBusyMerged**ou **DetailedMerge**. Il s’agit d’un type de données Integer. Le flux qui contient les intervalles définis par cet élément est renvoyé dans l’élément [MergedFreeBusy](mergedfreebusy.md) . 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)
  
[Opération GetUserOofSettings](getuseroofsettings-operation.md)


[Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

