---
title: NumberOfMembers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- NumberOfMembers
api_type:
- schema
ms.assetid: 845fb877-de49-4e26-8885-6f026edd9ee9
description: L’élément NumberOfMembers représente le nombre d’utilisateurs, de ressources et de salles dans une liste de distribution.
ms.openlocfilehash: d1a0f2afc1935f846dbe3d5ce1ba4385cf3cf8dd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529786"
---
# <a name="numberofmembers"></a>NumberOfMembers

**L’élément NumberOfMembers** représente le nombre d’utilisateurs, de ressources et de salles dans une liste de distribution. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
[SuggestionDayResultArray](suggestiondayresultarray.md)
  
[SuggestionDayResult](suggestiondayresult.md)
  
[SuggestionArray](suggestionarray.md)
  
[Suggestion](suggestion.md)
  
[AttendeeConflictDataArray](attendeeconflictdataarray.md)
  
[GroupAttendeeConflictData](groupattendeeconflictdata.md)
  
[NumberOfMembers](numberofmembers.md)
  
```xml
<NumberOfMembers>...</NumberOfMembers>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GroupAttendeeConflictData](groupattendeeconflictdata.md) <br/> |Contient des informations de conflit agrégées sur le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui ne disposent pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion suggérée.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a>Remarques

La valeur maximale de **l’élément NumberOfMembers** est 100. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
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

