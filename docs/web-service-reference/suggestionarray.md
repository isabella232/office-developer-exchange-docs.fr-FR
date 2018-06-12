---
title: SuggestionArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionArray
api_type:
- schema
ms.assetid: c1c26008-7b14-4563-8db5-bceb0f475b1b
description: L’élément SuggestionArray contient un tableau de suggestions de réunion.
ms.openlocfilehash: d595ae77de293a1975e15102f3f2c3395e6da633
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838646"
---
# <a name="suggestionarray"></a><span data-ttu-id="d4b6c-103">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="d4b6c-103">SuggestionArray</span></span>

<span data-ttu-id="d4b6c-104">L’élément **SuggestionArray** contient un tableau de suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="d4b6c-104">The **SuggestionArray** element contains an array of meeting suggestions.</span></span> 
  
[<span data-ttu-id="d4b6c-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d4b6c-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d4b6c-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="d4b6c-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="d4b6c-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="d4b6c-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="d4b6c-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="d4b6c-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="d4b6c-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="d4b6c-109">SuggestionArray</span></span>](suggestionarray.md)
  
```xml
<SuggestionArray>
   <Suggestion>...</Suggestion>
</SuggestionArray>
```

 <span data-ttu-id="d4b6c-110">**ArrayOfSuggestion**</span><span class="sxs-lookup"><span data-stu-id="d4b6c-110">**ArrayOfSuggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4b6c-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4b6c-111">Attributes and elements</span></span>

<span data-ttu-id="d4b6c-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4b6c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4b6c-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4b6c-113">Attributes</span></span>

<span data-ttu-id="d4b6c-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4b6c-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4b6c-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4b6c-115">Child elements</span></span>

|<span data-ttu-id="d4b6c-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4b6c-116">**Element**</span></span>|<span data-ttu-id="d4b6c-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4b6c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4b6c-118">Suggestion</span><span class="sxs-lookup"><span data-stu-id="d4b6c-118">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="d4b6c-119">Représente une suggestion de réunion unique.</span><span class="sxs-lookup"><span data-stu-id="d4b6c-119">Represents a single meeting suggestion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4b6c-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4b6c-120">Parent elements</span></span>

|<span data-ttu-id="d4b6c-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4b6c-121">**Element**</span></span>|<span data-ttu-id="d4b6c-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4b6c-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4b6c-123">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="d4b6c-123">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="d4b6c-124">Représente un seul jour qui contient les heures de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="d4b6c-124">Represents a single day that contains suggested meeting times.</span></span>  <br/> <span data-ttu-id="d4b6c-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="d4b6c-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d4b6c-126">Note</span><span class="sxs-lookup"><span data-stu-id="d4b6c-126">Remarks</span></span>

<span data-ttu-id="d4b6c-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d4b6c-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4b6c-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4b6c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4b6c-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4b6c-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4b6c-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4b6c-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d4b6c-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d4b6c-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4b6c-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4b6c-132">Validation File</span></span>  <br/> |<span data-ttu-id="d4b6c-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4b6c-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4b6c-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4b6c-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4b6c-135">False</span><span class="sxs-lookup"><span data-stu-id="d4b6c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4b6c-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4b6c-136">See also</span></span>



[<span data-ttu-id="d4b6c-137">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d4b6c-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d4b6c-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d4b6c-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d4b6c-139">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="d4b6c-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
