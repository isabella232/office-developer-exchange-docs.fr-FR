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
description: L’élément SuggestionQuality représente la qualité de l’heure de réunion proposée.
ms.openlocfilehash: e67e0149226b36c22cdd00acd78f6582f826dd3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838648"
---
# <a name="suggestionquality"></a>SuggestionQuality

L’élément **SuggestionQuality** représente la qualité de l’heure de réunion proposée. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Suggestion](suggestion.md) <br/> |Représente une seule suggestion de l’heure de la réunion.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente une valeur **SuggestionQuality** est requise. Les valeurs possibles sont les suivantes : 
  
- **Excellent** 100 % des utilisateurs et des ressources sont disponibles pour l’heure de réunion proposée. 
    
- **Une bonne** Le pourcentage minimal d’utilisateurs et des ressources disponibles est égale ou supérieure à la valeur de l’élément [GoodThreshold](goodthreshold.md) plus de 50. 
    
- **Juste** Le pourcentage maximal d’utilisateurs et les ressources disponibles pour une heure de réunion proposée est égal à la valeur de l’élément [GoodThreshold](goodthreshold.md) plus de 50. La valeur minimale pour une heure de réunion qualité **juste** est de 50 pour cent. 
    
- **Une mauvaise** Inférieur à 50 % des utilisateurs et des ressources sont disponibles pour l’heure de réunion proposée. 
    
## <a name="remarks"></a>Remarques

Le type **SuggestionQuality** est également le type de la [DayQuality](dayquality.md) et les éléments [MinimumSuggestionQuality](minimumsuggestionquality.md) . 
  
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

