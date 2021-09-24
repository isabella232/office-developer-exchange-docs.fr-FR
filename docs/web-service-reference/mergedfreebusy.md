---
title: MergedFreeBusy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: L’élément MergedFreeBusy contient le flux de données de libre/occupé fusionné.
ms.openlocfilehash: db451d6b2e67313836771604fae57b14b6b3db10
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511029"
---
# <a name="mergedfreebusy"></a>MergedFreeBusy

**L’élément MergedFreeBusy** contient le flux de données de libre/occupé fusionné. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[MergedFreeBusy](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyView](freebusyview.md) <br/> |Contient des informations de disponibilité pour un utilisateur spécifique.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est fournie par le serveur si la valeur de l’élément [FreeBusyViewType](freebusyviewtype.md) est l’une des suivantes : 
  
- DetailedMerged
    
- FreeBusyMerged
    
- MergedOnly
    
La valeur de texte est un flux d’informations de libre/occupé. 
  
## <a name="remarks"></a>Remarques

Le flux de données fourni par cet élément est défini par les éléments [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) et [TimeWindow.](timewindow.md) [L’élément TimeWindow](timewindow.md) définit l’étendue de temps pour la disponibilité. [L’élément MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) définit la façon dont l’heure de l’élément [TimeWindow](timewindow.md) est décomposée en intervalles renvoyés dans l’élément **MergedFreeBusy.** Chaque nombre dans le **flux MergedFreeBusy** représente un intervalle unique défini par l’élément [MergedFreeBusyIntervalInMinutes.](mergedfreebusyintervalinminutes.md) Le tableau suivant répertorie les valeurs possibles pour un intervalle individuel. 
  
|**Chiffre**|**Disponibilité**|
|:-----|:-----|
|0  <br/> |Gratuit  <br/> |
|1  <br/> |Provisoire  <br/> |
|2  <br/> |Occupé(e)  <br/> |
|3  <br/> |Absent(e) du bureau  <br/> |
|4   <br/> |Aucune donnée  <br/> |
   
Par exemple, une demande de données de libre/occupé inclut un élément [TimeWindow](timewindow.md) qui représente quatre heures et un élément [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) qui représente 60 minutes. Si le calendrier de l’utilisateur demandé est en absence du bureau pendant les 60 premières minutes, occupé pendant les 90 minutes suivantes et non reporté pour les 90 dernières minutes dans la fenêtre de temps, le flux **MergedFreeBusy** sera 3220. Si un intervalle contient plusieurs classifications de disponibilité, le nombre le plus élevé est utilisé pour classer cet intervalle. 
  
Le niveau de détail fourni par cet élément dépend des autorisations accordées au demandeur.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

