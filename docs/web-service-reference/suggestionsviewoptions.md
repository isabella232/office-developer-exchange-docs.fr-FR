---
title: SuggestionsViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SuggestionsViewOptions
api_type:
- schema
ms.assetid: bb04ae38-e62d-4a69-a479-8ff326ca726e
description: L’élément SuggestionsViewOptions contient les options pour obtenir des informations de suggestion de réunion.
ms.openlocfilehash: ba3591b88e581d45c811100a53b0a74e4bb8e010
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522613"
---
# <a name="suggestionsviewoptions"></a>SuggestionsViewOptions

**L’élément SuggestionsViewOptions** contient les options pour obtenir des informations de suggestion de réunion. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[GoodThreshold](goodthreshold.md) <br/> |Spécifie le pourcentage de participants dont la période doit être ouverte pour la période afin d’être éligible en tant qu’heure de réunion suggérée.  <br/> |
|[MaximumResultsByDay](maximumresultsbyday.md) <br/> |Spécifie le nombre de suggestions d’heures de réunion par jour renvoyées dans la réponse.  <br/> |
|[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md) <br/> |Spécifie le nombre de résultats suggérés pour les heures de réunion en dehors des heures de travail normales par jour.  <br/> |
|[MeetingDurationInMinutes](meetingdurationinminutes.md) <br/> |Spécifie la durée de la réunion à suggérer.  <br/> |
|[MinimumSuggestionQuality](minimumsuggestionquality.md) <br/> |Spécifie la qualité des suggestions de réunion à retourner dans la réponse.  <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifie l’étendue de temps à interroger pour obtenir des informations détaillées sur les heures de réunion suggérées.  <br/> |
|[CurrentMeetingTime](currentmeetingtime.md) <br/> |Représente l’heure de début d’une réunion que vous souhaitez mettre à jour avec les résultats de l’heure de réunion suggérés.  <br/> |
|[GlobalObjectId](globalobjectid.md) <br/> |Cet élément n’est pas utilisé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contient les arguments utilisés pour obtenir les informations de disponibilité de l’utilisateur. Il s’agit d’un élément racine.  <br/> Voici le chemin d’accès XPath à cet élément :  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas obligatoire et ne peut se produire qu’une seule fois s’il est utilisé. Cette valeur peut être null si la valeur de [l’élément FreeBusyViewOptions](freebusyviewoptions.md) n’est pas null. 
  
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

