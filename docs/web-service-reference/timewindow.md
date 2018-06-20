---
title: Durée
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeWindow
api_type:
- schema
ms.assetid: 49c79266-353a-4036-a8e2-8a4660d0d8ea
description: L’élément durée identifie l’intervalle de temps interrogé pour les informations de disponibilité utilisateur.
ms.openlocfilehash: 05858b4d62b72b3ff9904c90652bb1bff78ceb41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838725"
---
# <a name="timewindow"></a>Durée

L’élément **durée** identifie l’intervalle de temps interrogé pour les informations de disponibilité utilisateur. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[Durée](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 **Durée**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Heure de début](starttime.md) <br/> |Représente le début d’une période interrogé pour les informations de disponibilité utilisateur.  <br/> |
|[Heure de fin](endtime.md) <br/> |Représente la fin d’une période interrogée pour les informations de disponibilité utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |Spécifie le type d’informations disponible/occupé retournés dans la réponse.  <br/> Vous trouverez ci-dessous le XPath pour cet élément :  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a>Remarques

La valeur maximale pour cette période est de 42 jours. Cette valeur maximale peut être modifiée. Toutes les demandes des informations de disponibilité utilisateur au-delà de la valeur maximale renverra une erreur. Si aucun rendez-vous sont partiellement dans la période définie par les éléments [StartTime](starttime.md) et [EndTime](endtime.md) , ce rendez-vous est inclus dans son intégralité. 
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute Microsoft® Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)


[Obtention de disponibilité de l’utilisateur](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

