---
title: FreeBusyViewType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FreeBusyViewType
api_type:
- schema
ms.assetid: 7c7f82ba-fa52-4a3e-bec7-39d373c66fc7
description: L’élément FreeBusyViewType représente le type d’informations de libre/occupé renvoyées dans la réponse.
ms.openlocfilehash: 6eec490b39ccb9c02e7a16c8da7cfdd57f9b92c5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509923"
---
# <a name="freebusyviewtype"></a>FreeBusyViewType

**L’élément FreeBusyViewType représente** le type d’informations de libre/occupé renvoyées dans la réponse. 
  
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

Une valeur de texte est requise. Le tableau suivant répertorie les valeurs possibles pour cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |Cette valeur n’est pas valide pour les demandes. Cette valeur est valide pour les réponses.  <br/> |
|MergedOnly  <br/> |Représente un flux de libre/occupé agrégé. Dans les scénarios entre forêts dans lesquels un service de disponibilité n’est pas configuré pour l’utilisateur cible dans une forêt, le service de disponibilité du demandeur récupère les informations de disponibilité de l’utilisateur cible à partir du dossier public de disponibilité. Étant donné que les dossiers publics stockent uniquement les informations de libre/occupé sous forme fusionnée, **MergedOnly** est la seule information disponible.  <br/> |
|Disponibilité  <br/> |Représente les informations d’état héritées : libre, occupé, provisoire et absence du service. Cela inclut également les heures de début/fin des rendez-vous. Cette vue est plus riche que la vue de libre/occupé héritée, car les heures de début et de fin de réunion individuelles sont fournies au lieu d’un flux de libre/occupé agrégé.  <br/> |
|FreeBusyMerged  <br/> |Représente toutes les propriétés de **FreeBusy** avec un flux d’informations de disponibilité fusionnées.  <br/> |
|Détails  <br/> |Représente les informations d’état héritées : libre, occupé, provisoire et OOF ; heures de début/fin des rendez-vous ; et diverses propriétés du rendez-vous telles que l’objet, le lieu et l’importance. Cette vue demandée retourne la quantité maximale d’informations pour laquelle l’utilisateur demandeur est privilégié. Si des informations de libre/occupé fusionnées sont disponibles uniquement, comme pour les informations de demande pour les utilisateurs d’une forêt Microsoft Exchange Server 2003, **MergedOnly** est renvoyé. Dans le cas **contraire, FreeBusy** **ou Detailed** sera renvoyé.  <br/> Si **detailed** est spécifié pour une liste de distribution, les informations de libre/occupé des membres de la liste sont fusionnées et **MergedOnly** est renvoyé.  <br/> |
|DetailedMerged  <br/> |Représente toutes les propriétés dans **Detailed** avec un flux d’informations de disponibilité fusionnées. Si seules les informations de libre/occupé fusionnées sont disponibles, par exemple si la boîte aux lettres existe sur un ordinateur exécutant Exchange 2003, **MergedOnly** est renvoyé. Dans le **cas contraire, FreeBusyMerged** ou **DetailedMerged** sera renvoyé.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est requis si [l’élément FreeBusyView](freebusyview.md) est utilisé. Le type d’informations de libre/occupé renvoyé est désigné dans [l’élément RequestedView.](requestedview.md) Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé. 
  
Le tableau suivant indique ce qui est renvoyé pour les différents types d’affichage et la propriété MAPI correspondante. Chaque type d’affichage s’appuie sur l’ancien type d’affichage.
  
|**FreeBusyViewType**|**Propriétés**|**MAPI Calendar, propriété**|
|:-----|:-----|:-----|
|**MergedOnly** <br/> |MergedFreeBusyStream  <br/> ||
|**FreeBusy** <br/> |Statut classique  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusy** <br/> |Heures de travail  <br/> ||
|**FreeBusy** <br/> |Heure de début  <br/> |PR_START_DATE  <br/> |
|**FreeBusy** <br/> |Heure de fin  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |Statut classique  <br/> |PropTag (0x80860003)  <br/> |
|**FreeBusyMerged** <br/> |Heures de travail  <br/> ||
|**FreeBusyMerged** <br/> |Heure de début  <br/> |PR_START_DATE  <br/> |
|**FreeBusyMerged** <br/> |Heure de fin  <br/> |PR_END_DATE  <br/> |
|**FreeBusyMerged** <br/> |MergedFreeBusyStream  <br/> ||
|**Détails** <br/> |Statut classique  <br/> |PropTag (0x80860003)  <br/> |
|**Détails** <br/> |Heures de travail  <br/> ||
|**Détails** <br/> |Heure de début  <br/> |PR_START_DATE  <br/> |
|**Détails** <br/> |Heure de fin  <br/> |PR_END_DATE  <br/> |
|**Détails** <br/> |Sujet  <br/> |PR_SUBJECT  <br/> |
|**Détails** <br/> |Emplacement  <br/> |PR_LOCATION  <br/> |
|**Détails** <br/> |Entry-Id(sauf privé)  <br/> ||
|**Détails** <br/> |Indicateur privé  <br/> ||
|**Détails** <br/> |IsMeeting  <br/> ||
|**Détails** <br/> |IsRecurring  <br/> ||
|**Détails** <br/> |IsException  <br/> ||
|**Détails** <br/> |IsReminderSet  <br/> ||
|**Détails** <br/> |Message hors Office (si nécessaire)  <br/> ||
|**DetailedMerged** <br/> |Statut classique  <br/> |PropTag (0x80860003)  <br/> |
|**DetailedMerged** <br/> |Heures de travail  <br/> ||
|**DetailedMerged** <br/> |Heure de début  <br/> |PR_START_DATE  <br/> |
|**DetailedMerged** <br/> |Heure de fin  <br/> |PR_END_DATE  <br/> |
|**DetailedMerged** <br/> |Sujet  <br/> |PR_SUBJECT  <br/> |
|**DetailedMerged** <br/> |Emplacement  <br/> |PR_LOCATION  <br/> |
|**DetailedMerged** <br/> |Entry-Id(sauf privé)  <br/> ||
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
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

