---
title: NumberOfMembersWithNoData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- NumberOfMembersWithNoData
api_type:
- schema
ms.assetid: 7ca9c57c-9519-442c-a9f4-dca2b0309716
description: L’élément NumberOfMembersWithNoData représente le nombre de membres de la liste de distribution qui n’ont pas publié de données de libre/occupé à comparer à une heure de réunion suggérée. Cet élément représente les membres d’une liste de distribution trop grande ou les membres qui n’ont pas l’état Aucune donnée.
ms.openlocfilehash: 4b021ce75a84eca3e1b5a66cf51f6b5d7adec86b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529684"
---
# <a name="numberofmemberswithnodata"></a>NumberOfMembersWithNoData

**L’élément NumberOfMembersWithNoData** représente le nombre de membres de la liste de distribution qui n’ont pas publié de données de libre/occupé à comparer à une heure de réunion suggérée. Cet élément représente les membres d’une liste de distribution trop grande ou les membres qui n’ont **pas l’état Aucune** donnée. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
[SuggestionDayResultArray](suggestiondayresultarray.md)
  
[SuggestionDayResult](suggestiondayresult.md)
  
[SuggestionArray](suggestionarray.md)
  
[Suggestion](suggestion.md)
  
[AttendeeConflictDataArray](attendeeconflictdataarray.md)
  
[GroupAttendeeConflictData](groupattendeeconflictdata.md)
  
[NumberOfMembersWithNoData](numberofmemberswithnodata.md)
  
```xml
<NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
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
|[GroupAttendeeConflictData](groupattendeeconflictdata.md) <br/> |Contient des informations de conflit agrégées sur le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion suggérée.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a>Remarques

Un contact d’un groupe qui n’a pas de boîte aux lettres est un exemple de membre de liste de distribution qui ne comprend pas de données de calendrier. Un contact peut également ne pas avoir **le statut Aucune** donnée pour les raisons suivantes : 
  
- Les autorisations sont insuffisantes.
    
- La liste de distribution est trop grande pour être étendue.
    
- Le service d’annuaire Active Directory n’est pas disponible.
    
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

