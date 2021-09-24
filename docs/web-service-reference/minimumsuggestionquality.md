---
title: MinimumSuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MinimumSuggestionQuality
api_type:
- schema
ms.assetid: 3725cbd4-9bc1-4f7d-8929-b2c68cb46114
description: L’élément MinimumSuggestionQuality définit la qualité des suggestions de réunion à retourner dans la réponse.
ms.openlocfilehash: c1126158f7a521fbefaf34fda906d60dd15c2af4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510931"
---
# <a name="minimumsuggestionquality"></a>MinimumSuggestionQuality

**L’élément MinimumSuggestionQuality** définit la qualité des suggestions de réunion à retourner dans la réponse. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[MinimumSuggestionQuality](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
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
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Contient les options pour obtenir des informations sur les suggestions de réunion.  <br/> Voici le chemin d’accès XPath à cet élément :  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Le tableau suivant répertorie les valeurs possibles pour cet élément :
  
|**Valeur**|**Description**|
|:-----|:-----|
|**Excellente** <br/> |0 % des participants sont en conflit avec l’heure de réunion suggérée.  <br/> |
|**Good** <br/> |Le pourcentage considéré comme étant bon est fixé à l’aide de [l’élément GoodThreshold.](goodthreshold.md)  <br/> |
|**Fair** <br/> |Le pourcentage considéré comme juste est fixé à l’aide de [l’élément GoodThreshold.](goodthreshold.md)  <br/> |
|**Mauvais** <br/> |50 % ou plus des participants sont en conflit avec l’heure de réunion suggérée.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est requis si [l’élément SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé. 
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)


[Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

