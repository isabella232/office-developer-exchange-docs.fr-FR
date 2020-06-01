---
title: MaximumNonWorkHourResultsByDay
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaximumNonWorkHourResultsByDay
api_type:
- schema
ms.assetid: 9fb7314d-779c-4b1f-9d7c-b5cb092ed134
description: L’élément MaximumNonWorkHourResultsByDay spécifie le nombre de résultats suggérés pour les heures de travail en dehors des heures ouvrées normales par jour.
ms.openlocfilehash: 410d6bd84838d979af6bc53ca47f445ae55a09e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465498"
---
# <a name="maximumnonworkhourresultsbyday"></a>MaximumNonWorkHourResultsByDay

L’élément **MaximumNonWorkHourResultsByDay** spécifie le nombre de résultats suggérés pour les heures de travail en dehors des heures ouvrées normales par jour. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md)
  
```xml
<MaximumNonWorkHourResultsByDay>...</MaximumNonWorkHourResultsByDay>
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
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Contient les options permettant d’obtenir des informations sur les suggestions de réunion.  <br/> Voici le XPath de cet élément :  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur texte représente un entier.
  
## <a name="remarks"></a>Remarques

Cet élément est requis si l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé. 
  
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

