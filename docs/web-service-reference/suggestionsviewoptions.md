---
title: SuggestionsViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionsViewOptions
api_type:
- schema
ms.assetid: bb04ae38-e62d-4a69-a479-8ff326ca726e
description: L’élément SuggestionsViewOptions contient les options permettant d’obtenir des informations de suggestion de réunion.
ms.openlocfilehash: 09ff317ae0b2ebf1eadc89dc3bb1cf5b3ae19dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838651"
---
# <a name="suggestionsviewoptions"></a>SuggestionsViewOptions

L’élément **SuggestionsViewOptions** contient les options permettant d’obtenir des informations de suggestion de réunion. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
```xml
<SuggestionsViewOptions>
   <GoodThreshold>...</GoodThreshold>
   <MaximumResultsByDay>...</MaximumResultsByDay>
   <MaximumNonWorkingHourResultsByDay>...</MaximumNonWorkingHourResultsByDay>
   <MeetingDurationInMinutes>...</MeetingDurationInMinutes>
   <MinimumSuggestionQuality>...</MinimumSuggestionQuality>
   <SuggestionIntervalInMinutes>...</SuggestionIntervalInMinutes>
   <DetailedSuggestionsWindow>...</DetailedSuggestionsWindow>
   <CurrentMeetingTime>...</CurrentMeetingTime>
   <GlobalObjectId>...</GlobalObjectId>
</SuggestionsViewOptions>
```

 **SuggestionsViewOptionsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[GoodThreshold](goodthreshold.md) <br/> |Indique le pourcentage des participants qui doivent ouvrir la période de temps pour la période de temps être considérée comme une heure de réunion proposée bonne.  <br/> |
|[MaximumResultsByDay](maximumresultsbyday.md) <br/> |Spécifie le nombre de répétitions de réunion proposée par jour retourné dans la réponse.  <br/> |
|[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md) <br/> |Spécifie le nombre de suggestions de résultats pour les réunions planifiées en dehors des heures de travail normal par jour.  <br/> |
|[MeetingDurationInMinutes](meetingdurationinminutes.md) <br/> |Spécifie la longueur de la réunion suggérée.  <br/> |
|[MinimumSuggestionQuality](minimumsuggestionquality.md) <br/> |Spécifie la qualité des suggestions de réunion à renvoyer dans la réponse.  <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifie l’intervalle de temps qui est interrogé pour des informations détaillées sur les heures de réunion suggérée.  <br/> |
|[CurrentMeetingTime](currentmeetingtime.md) <br/> |Résultats du temps représente l’heure de début d’une réunion que vous souhaitez mettre à jour avec la réunion proposée.  <br/> |
|[GlobalObjectId](globalobjectid.md) <br/> |Cet élément n’est pas utilisé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contient les arguments utilisés pour obtenir des informations de disponibilité d’utilisateur. Il s’agit d’un élément racine.  <br/> Vous trouverez ci-dessous le XPath pour cet élément :  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas obligatoire et peut se produire seulement une seule fois en cas d’utilisation. Cette valeur peut être nulle si la valeur de l’élément [FreeBusyViewOptions](freebusyviewoptions.md) n’est pas nulle. 
  
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

