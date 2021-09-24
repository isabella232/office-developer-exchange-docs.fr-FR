---
title: GoodThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GoodThreshold
api_type:
- schema
ms.assetid: 68f607f5-7271-46a6-8ffc-91878185a683
description: L’élément GoodThreshold spécifie le pourcentage de participants dont la période doit être ouverte afin que la période soit éligible en tant qu’heure de réunion suggérée.
ms.openlocfilehash: bec5159b46a350cb01f8d573c68e1925aeb40ac9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533219"
---
# <a name="goodthreshold"></a>GoodThreshold

**L’élément GoodThreshold** spécifie le pourcentage de participants dont la période doit être ouverte afin que la période soit éligible en tant qu’heure de réunion suggérée. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[GoodThreshold](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
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
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Contient les options pour obtenir des informations sur les suggestions de réunion.  <br/> Voici le chemin d’accès XPath à cet élément :  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Les valeurs d’unger attendues sont entre 0 et 50.
  
## <a name="remarks"></a>Remarques

Cet élément est requis si [l’élément SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé. **L’élément GoodThreshold** détermine également quelles réunions sont considérées comme équitables. Il s’agit du pourcentage de participants en conflit inférieur au bon seuil et supérieur à 50 %, l’heure de réunion suggérée est qualifiée d’équitable. Le bon seuil plus 50 est égal au pourcentage qui définit le seuil Bon/Juste. 
  
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

