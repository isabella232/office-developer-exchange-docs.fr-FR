---
title: FreeBusyView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: L’élément FreeBusyView contient des informations de disponibilité pour un utilisateur spécifique.
ms.openlocfilehash: c662e8a44118f61b4c8be642d9ac862051c3a15d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546412"
---
# <a name="freebusyview"></a>FreeBusyView

**L’élément FreeBusyView contient** des informations de disponibilité pour un utilisateur spécifique. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
```xml
<FreeBusyView>
   <FreeBusyViewType>...</FreeBusyViewType>
   <MergedFreeBusy>...</MergedFreeBusy>
   <CalendarEventArray>...</CalendarEventArray>
   <WorkingHours>...</WorkingHours>
</FreeBusyView>
```

 **FreeBusyView**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyViewType](freebusyviewtype.md) <br/> |Représente le type d’informations de libre/occupé demandées renvoyées dans la réponse.  <br/> |
|[MergedFreeBusy](mergedfreebusy.md) <br/> |Contient le flux de données de la libre/occupé fusionnée.  <br/> |
|[CalendarEventArray](calendareventarray.md) <br/> |Contient un ensemble d’occurrences d’éléments de calendrier uniques qui représentent la disponibilité de l’utilisateur demandé.  <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Représente les paramètres de fuseau horaire et les heures de travail de l’utilisateur de boîte aux lettres demandé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyResponse](freebusyresponse.md) <br/> |Contient les informations de libre/occupé d’un utilisateur de boîte aux lettres unique.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a>Remarques

Tous les éléments enfants sont répertoriés dans l’ordre dans lequel ils se produisent. Le niveau de détail fourni par cet élément dépend des autorisations accordées au demandeur.
  
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

