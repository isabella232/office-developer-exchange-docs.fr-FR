---
title: FreeBusyViewType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyViewType
api_type:
- schema
ms.assetid: 7c7f82ba-fa52-4a3e-bec7-39d373c66fc7
description: L’élément FreeBusyViewType représente le type d’informations disponible/occupé retournés dans la réponse.
ms.openlocfilehash: fe965d062f72d99dff7148f4d00b12fd8c4e1366
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756501"
---
# <a name="freebusyviewtype"></a>FreeBusyViewType

L’élément **FreeBusyViewType** représente le type d’informations disponible/occupé retournés dans la réponse. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[FreeBusyViewType](freebusyviewtype.md)
  
```xml
<FreeBusyViewType>None or MergedOnly or FreeBusy or FreeBusyMerged or Detailed or DetailedMerged</FreeBusyViewType>
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
|[FreeBusyView](freebusyview.md) <br/> |Contient des informations de disponibilité pour un utilisateur spécifique.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Le tableau suivant répertorie les valeurs possibles de cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|None  <br/> |Cette valeur n’est pas valide pour les demandes. Cette valeur est valide pour les réponses.  <br/> |
|MergedOnly  <br/> |Représente un flux d’informations de disponibilité agrégé. Dans les scénarios inter-forêts dans laquelle l’utilisateur cible dans une forêt n’a pas un configuration du service de disponibilité, le service de disponibilité du demandeur récupère les informations de disponibilité de l’utilisateur cible à partir du dossier public et de disponibilité. Dossiers publics enregistrer uniquement les informations disponible/occupé dans formulaire fusionné, **MergedOnly** étant donné que les informations disponibles uniquement.  <br/> |
|Disponibilité  <br/> |Représente les informations d’état hérité : libre, provisoire, occupé (e) et d’absence du bureau. Cela inclut également les heures de début/fin du rendez-vous. Cet affichage est plus riche que hérité des disponibilités afficher car individuellement début et de fin fois sont fournies au lieu d’un flux de disponibilité agrégé.  <br/> |
|FreeBusyMerged  <br/> |Représente les propriétés de **FreeBusy** avec un flux d’informations de disponibilité de disponibilité fusionné.  <br/> |
|Détaillé  <br/> |Représente les informations d’état hérité : libre, provisoire, occupé et ADB ; les heures de début/fin du rendez-vous ; ainsi que différentes propriétés du rendez-vous comme objet, emplacement et importance. Cet affichage demandé renverra le maximum d’informations pour laquelle l’utilisateur est privilégié. Si les informations de disponibilité fusionnées ne sont disponibles, comme avec demander des informations pour les utilisateurs d’une forêt Microsoft Exchange Server 2003, **MergedOnly** s’afficheront. Dans le cas contraire, **FreeBusy** ou **détaillé** est retournées.  <br/> Si **détaillé** est spécifié pour une liste de distribution, les informations de disponibilité pour les membres de la liste sont fusionnées et **MergedOnly** est renvoyée.  <br/> |
|DetailedMerged  <br/> |Représente toutes les propriétés de **détaillé** avec un flux d’informations de disponibilité de disponibilité fusionné. Si une seule fusionnées informations disponible/occupé sont disponibles, par exemple, si la boîte aux lettres existe sur un ordinateur qui exécute Exchange 2003, **MergedOnly** seront retournées. Dans le cas contraire, **FreeBusyMerged** ou **DetailedMerged** s’afficheront.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est obligatoire si l’élément [FreeBusyView](freebusyview.md) est utilisé. Le type d’informations de disponibilité renvoyées est indiqué dans l’élément [RequestedView](requestedview.md) . Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé. 
  
Le tableau suivant indique ce qui est renvoyé pour les types d’affichage différents et la propriété MAPI correspondante. Chaque type d’affichage s’appuie sur le type d’affichage précédent.
  
|**FreeBusyViewType**|**Propriétés**|**Propriété MAPI calendrier**|
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
|**Détaillées** <br/> |Message d’Office (si nécessaire)  <br/> ||
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
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obtention de disponibilité de l’utilisateur](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

