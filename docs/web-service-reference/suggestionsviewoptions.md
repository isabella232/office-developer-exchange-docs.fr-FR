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
# <a name="suggestionsviewoptions"></a><span data-ttu-id="1d1bb-103">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="1d1bb-103">SuggestionsViewOptions</span></span>

<span data-ttu-id="1d1bb-104">L’élément **SuggestionsViewOptions** contient les options permettant d’obtenir des informations de suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-104">The **SuggestionsViewOptions** element contains the options for obtaining meeting suggestion information.</span></span> 
  
[<span data-ttu-id="1d1bb-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="1d1bb-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="1d1bb-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="1d1bb-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
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

 <span data-ttu-id="1d1bb-107">**SuggestionsViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="1d1bb-107">**SuggestionsViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d1bb-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1d1bb-108">Attributes and elements</span></span>

<span data-ttu-id="1d1bb-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d1bb-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="1d1bb-110">Attributes</span></span>

<span data-ttu-id="1d1bb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d1bb-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1d1bb-112">Child elements</span></span>

|<span data-ttu-id="1d1bb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1d1bb-113">**Element**</span></span>|<span data-ttu-id="1d1bb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1d1bb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d1bb-115">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="1d1bb-115">GoodThreshold</span></span>](goodthreshold.md) <br/> |<span data-ttu-id="1d1bb-116">Indique le pourcentage des participants qui doivent ouvrir la période de temps pour la période de temps être considérée comme une heure de réunion proposée bonne.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-116">Specifies the percentage of attendees that must have the time period open for the time period to qualify as a good suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="1d1bb-117">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="1d1bb-117">MaximumResultsByDay</span></span>](maximumresultsbyday.md) <br/> |<span data-ttu-id="1d1bb-118">Spécifie le nombre de répétitions de réunion proposée par jour retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-118">Specifies the number of suggested meeting times per day returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="1d1bb-119">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="1d1bb-119">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md) <br/> |<span data-ttu-id="1d1bb-120">Spécifie le nombre de suggestions de résultats pour les réunions planifiées en dehors des heures de travail normal par jour.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-120">Specifies the number of suggested results for meeting times outside regular working hours per day.</span></span>  <br/> |
|[<span data-ttu-id="1d1bb-121">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="1d1bb-121">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md) <br/> |<span data-ttu-id="1d1bb-122">Spécifie la longueur de la réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-122">Specifies the length of the meeting to be suggested.</span></span>  <br/> |
|[<span data-ttu-id="1d1bb-123">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="1d1bb-123">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md) <br/> |<span data-ttu-id="1d1bb-124">Spécifie la qualité des suggestions de réunion à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-124">Specifies the quality of meeting suggestions to be returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="1d1bb-125">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="1d1bb-125">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="1d1bb-126">Identifie l’intervalle de temps qui est interrogé pour des informations détaillées sur les heures de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-126">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="1d1bb-127">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="1d1bb-127">CurrentMeetingTime</span></span>](currentmeetingtime.md) <br/> |<span data-ttu-id="1d1bb-128">Résultats du temps représente l’heure de début d’une réunion que vous souhaitez mettre à jour avec la réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-128">Represents the start time of a meeting that you want to update with the suggested meeting time results.</span></span>  <br/> |
|[<span data-ttu-id="1d1bb-129">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="1d1bb-129">GlobalObjectId</span></span>](globalobjectid.md) <br/> |<span data-ttu-id="1d1bb-130">Cet élément n’est pas utilisé.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-130">This element is not used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d1bb-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1d1bb-131">Parent elements</span></span>

|<span data-ttu-id="1d1bb-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1d1bb-132">**Element**</span></span>|<span data-ttu-id="1d1bb-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="1d1bb-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d1bb-134">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="1d1bb-134">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="1d1bb-135">Contient les arguments utilisés pour obtenir des informations de disponibilité d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-135">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="1d1bb-136">Il s’agit d’un élément racine.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-136">This is a root element.</span></span>  <br/> <span data-ttu-id="1d1bb-137">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="1d1bb-137">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1d1bb-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="1d1bb-138">Remarks</span></span>

<span data-ttu-id="1d1bb-139">Cet élément n’est pas obligatoire et peut se produire seulement une seule fois en cas d’utilisation.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-139">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="1d1bb-140">Cette valeur peut être nulle si la valeur de l’élément [FreeBusyViewOptions](freebusyviewoptions.md) n’est pas nulle.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-140">This value can be null if the value of the [FreeBusyViewOptions](freebusyviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1d1bb-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1d1bb-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="1d1bb-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1d1bb-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d1bb-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1d1bb-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1d1bb-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1d1bb-144">Schema Name</span></span>  <br/> |<span data-ttu-id="1d1bb-145">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1d1bb-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="1d1bb-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1d1bb-146">Validation File</span></span>  <br/> |<span data-ttu-id="1d1bb-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1d1bb-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1d1bb-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1d1bb-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d1bb-149">False</span><span class="sxs-lookup"><span data-stu-id="1d1bb-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d1bb-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1d1bb-150">See also</span></span>



[<span data-ttu-id="1d1bb-151">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="1d1bb-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="1d1bb-152">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="1d1bb-152">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

