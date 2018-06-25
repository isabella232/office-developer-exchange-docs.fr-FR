---
title: FreeBusyView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: L’élément FreeBusyView contient des informations de disponibilité pour un utilisateur spécifique.
ms.openlocfilehash: d0d603f18642a94e841a1a6bb8e8849aa6b5b273
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756486"
---
# <a name="freebusyview"></a>FreeBusyView

L’élément **FreeBusyView** contient des informations de disponibilité pour un utilisateur spécifique. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyViewType](freebusyviewtype.md) <br/> |Représente le type d’informations de disponibilité demandées retournés dans la réponse.  <br/> |
|[MergedFreeBusy](mergedfreebusy.md) <br/> |Contient le flux de disponibilité fusionné de données.  <br/> |
|[CalendarEventArray](calendareventarray.md) <br/> |Contient un ensemble d’occurrences d’élément calendrier unique représentant la disponibilité de l’utilisateur demandé.  <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Représente les paramètres de fuseau horaire et les heures de travail pour l’utilisateur de boîte aux lettres demandée.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyResponse](freebusyresponse.md) <br/> |Contient les informations de disponibilité pour un utilisateur de boîte aux lettres unique.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a>Remarques

Tous les éléments enfants sont répertoriés dans l’ordre dans lequel elles se produisent. Le niveau de détail fourni par cet élément varie selon les autorisations accordées au demandeur.
  
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

