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
description: L’élément SuggestionsViewOptions contient les options permettant d’obtenir des informations sur les suggestions de réunion.
ms.openlocfilehash: f584b19997f98760bd4e438dcd48a5c18cc63e4b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44433993"
---
# <a name="suggestionsviewoptions"></a>SuggestionsViewOptions

L’élément **SuggestionsViewOptions** contient les options permettant d’obtenir des informations sur les suggestions de réunion. 
  
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
|[GoodThreshold](goodthreshold.md) <br/> |Spécifie le pourcentage de participants qui doivent avoir ouvert la période de temps pour la période considérée comme une heure de réunion recommandée.  <br/> |
|[MaximumResultsByDay](maximumresultsbyday.md) <br/> |Indique le nombre de réunions suggérées par jour renvoyées dans la réponse.  <br/> |
|[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md) <br/> |Indique le nombre de résultats suggérés pour les heures de travail en dehors des heures ouvrées normales par jour.  <br/> |
|[MeetingDurationInMinutes](meetingdurationinminutes.md) <br/> |Spécifie la durée de la réunion à suggérer.  <br/> |
|[MinimumSuggestionQuality](minimumsuggestionquality.md) <br/> |Spécifie la qualité des suggestions de réunion à renvoyer dans la réponse.  <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |Identifie l’intervalle de temps interrogé pour obtenir des informations détaillées sur les heures de réunion suggérées.  <br/> |
|[CurrentMeetingTime](currentmeetingtime.md) <br/> |Représente l’heure de début d’une réunion que vous souhaitez mettre à jour avec les résultats de la réunion suggérés.  <br/> |
|[GlobalObjectId](globalobjectid.md) <br/> |Cet élément n’est pas utilisé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |Contient les arguments utilisés pour obtenir les informations de disponibilité de l’utilisateur. Il s’agit d’un élément racine.  <br/> Voici le XPath de cet élément :  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas obligatoire et ne peut se produire qu’une seule fois s’il est utilisé. Cette valeur peut être null si la valeur de l’élément [FreeBusyViewOptions](freebusyviewoptions.md) n’est pas null. 
  
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

