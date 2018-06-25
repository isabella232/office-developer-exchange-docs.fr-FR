---
title: WorkingPeriodArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriodArray
api_type:
- schema
ms.assetid: 3a3f6393-eacc-4734-b6c9-b67023fe2830
description: L’élément WorkingPeriodArray contient l’utilisation des informations sur les périodes de l’utilisateur de boîte aux lettres.
ms.openlocfilehash: 02712f05dc3373a532d769f476341b78ad25a79c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839067"
---
# <a name="workingperiodarray"></a>WorkingPeriodArray

L’élément **WorkingPeriodArray** contient l’utilisation des informations sur les périodes de l’utilisateur de boîte aux lettres. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[WorkingHours](workinghours-ex15websvcsotherref.md)
  
[WorkingPeriodArray](workingperiodarray.md)
  
```xml
<WorkingPeriodArray>
   <WorkingPeriod>...</WorkingPeriod>
</WorkingPeriodArray>
```

 **ArrayOfWorkingPeriod**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[WorkingPeriod](workingperiod.md) <br/> |Contient la semaine de travail les jours et les heures de l’utilisateur de boîte aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |Représente les paramètres de fuseau horaire et les heures de travail pour l’utilisateur de boîte aux lettres demandée.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est obligatoire si l’élément [WorkingHours](workinghours-ex15websvcsotherref.md) est utilisé. Tous les éléments enfants sont répertoriés dans l’ordre dans lequel elles se produisent. 
  
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

