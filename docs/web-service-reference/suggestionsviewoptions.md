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
# <a name="suggestionsviewoptions"></a><span data-ttu-id="f9272-103">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="f9272-103">SuggestionsViewOptions</span></span>

<span data-ttu-id="f9272-104">L’élément **SuggestionsViewOptions** contient les options permettant d’obtenir des informations sur les suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="f9272-104">The **SuggestionsViewOptions** element contains the options for obtaining meeting suggestion information.</span></span> 
  
[<span data-ttu-id="f9272-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="f9272-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="f9272-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="f9272-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
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

 <span data-ttu-id="f9272-107">**SuggestionsViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="f9272-107">**SuggestionsViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9272-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f9272-108">Attributes and elements</span></span>

<span data-ttu-id="f9272-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f9272-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9272-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="f9272-110">Attributes</span></span>

<span data-ttu-id="f9272-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f9272-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9272-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f9272-112">Child elements</span></span>

|<span data-ttu-id="f9272-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f9272-113">**Element**</span></span>|<span data-ttu-id="f9272-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f9272-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9272-115">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="f9272-115">GoodThreshold</span></span>](goodthreshold.md) <br/> |<span data-ttu-id="f9272-116">Spécifie le pourcentage de participants qui doivent avoir ouvert la période de temps pour la période considérée comme une heure de réunion recommandée.</span><span class="sxs-lookup"><span data-stu-id="f9272-116">Specifies the percentage of attendees that must have the time period open for the time period to qualify as a good suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="f9272-117">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="f9272-117">MaximumResultsByDay</span></span>](maximumresultsbyday.md) <br/> |<span data-ttu-id="f9272-118">Indique le nombre de réunions suggérées par jour renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="f9272-118">Specifies the number of suggested meeting times per day returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="f9272-119">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="f9272-119">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md) <br/> |<span data-ttu-id="f9272-120">Indique le nombre de résultats suggérés pour les heures de travail en dehors des heures ouvrées normales par jour.</span><span class="sxs-lookup"><span data-stu-id="f9272-120">Specifies the number of suggested results for meeting times outside regular working hours per day.</span></span>  <br/> |
|[<span data-ttu-id="f9272-121">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="f9272-121">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md) <br/> |<span data-ttu-id="f9272-122">Spécifie la durée de la réunion à suggérer.</span><span class="sxs-lookup"><span data-stu-id="f9272-122">Specifies the length of the meeting to be suggested.</span></span>  <br/> |
|[<span data-ttu-id="f9272-123">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="f9272-123">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md) <br/> |<span data-ttu-id="f9272-124">Spécifie la qualité des suggestions de réunion à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="f9272-124">Specifies the quality of meeting suggestions to be returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="f9272-125">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="f9272-125">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="f9272-126">Identifie l’intervalle de temps interrogé pour obtenir des informations détaillées sur les heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="f9272-126">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="f9272-127">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="f9272-127">CurrentMeetingTime</span></span>](currentmeetingtime.md) <br/> |<span data-ttu-id="f9272-128">Représente l’heure de début d’une réunion que vous souhaitez mettre à jour avec les résultats de la réunion suggérés.</span><span class="sxs-lookup"><span data-stu-id="f9272-128">Represents the start time of a meeting that you want to update with the suggested meeting time results.</span></span>  <br/> |
|[<span data-ttu-id="f9272-129">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="f9272-129">GlobalObjectId</span></span>](globalobjectid.md) <br/> |<span data-ttu-id="f9272-130">Cet élément n’est pas utilisé.</span><span class="sxs-lookup"><span data-stu-id="f9272-130">This element is not used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f9272-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f9272-131">Parent elements</span></span>

|<span data-ttu-id="f9272-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f9272-132">**Element**</span></span>|<span data-ttu-id="f9272-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="f9272-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9272-134">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="f9272-134">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="f9272-135">Contient les arguments utilisés pour obtenir les informations de disponibilité de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="f9272-135">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="f9272-136">Il s’agit d’un élément racine.</span><span class="sxs-lookup"><span data-stu-id="f9272-136">This is a root element.</span></span>  <br/> <span data-ttu-id="f9272-137">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="f9272-137">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9272-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="f9272-138">Remarks</span></span>

<span data-ttu-id="f9272-139">Cet élément n’est pas obligatoire et ne peut se produire qu’une seule fois s’il est utilisé.</span><span class="sxs-lookup"><span data-stu-id="f9272-139">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="f9272-140">Cette valeur peut être null si la valeur de l’élément [FreeBusyViewOptions](freebusyviewoptions.md) n’est pas null.</span><span class="sxs-lookup"><span data-stu-id="f9272-140">This value can be null if the value of the [FreeBusyViewOptions](freebusyviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f9272-141">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f9272-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f9272-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f9272-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9272-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f9272-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9272-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f9272-144">Schema Name</span></span>  <br/> |<span data-ttu-id="f9272-145">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f9272-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="f9272-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f9272-146">Validation File</span></span>  <br/> |<span data-ttu-id="f9272-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f9272-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9272-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f9272-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="f9272-149">False</span><span class="sxs-lookup"><span data-stu-id="f9272-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9272-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f9272-150">See also</span></span>



[<span data-ttu-id="f9272-151">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f9272-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="f9272-152">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="f9272-152">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

