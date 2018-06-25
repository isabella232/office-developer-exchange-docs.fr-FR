---
title: MeetingTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTime
api_type:
- schema
ms.assetid: 6e6d2d8b-e8a2-43e6-a715-0fc7d6dd44b9
description: L’élément MeetingTime représente une heure de réunion proposée.
ms.openlocfilehash: 1ea79be394124431aa1279ee94d5e5c6331d377b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828435"
---
# <a name="meetingtime"></a><span data-ttu-id="cd695-103">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="cd695-103">MeetingTime</span></span>

<span data-ttu-id="cd695-104">L’élément **MeetingTime** représente une heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="cd695-104">The **MeetingTime** element represents a suggested meeting time.</span></span> 
  
[<span data-ttu-id="cd695-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cd695-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="cd695-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="cd695-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="cd695-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="cd695-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="cd695-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="cd695-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="cd695-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="cd695-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="cd695-110">Suggestion</span><span class="sxs-lookup"><span data-stu-id="cd695-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="cd695-111">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="cd695-111">MeetingTime</span></span>](meetingtime.md)
  
```xml
<MeetingTime>...</MeetingTime
```

 <span data-ttu-id="cd695-112">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="cd695-112">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd695-113">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cd695-113">Attributes and elements</span></span>

<span data-ttu-id="cd695-114">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cd695-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd695-115">Attributs</span><span class="sxs-lookup"><span data-stu-id="cd695-115">Attributes</span></span>

<span data-ttu-id="cd695-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cd695-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd695-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cd695-117">Child elements</span></span>

<span data-ttu-id="cd695-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cd695-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd695-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cd695-119">Parent elements</span></span>

|<span data-ttu-id="cd695-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cd695-120">**Element**</span></span>|<span data-ttu-id="cd695-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="cd695-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd695-122">Suggestion</span><span class="sxs-lookup"><span data-stu-id="cd695-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="cd695-123">Représente une seule suggestion de l’heure de la réunion.</span><span class="sxs-lookup"><span data-stu-id="cd695-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="cd695-124">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="cd695-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cd695-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="cd695-125">Text value</span></span>

<span data-ttu-id="cd695-126">Une valeur de texte qui représente une valeur **dateTime** est requise.</span><span class="sxs-lookup"><span data-stu-id="cd695-126">A text value that represents a **dateTime** value is required.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cd695-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="cd695-127">Remarks</span></span>

<span data-ttu-id="cd695-128">L’élément [MeetingTime](meetingtime.md) est un élément enfant requis de l’élément de [Suggestion](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="cd695-128">The [MeetingTime](meetingtime.md) element is a required child element of the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="cd695-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="cd695-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd695-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cd695-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd695-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cd695-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd695-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cd695-132">Schema Name</span></span>  <br/> |<span data-ttu-id="cd695-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cd695-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="cd695-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cd695-134">Validation File</span></span>  <br/> |<span data-ttu-id="cd695-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cd695-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd695-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cd695-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="cd695-137">False</span><span class="sxs-lookup"><span data-stu-id="cd695-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd695-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cd695-138">See also</span></span>



[<span data-ttu-id="cd695-139">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="cd695-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="cd695-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cd695-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="cd695-141">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="cd695-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

