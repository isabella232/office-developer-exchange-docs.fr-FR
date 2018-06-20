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
description: L’élément GroupAttendeeConflictData contient des informations de conflit agrégation sur le nombre d’utilisateurs qui sont disponible, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une distribution de liste pour un suggérés heure de la réunion.
ms.openlocfilehash: 382b4d866c95de98bd444cd6226d71813889d4f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827757"
---
# <a name="groupattendeeconflictdata"></a>GroupAttendeeConflictData

L’élément **GroupAttendeeConflictData** contient des informations de conflit agrégation sur le nombre d’utilisateurs qui sont disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion proposée. 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [SuggestionsResponse](suggestionsresponse.md)
- [SuggestionDayResultArray](suggestiondayresultarray.md)
- [SuggestionDayResult](suggestiondayresult.md)
- [SuggestionArray](suggestionarray.md)
- [Suggestion](suggestion.md)
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[NumberOfMembers](numberofmembers.md) <br/> |Représente le nombre d’utilisateurs, des ressources et des salles dans une liste de distribution.  <br/> |
|[NumberOfMembersAvailable](numberofmembersavailable.md) <br/> |Représente le nombre de membres de liste de distribution qui sont disponibles pour une heure de réunion proposée. Cet élément représente des membres pour lesquels l’état est **disponible**.  <br/> |
|[NumberOfMembersWithConflict](numberofmemberswithconflict.md) <br/> |Représente le nombre de membres de liste de distribution qui ont un conflit avec une heure de réunion proposée. Cet élément représente des membres qui ont l’état **occupé (e)**, **absent du bureau**ou **provisoire** .  <br/> |
|[NumberOfMembersWithNoData](numberofmemberswithnodata.md) <br/> |Représente le nombre de membres du groupe qui n’ont pas de données et de disponibilité publiées à comparer à une heure de réunion proposée. Cet élément représente les membres d’une liste de distribution est trop grande ou qui ont l’état **Aucune donnée** .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AttendeeConflictDataArray](attendeeconflictdataarray.md) <br/> |Contient un tableau de données de conflit pour les participants interrogées identifiés dans l' [opération GetUserAvailability](getuseravailability-operation.md).  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **GroupAttendeeConflictData** est présent dans la réponse lorsqu’un participant dans la [GetUserAvailabilityRequest](getuseravailabilityrequest.md) est résolu en une liste de distribution. L’élément **GroupAttendeeConflictData** identifie les trois états de membres d’une liste de distribution : disponible, en conflit, ou aucune donnée. Développement de listes de distribution prendront en charge jusqu'à 100 membres. Par conséquent, l’élément [NumberOfMembers](numberofmembers.md) peut contenir un maximum de 100 membres. Développement de listes de distribution est récursive. Si une liste de distribution contient une liste de distribution enfants qui développe l’appartenance total parent à plus de 100 membres, la liste de distribution enfants n’est pas développée et comptera comme une seule entrée du nombre d’éléments [NumberOfMembersWithNoData](numberofmemberswithnodata.md) . Si une liste de distribution enfants peut être développée et l’appartenance parent total ne développe pas plus de 100 membres, son appartenance est développé et les nombres de membres sont ajoutées pour les éléments enfants de l’élément **GroupAttendeeConflictData** . 
  
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

