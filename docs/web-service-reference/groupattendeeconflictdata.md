---
title: GroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupAttendeeConflictData
api_type:
- schema
ms.assetid: fd8bf19a-298b-4135-93e8-ead3db7e1142
description: L’élément GroupAttendeeConflictData contient des informations sur les conflits globaux sur le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion suggérée.
ms.openlocfilehash: c75a4e6f8fdff7fb2514f448350fee9f1acb9775
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462928"
---
# <a name="groupattendeeconflictdata"></a>GroupAttendeeConflictData

L’élément **GroupAttendeeConflictData** contient des informations sur les conflits globaux sur le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion suggérée. 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [SuggestionsResponse](suggestionsresponse.md)
- [SuggestionDayResultArray](suggestiondayresultarray.md)
- [SuggestionDayResult](suggestiondayresult.md)
- [SuggestionArray](suggestionarray.md)
- [Suggérer](suggestion.md)
- [AttendeeConflictDataArray](attendeeconflictdataarray.md)
- [GroupAttendeeConflictData](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

**GroupAttendeeConflictData**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[NumberOfMembers](numberofmembers.md) <br/> |Représente le nombre d’utilisateurs, de ressources et de salles dans une liste de distribution.  <br/> |
|[NumberOfMembersAvailable](numberofmembersavailable.md) <br/> |Représente le nombre de membres de la liste de distribution qui sont disponibles pour une heure de réunion suggérée. Cet élément représente les membres pour lesquels l’État est **libre**.  <br/> |
|[NumberOfMembersWithConflict](numberofmemberswithconflict.md) <br/> |Représente le nombre de membres de la liste de distribution qui ont un conflit avec une heure de réunion suggérée. Cet élément représente les membres qui ont un état occupé, absent (e), **absent**( **e**) ou **provisoire** .  <br/> |
|[NumberOfMembersWithNoData](numberofmemberswithnodata.md) <br/> |Représente le nombre de membres du groupe qui n’ont pas de données de disponibilité publiées à comparer à une heure de réunion suggérée. Cet élément représente les membres d’une liste de distribution qui est trop grande ou dont les membres n’ont pas d’état de **données** .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AttendeeConflictDataArray](attendeeconflictdataarray.md) <br/> |Contient un tableau de données conflictuelles pour les participants interrogés identifiés dans l' [opération GetUserAvailability](getuseravailability-operation.md).  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **GroupAttendeeConflictData** est présent dans la réponse lorsqu’un participant de la [GetUserAvailabilityRequest](getuseravailabilityrequest.md) est résolu en une liste de distribution. L’élément **GroupAttendeeConflictData** identifie trois États pour les membres d’une liste de distribution : disponible, en conflit ou sans données. L’extension de la liste de distribution prendra en charge jusqu’à 100 membres. Par conséquent, l’élément [NumberOfMembers](numberofmembers.md) peut contenir un maximum de 100 membres. L’extension de la liste de distribution est récursive. Si une liste de distribution contient une liste de distribution enfant qui étend l’appartenance totale au parent à plus de 100 membres, la liste de distribution enfant n’est pas étendue et compte comme une seule entrée du nombre d’éléments [NumberOfMembersWithNoData](numberofmemberswithnodata.md) . Si une liste de distribution enfant peut être étendue et que l’appartenance au groupe parent ne dépasse pas 100 membres, son appartenance est étendue et le nombre de membres est ajouté aux éléments enfants de l’élément **GroupAttendeeConflictData** . 
  
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

