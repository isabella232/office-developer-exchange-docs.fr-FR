---
title: TimeWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeWindow
api_type:
- schema
ms.assetid: 49c79266-353a-4036-a8e2-8a4660d0d8ea
description: L’élément TimeWindow identifie l’étendue de temps à interroger pour les informations de disponibilité de l’utilisateur.
ms.openlocfilehash: 93a486a5bc2306cfa61b74de82d795a711dbbceb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531343"
---
# <a name="timewindow"></a>TimeWindow

**L’élément TimeWindow** identifie l’étendue de temps à interroger pour les informations de disponibilité de l’utilisateur. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[TimeWindow](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 **Duration**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Représente le début d’un laps de temps interrogé pour les informations de disponibilité de l’utilisateur.  <br/> |
|[EndTime](endtime.md) <br/> |Représente la fin d’un laps de temps interrogé pour les informations de disponibilité de l’utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |Spécifie le type d’informations de libre/occupé renvoyées dans la réponse.  <br/> Voici le chemin d’accès XPath à cet élément :  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a>Remarques

La valeur maximale pour cette période est de 42 jours. Cette valeur maximale peut être modifiée. Toute demande d’informations de disponibilité utilisateur au-delà de la valeur maximale retourne une erreur. Si des rendez-vous sont partiellement dans l’intervalle de temps défini par les éléments [StartTime](starttime.md) et [EndTime,](endtime.md) ce rendez-vous est inclus dans son intégralité. 
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute Microsoft® Exchange Server 2007 sur qui le rôle serveur d’accès au client est installé. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)


[Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

