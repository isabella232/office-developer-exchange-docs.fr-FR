---
title: DayOfWeek (WorkingPeriod)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 7a8a8cc1-392b-4db5-bb76-710477e31396
description: L’élément DayOfWeek contient la liste des jours de travail planifié pour l’utilisateur de boîte aux lettres.
ms.openlocfilehash: a6a68017291ba13f45b3970307669222d583fcbb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755826"
---
# <a name="dayofweek-workingperiod"></a>DayOfWeek (WorkingPeriod)

L’élément **DayOfWeek** contient la liste des jours de travail planifié pour l’utilisateur de boîte aux lettres. 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)  
- [FreeBusyResponseArray](freebusyresponsearray.md)  
- [FreeBusyResponse](freebusyresponse.md)  
- [FreeBusyView](freebusyview.md)  
- [WorkingHours](workinghours-ex15websvcsotherref.md)  
- [WorkingPeriodArray](workingperiodarray.md) 
- [WorkingPeriod](workingperiod.md)  
- [DayOfWeek (WorkingPeriod)](dayofweek-workingperiod.md)
  
```xml
<DayOfWeek>Sunday Monday Tuesday Wednesday Thursday Friday Saturday</DayOfWeek>
```

**DaysOfWeek**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[WorkingPeriod](workingperiod.md) <br/> |Contient la semaine de travail les jours et les heures de l’utilisateur de boîte aux lettres.<br/><br/>Vous trouverez ci-dessous l’expression XPath pour cet élément :<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte est renvoyée si l’utilisateur de boîte aux lettres a jours définissez pour représenter la semaine de travail. Les valeurs possibles de cet élément sont les suivantes :
  
- Dimanche    
- Lundi    
- Mardi    
- Mercredi    
- Jeudi    
- Vendredi    
- Samedi 
    
Les valeurs de texte seront afficheront dans l’ordre.
  
## <a name="remarks"></a>Remarques

Il est important de noter que la différence entre cet élément et l’élément disponibilité [DayOfWeek (fuseau horaire)](dayofweek-timezone.md) est le type. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [Obtention de disponibilité de l’utilisateur](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

