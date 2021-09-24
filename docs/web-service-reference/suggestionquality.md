---
title: SuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SuggestionQuality
api_type:
- schema
ms.assetid: 734f1a58-adda-4830-973e-e84bf7b870d5
description: L’élément SuggestionQuality représente la qualité de l’heure de réunion suggérée.
ms.openlocfilehash: 4d8a504e60e8f043bfb120080a89733e78b16b9e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531551"
---
# <a name="suggestionquality"></a>SuggestionQuality

**L’élément SuggestionQuality** représente la qualité de l’heure de réunion suggérée. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
[SuggestionDayResultArray](suggestiondayresultarray.md)
  
[SuggestionDayResult](suggestiondayresult.md)
  
[SuggestionArray](suggestionarray.md)
  
[Suggestion](suggestion.md)
  
[SuggestionQuality](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 **SuggestionQuality**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Suggestion](suggestion.md) <br/> |Représente une suggestion d’heure de réunion unique.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une **valeur SuggestionQuality** est requise. Les valeurs possibles sont les suivantes : 
  
- **D’excellents** 100 % des utilisateurs et des ressources sont disponibles pour l’heure de réunion suggérée. 
    
- **Bon** Le pourcentage minimal d’utilisateurs et de ressources disponibles est supérieur ou égal à la valeur de l’élément [GoodThreshold](goodthreshold.md) plus 50. 
    
- **Fair** Le pourcentage maximal d’utilisateurs et de ressources disponibles pour une heure de réunion suggérée est égal à la valeur de l’élément [GoodThreshold](goodthreshold.md) plus 50. La valeur minimale pour une heure **de** réunion de qualité équitable est de 50 %. 
    
- **Médiocre** Moins de 50 % des utilisateurs et des ressources sont disponibles pour l’heure de réunion suggérée. 
    
## <a name="remarks"></a>Remarques

Le **type SuggestionQuality** est également le type pour les éléments [DayQuality](dayquality.md) et [MinimumSuggestionQuality.](minimumsuggestionquality.md) 
  
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

