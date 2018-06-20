---
title: MergedFreeBusy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: L’élément MergedFreeBusy contient le flux de disponibilité fusionné de données.
ms.openlocfilehash: 542b9fae0c36b0236bd806e8a9117753968e812c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828449"
---
# <a name="mergedfreebusy"></a>MergedFreeBusy

L’élément **MergedFreeBusy** contient le flux de disponibilité fusionné de données. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[MergedFreeBusy](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyView](freebusyview.md) <br/> |Contient des informations de disponibilité pour un utilisateur spécifique.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte est fournie par le serveur si la valeur de l’élément [FreeBusyViewType](freebusyviewtype.md) est une des options suivantes : 
  
- DetailedMerged
    
- FreeBusyMerged
    
- MergedOnly
    
La valeur de texte est un flux d’informations de disponibilité. 
  
## <a name="remarks"></a>Remarques

Le flux de données fournis par cet élément est défini par les éléments [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) et [durée](timewindow.md) . L’élément de [durée](timewindow.md) définit l’intervalle de temps interrogé pour la disponibilité. L’élément [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) définit comment l’heure à partir de l’élément de la [durée](timewindow.md) est divisé en intervalles renvoyés dans l’élément **MergedFreeBusy** . Chaque numéro dans le flux **MergedFreeBusy** représente un intervalle unique défini par l’élément [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) . Le tableau suivant répertorie les valeurs possibles pour un intervalle spécifique. 
  
|**Chiffre**|**Disponibilité**|
|:-----|:-----|
|0  <br/> |Gratuit  <br/> |
|1  <br/> |Provisoire  <br/> |
|2  <br/> |Occupé(e)  <br/> |
|3  <br/> |Absent(e) du bureau  <br/> |
|4  <br/> |Aucune donnée  <br/> |
   
Par exemple, une demande de données et de disponibilité inclut un élément de [durée](timewindow.md) qui représente les quatre heures et un élément [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) qui représente 60 minutes. Si le calendrier de l’utilisateur demandé est absent du bureau pour les premières 60 minutes, occupé (e) pour les 90 minutes suivantes et non planifiée pour les 90 minutes finales dans la fenêtre de temps, le flux **MergedFreeBusy** seront 3220. Si un intervalle contient plusieurs classifications de disponibilité, le nombre le plus élevé est utilisé pour classer cet intervalle. 
  
Le niveau de détail fourni par cet élément varie selon les autorisations accordées au demandeur.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obtention de disponibilité de l’utilisateur](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

