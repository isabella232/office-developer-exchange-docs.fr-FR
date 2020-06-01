---
title: SuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionQuality
api_type:
- schema
ms.assetid: 734f1a58-adda-4830-973e-e84bf7b870d5
description: L’élément SuggestionQuality représente la qualité de l’heure de la réunion suggérée.
ms.openlocfilehash: 3f8c15ccabd03687dc386a0328020cbc0bc802c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457976"
---
# <a name="suggestionquality"></a>SuggestionQuality

L’élément **SuggestionQuality** représente la qualité de l’heure de la réunion suggérée. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
[SuggestionDayResultArray](suggestiondayresultarray.md)
  
[SuggestionDayResult](suggestiondayresult.md)
  
[SuggestionArray](suggestionarray.md)
  
[Suggérer](suggestion.md)
  
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
|[Suggérer](suggestion.md) <br/> |Représente une seule suggestion de temps de réunion.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une valeur **SuggestionQuality** est requise. Les valeurs possibles sont les suivantes : 
  
- Un **excellent** pourcentage de 100 pour cent des utilisateurs et des ressources est disponible pour la réunion suggérée. 
    
- **Utile** Le pourcentage minimal d’utilisateurs et de ressources disponibles est supérieur ou égal à la valeur de l’élément [GoodThreshold](goodthreshold.md) plus 50. 
    
- **Équitable** Le pourcentage maximal d’utilisateurs et de ressources disponibles pour une heure de réunion suggérée est égal à la valeur de l’élément [GoodThreshold](goodthreshold.md) plus 50. La valeur minimale pour un temps de réunion de qualité **équitable** est de 50%. 
    
- **Médiocre** Moins de 50% des utilisateurs et des ressources sont disponibles pour la réunion suggérée. 
    
## <a name="remarks"></a>Remarques

Le type **SuggestionQuality** est également le type pour les éléments [DayQuality](dayquality.md) et [MinimumSuggestionQuality](minimumsuggestionquality.md) . 
  
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

