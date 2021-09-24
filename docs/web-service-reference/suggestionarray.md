---
title: SuggestionArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SuggestionArray
api_type:
- schema
ms.assetid: c1c26008-7b14-4563-8db5-bceb0f475b1b
description: L’élément SuggestionArray contient un tableau de suggestions de réunion.
ms.openlocfilehash: 60b7f02915c609e108136957511dfe42717344f9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531575"
---
# <a name="suggestionarray"></a>SuggestionArray

**L’élément SuggestionArray** contient un tableau de suggestions de réunion. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
[SuggestionDayResultArray](suggestiondayresultarray.md)
  
[SuggestionDayResult](suggestiondayresult.md)
  
[SuggestionArray](suggestionarray.md)
  
```xml
<SuggestionArray>
   <Suggestion>...</Suggestion>
</SuggestionArray>
```

 **ArrayOfSuggestion**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Suggestion](suggestion.md) <br/> |Représente une suggestion de réunion unique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SuggestionDayResult](suggestiondayresult.md) <br/> |Représente un jour unique qui contient des heures de réunion suggérées.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="remarks"></a>Remarques

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

