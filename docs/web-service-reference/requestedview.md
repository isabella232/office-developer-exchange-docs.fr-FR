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
description: L’élément RequestedView définit le type des informations de calendrier que demande un client.
ms.openlocfilehash: 7710227720264432c325f95da894cbbbd4748dc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829145"
---
# <a name="requestedview"></a>RequestedView

L’élément **RequestedView** définit le type des informations de calendrier que demande un client. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[FreeBusyViewOptions](freebusyviewoptions.md)
  
[RequestedView](requestedview.md)
  
```xml
<RequestedView>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</RequestedView>
```

 **FreeBusyViewType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyViewOptions](freebusyviewoptions.md) <br/> |Spécifie le type d’informations disponible/occupé retournés dans la réponse.  <br/> Vous trouverez ci-dessous le XPath pour cet élément :  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Le tableau suivant répertorie les valeurs possibles de cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|None  <br/> |Cette valeur n’est pas valide pour les demandes. Cette valeur est valide pour les réponses.  <br/> |
|MergedOnly  <br/> |Représente un flux d’informations de disponibilité agrégé. Dans les scénarios inter-forêts dans laquelle l’utilisateur cible dans une forêt n’a pas un configuration du service de disponibilité, le service de disponibilité du demandeur récupère les informations de disponibilité de l’utilisateur cible à partir du dossier public et de disponibilité. Dossiers publics enregistrer uniquement les informations disponible/occupé dans formulaire fusionné, **MergedOnly** étant donné que les informations disponibles uniquement.  <br/> |
|Disponibilité  <br/> |Représente les informations d’état hérité : libre, provisoire, occupé (e) et d’absence du bureau. Cela inclut également les heures de début/fin du rendez-vous. Cet affichage est plus riche que hérité des disponibilités afficher car individuellement début et de fin fois sont fournies au lieu d’un flux de disponibilité agrégé.  <br/> |
|FreeBusyMerged  <br/> |Représente les propriétés de **FreeBusy** avec un flux d’informations de disponibilité fusionnés.  <br/> |
|Détaillé  <br/> |Représente les informations d’état hérité : libre, provisoire, occupé et ADB ; les heures de début/fin du rendez-vous ; ainsi que différentes propriétés du rendez-vous comme objet, emplacement et importance. Cet affichage demandé renverra le maximum d’informations pour laquelle l’utilisateur est privilégié. Si les informations de disponibilité fusionnées ne sont disponibles, comme avec demander des informations pour les utilisateurs d’une forêt Microsoft Exchange Server 2003, **MergedOnly** s’afficheront. Dans le cas contraire, **FreeBusy** ou **détaillé** est retournées.  <br/> |
|DetailedMerged  <br/> |Représente les propriétés de **détaillé** avec un flux d’informations de disponibilité fusionnés. Si les informations de disponibilité fusionnées ne sont disponibles, **MergedOnly** seront retournées. Dans le cas contraire, **FreeBusyMerged** ou **DetailedMerged** s’afficheront.  <br/> |
   
## <a name="remarks"></a>Remarques

La valeur de cet élément est renvoyée avec l’élément [FreeBusyViewType](freebusyviewtype.md) dans la réponse. 
  
Le tableau suivant indique ce qui est renvoyé pour les types d’affichage différents et la propriété MAPI correspondante. Chaque type d’affichage s’appuie sur le type d’affichage précédent.
  
|**Type d’affichage des informations de disponibilité**|**Propriétés**|**Propriété MAPI calendrier**|
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
|**Détaillées** <br/> |État classique  <br/> |PropTag (0x80860003)  <br/> |
|**Détaillées** <br/> |Heures de travail  <br/> ||
|**Détaillées** <br/> |Heure de début  <br/> |PR_START_DATE  <br/> |
|**Détaillées** <br/> |Heure de fin  <br/> |PR_END_DATE  <br/> |
|**Détaillées** <br/> |Objet  <br/> |PR_SUBJECT  <br/> |
|**Détaillées** <br/> |Emplacement  <br/> |EMPLACEMENT_PR  <br/> |
|**Détaillées** <br/> |Entrée-Id(unless private)  <br/> ||
|**Détaillées** <br/> |Indicateur privé  <br/> ||
|**Détaillées** <br/> |IsMeeting  <br/> ||
|**Détaillées** <br/> |IsRecurring  <br/> ||
|**Détaillées** <br/> |IsException  <br/> ||
|**Détaillées** <br/> |IsReminderSet  <br/> ||
|**DetailedMerged** <br/> |État classique  <br/> |PropTag (0x80860003)  <br/> |
|**DetailedMerged** <br/> |Heures de travail  <br/> ||
|**DetailedMerged** <br/> |Heure de début  <br/> |PR_START_DATE  <br/> |
|**DetailedMerged** <br/> |Heure de fin  <br/> |PR_END_DATE  <br/> |
|**DetailedMerged** <br/> |Objet  <br/> |PR_SUBJECT  <br/> |
|**DetailedMerged** <br/> |Emplacement  <br/> |EMPLACEMENT_PR  <br/> |
|**DetailedMerged** <br/> |Entrée-Id(unless private)  <br/> ||
|**DetailedMerged** <br/> |Indicateur privé  <br/> ||
|**DetailedMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**DetailedMerged** <br/> |IsMeeting  <br/> ||
|**DetailedMerged** <br/> |IsRecurring  <br/> ||
|**DetailedMerged** <br/> |IsException  <br/> ||
|**DetailedMerged** <br/> |IsReminderSet  <br/> ||
   
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

