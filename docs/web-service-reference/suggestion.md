---
title: Suggérer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Suggestion
api_type:
- schema
ms.assetid: 040a5c8f-b62f-4d1d-9d2c-dc3c5e01481f
description: L’élément suggestion représente une seule suggestion de réunion.
ms.openlocfilehash: 25821abd5463ddba86a487709c8d2f8d928a94cc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530379"
---
# <a name="suggestion"></a><span data-ttu-id="2aa55-103">Suggérer</span><span class="sxs-lookup"><span data-stu-id="2aa55-103">Suggestion</span></span>

<span data-ttu-id="2aa55-104">L’élément **suggestion** représente une seule suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="2aa55-104">The **Suggestion** element represents a single meeting suggestion.</span></span> 
  
[<span data-ttu-id="2aa55-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2aa55-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="2aa55-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="2aa55-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="2aa55-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="2aa55-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="2aa55-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="2aa55-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="2aa55-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="2aa55-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="2aa55-110">Suggérer</span><span class="sxs-lookup"><span data-stu-id="2aa55-110">Suggestion</span></span>](suggestion.md)
  
```xml
<Suggestion>
   <MeetingTime>...</MeetingTime>
   <IsWorkTime>...</IsWorkTime>
   <SuggestionQuality>...</SuggestionQuality>
   <AttendeeConflictDataArray>...</AttendeeConflictDataArray>
</Suggestion>
```

 <span data-ttu-id="2aa55-111">**Suggérer**</span><span class="sxs-lookup"><span data-stu-id="2aa55-111">**Suggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2aa55-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2aa55-112">Attributes and elements</span></span>

<span data-ttu-id="2aa55-113">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2aa55-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2aa55-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="2aa55-114">Attributes</span></span>

<span data-ttu-id="2aa55-115">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2aa55-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2aa55-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2aa55-116">Child elements</span></span>

|<span data-ttu-id="2aa55-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2aa55-117">**Element**</span></span>|<span data-ttu-id="2aa55-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="2aa55-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2aa55-119">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="2aa55-119">MeetingTime</span></span>](meetingtime.md) <br/> |<span data-ttu-id="2aa55-120">Représente une suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="2aa55-120">Represents a suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="2aa55-121">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="2aa55-121">IsWorkTime</span></span>](isworktime.md) <br/> |<span data-ttu-id="2aa55-122">Indique si l’heure de la réunion suggérée se produit pendant les heures de travail prévues.</span><span class="sxs-lookup"><span data-stu-id="2aa55-122">Represents whether the suggested meeting time occurs during scheduled work hours.</span></span>  <br/> |
|[<span data-ttu-id="2aa55-123">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="2aa55-123">SuggestionQuality</span></span>](suggestionquality.md) <br/> |<span data-ttu-id="2aa55-124">Représente la qualité de la réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="2aa55-124">Represents the quality of the suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="2aa55-125">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="2aa55-125">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="2aa55-126">Contient un tableau d’informations décrivant les conflits entre les utilisateurs et les ressources et l’heure de la réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="2aa55-126">Contains an array of information that describes conflicts between users and resources and the suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2aa55-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2aa55-127">Parent elements</span></span>

|<span data-ttu-id="2aa55-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2aa55-128">**Element**</span></span>|<span data-ttu-id="2aa55-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="2aa55-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2aa55-130">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="2aa55-130">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="2aa55-131">Contient un tableau des heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="2aa55-131">Contains an array of suggested meeting times.</span></span>  <br/> <span data-ttu-id="2aa55-132">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="2aa55-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2aa55-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="2aa55-133">Remarks</span></span>

<span data-ttu-id="2aa55-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2aa55-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2aa55-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2aa55-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2aa55-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2aa55-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2aa55-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2aa55-137">Schema Name</span></span>  <br/> |<span data-ttu-id="2aa55-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2aa55-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="2aa55-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2aa55-139">Validation File</span></span>  <br/> |<span data-ttu-id="2aa55-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2aa55-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2aa55-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2aa55-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="2aa55-142">False</span><span class="sxs-lookup"><span data-stu-id="2aa55-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2aa55-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2aa55-143">See also</span></span>



[<span data-ttu-id="2aa55-144">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2aa55-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="2aa55-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2aa55-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="2aa55-146">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="2aa55-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

