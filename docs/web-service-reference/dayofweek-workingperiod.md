---
title: DayOfWeek (WorkingPeriod)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 7a8a8cc1-392b-4db5-bb76-710477e31396
description: L’élément DayOfWeek contient la liste des jours ou travaillés programmés pour l’utilisateur de boîte aux lettres.
ms.openlocfilehash: 97950d7f2d6db76ac76253979e9187bddc5c99e1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529005"
---
# <a name="dayofweek-workingperiod"></a>DayOfWeek (WorkingPeriod)

**L’élément DayOfWeek** contient la liste des jours ou travaillés programmés pour l’utilisateur de boîte aux lettres. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[WorkingPeriod](workingperiod.md) <br/> |Contient les jours et heures de la semaine de travail de l’utilisateur de boîte aux lettres.<br/><br/>Voici l’expression XPath de cet élément :<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur texte est renvoyée si l’utilisateur de la boîte aux lettres a des jours pour représenter la semaine de travail. Les valeurs possibles pour cet élément sont les suivantes :
  
- Dimanche    
- Lundi    
- Mardi    
- Mercredi    
- Jeudi    
- Vendredi    
- Samedi 
    
Les valeurs de texte sont renvoyées dans cet ordre.
  
## <a name="remarks"></a>Remarques

Il est important de noter que la différence entre cet élément et l’élément [Availability DayOfWeek (TimeZone)](dayofweek-timezone.md) est le type. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

