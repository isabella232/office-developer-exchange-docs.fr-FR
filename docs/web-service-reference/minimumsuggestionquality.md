---
title: MinimumSuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MinimumSuggestionQuality
api_type:
- schema
ms.assetid: 3725cbd4-9bc1-4f7d-8929-b2c68cb46114
description: L’élément MinimumSuggestionQuality définit la qualité des suggestions de réunion à renvoyer dans la réponse.
ms.openlocfilehash: ac79682bd761f678f23fc2d698a50fd7704f6fab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828468"
---
# <a name="minimumsuggestionquality"></a>MinimumSuggestionQuality

L’élément **MinimumSuggestionQuality** définit la qualité des suggestions de réunion à renvoyer dans la réponse. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[MinimumSuggestionQuality](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
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
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Contient les options permettant d’obtenir des informations de suggestion de réunion.  <br/> Vous trouverez ci-dessous le XPath pour cet élément :  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Le tableau suivant répertorie les valeurs possibles de cet élément :
  
|**Valeur**|**Description**|
|:-----|:-----|
|**Excellente** <br/> |0 % des participants ont un conflit avec l’heure de réunion proposée.  <br/> |
|**Une bonne** <br/> |Le pourcentage est considérée comme bonne est défini à l’aide de l’élément [GoodThreshold](goodthreshold.md) .  <br/> |
|**Juste** <br/> |Le pourcentage est considéré comme étant juste est défini à l’aide de l’élément [GoodThreshold](goodthreshold.md) .  <br/> |
|**Une mauvaise** <br/> |50 % ou plus des participants ont un conflit avec l’heure de réunion proposée.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est obligatoire si l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé. 
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)


[Obtention de disponibilité de l’utilisateur](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

