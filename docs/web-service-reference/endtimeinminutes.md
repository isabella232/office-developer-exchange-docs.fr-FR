---
title: EndTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTimeInMinutes
api_type:
- schema
ms.assetid: ef05bdda-7a66-44db-bb73-a2ce8316c257
description: L’élément EndTimeInMinutes représente la fin de la journée de travail pour un utilisateur de boîte aux lettres.
ms.openlocfilehash: 2885d810512eb0e575aa25b4f38d28332a10b8f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756198"
---
# <a name="endtimeinminutes"></a>EndTimeInMinutes

L’élément **EndTimeInMinutes** représente la fin de la journée de travail pour un utilisateur de boîte aux lettres. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[WorkingHours](workinghours-ex15websvcsotherref.md)
  
[WorkingPeriodArray](workingperiodarray.md)
  
[WorkingPeriod](workingperiod.md)
  
[EndTimeInMinutes](endtimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[WorkingPeriod](workingperiod.md) <br/> |Contient la semaine de travail les jours et les heures de l’utilisateur de boîte aux lettres.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i]` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. La valeur de texte représente la fin de la journée de travail par le nombre de minutes se sont écoulées depuis le début de la journée. Par exemple, une heure de fin à 18 : 00 est représenté par 1 080 minutes.
  
La plage de valeurs possibles pour cet élément est 0 et 1440.
  
## <a name="remarks"></a>Remarques

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

