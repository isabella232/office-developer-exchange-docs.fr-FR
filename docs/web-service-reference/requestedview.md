---
title: RequestedView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestedView
api_type:
- schema
ms.assetid: e2b4cf8c-5d43-4cd8-b86d-cc27a5d2f095
description: L’élément RequestedView définit le type d’informations de calendrier demandées par un client.
ms.openlocfilehash: bc4f863841fc5a7d1d23f0bd4c7c2895d2593a2d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459159"
---
# <a name="requestedview"></a>RequestedView

L’élément **RequestedView** définit le type d’informations de calendrier demandées par un client. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[RequestedView](requestedview.md)
  
```xml
<RequestedView>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</RequestedView>
```

 **FreeBusyViewType**
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

Une valeur de texte est requise. Le tableau suivant répertorie les valeurs possibles pour cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |Cette valeur n’est pas valide pour les demandes. Cette valeur est valide pour les réponses.  <br/> |
|MergedOnly  <br/> |Représente un flux de disponibilité agrégé. Dans les scénarios entre forêts dans lesquels l’utilisateur cible d’une forêt ne dispose pas d’un service de disponibilité configuré, le service de disponibilité du demandeur récupère les informations de disponibilité de l’utilisateur cible à partir du dossier public disponible/occupé. Étant donné que les dossiers publics stockent uniquement les informations de disponibilité dans un formulaire fusionné, **MergedOnly** est la seule information disponible.  <br/> |
|Disponibilité  <br/> |Représente les informations d’État héritées : libre, occupé, provisoire et OOF. Cela inclut également les heures de début et de fin des rendez-vous. Cette vue est plus riche que la vue de disponibilité héritée, car les heures de début et de fin d’une réunion individuelle sont fournies au lieu d’un flux de disponibilité agrégé.  <br/> |
|FreeBusyMerged  <br/> |Représente toutes les propriétés dans **freebusy** avec un flux d’informations de disponibilité fusionnées.  <br/> |
|Précises  <br/> |Représente les informations d’État héritées : libre, occupé, provisoire et absent (e) du Bureau ; heures de début et de fin des rendez-vous ; et diverses propriétés du rendez-vous telles que l’objet, le lieu et l’importance. Cette vue demandée renverra la quantité maximale d’informations pour lesquelles l’utilisateur à l’origine de la demande est privilégié. Si les informations de disponibilité fusionnées uniquement sont disponibles, comme pour demander des informations pour les utilisateurs dans une forêt Microsoft Exchange Server 2003, **MergedOnly** sera renvoyé. Dans le cas contraire, **freebusy** ou **detailed** sera renvoyé.  <br/> |
|DetailedMerged  <br/> |Représente toutes les propriétés en **détail** avec un flux d’informations de disponibilité fusionnées. Si seules les informations de disponibilité fusionnées sont disponibles, **MergedOnly** est renvoyé. Sinon, **FreeBusyMerged** ou **DetailedMerged** sera renvoyé.  <br/> |
   
## <a name="remarks"></a>Remarques

La valeur définie par cet élément est renvoyée avec l’élément [FreeBusyViewType](freebusyviewtype.md) dans la réponse. 
  
Le tableau suivant indique les éléments renvoyés pour les différents types d’affichage et la propriété MAPI correspondante. Chaque type d’affichage repose sur le type d’affichage précédent.
  
|**Type de vue disponible/occupé**|**Propriétés**|**Propriété de calendrier MAPI**|
|:-----|:-----|:-----|
|**MergedOnly** <br/> |MergedFreeBusyStream  <br/> ||
|**FreeBusy** <br/> |État classique  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusy** <br/> |Heures de travail  <br/> ||
|**FreeBusy** <br/> |Heure de début  <br/> |PR_START_DATE  <br/> |
|**FreeBusy** <br/> |Heure de fin  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |État classique  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusyMerged** <br/> |Heures de travail  <br/> ||
|**FreeBusyMerged** <br/> |Heure de début  <br/> |PR_START_DATE  <br/> |
|**FreeBusyMerged** <br/> |Heure de fin  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**Précises** <br/> |État classique  <br/> |PropTag (0x80860003)  <br/> |
|**Précises** <br/> |Heures de travail  <br/> ||
|**Précises** <br/> |Heure de début  <br/> |PR_START_DATE  <br/> |
|**Précises** <br/> |Heure de fin  <br/> |PR_END_DATE  <br/> |
|**Précises** <br/> |Subject  <br/> |PR_SUBJECT  <br/> |
|**Précises** <br/> |Emplacement  <br/> |PR_LOCATION  <br/> |
|**Précises** <br/> |Entry-ID (sauf si privé)  <br/> ||
|**Précises** <br/> |Indicateur privé  <br/> ||
|**Précises** <br/> |IsMeeting  <br/> ||
|**Précises** <br/> |IsRecurring  <br/> ||
|**Précises** <br/> |IsException  <br/> ||
|**Précises** <br/> |IsReminderSet  <br/> ||
|**DetailedMerged** <br/> |État classique  <br/> |PropTag (0x80860003)  <br/> |
|**DetailedMerged** <br/> |Heures de travail  <br/> ||
|**DetailedMerged** <br/> |Heure de début  <br/> |PR_START_DATE  <br/> |
|**DetailedMerged** <br/> |Heure de fin  <br/> |PR_END_DATE  <br/> |
|**DetailedMerged** <br/> |Subject  <br/> |PR_SUBJECT  <br/> |
|**DetailedMerged** <br/> |Emplacement  <br/> |PR_LOCATION  <br/> |
|**DetailedMerged** <br/> |Entry-ID (sauf si privé)  <br/> ||
|**DetailedMerged** <br/> |Indicateur privé  <br/> ||
|**DetailedMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**DetailedMerged** <br/> |IsMeeting  <br/> ||
|**DetailedMerged** <br/> |IsRecurring  <br/> ||
|**DetailedMerged** <br/> |IsException  <br/> ||
|**DetailedMerged** <br/> |IsReminderSet  <br/> ||
   
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

