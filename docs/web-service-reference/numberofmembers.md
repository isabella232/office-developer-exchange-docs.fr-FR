---
title: NumberOfMembers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembers
api_type:
- schema
ms.assetid: 845fb877-de49-4e26-8885-6f026edd9ee9
description: L’élément NumberOfMembers représente le nombre d’utilisateurs, des ressources et des salles dans une liste de distribution.
ms.openlocfilehash: 9777660b1a54bfb5afb6e569ba1009a1654bdef3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828635"
---
# <a name="numberofmembers"></a><span data-ttu-id="4f242-103">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="4f242-103">NumberOfMembers</span></span>

<span data-ttu-id="4f242-104">L’élément **NumberOfMembers** représente le nombre d’utilisateurs, des ressources et des salles dans une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="4f242-104">The **NumberOfMembers** element represents the number of users, resources, and rooms in a distribution list.</span></span> 
  
[<span data-ttu-id="4f242-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4f242-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="4f242-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="4f242-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="4f242-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="4f242-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="4f242-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="4f242-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="4f242-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="4f242-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="4f242-110">Suggestion</span><span class="sxs-lookup"><span data-stu-id="4f242-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="4f242-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="4f242-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="4f242-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="4f242-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="4f242-113">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="4f242-113">NumberOfMembers</span></span>](numberofmembers.md)
  
```xml
<NumberOfMembers>...</NumberOfMembers>
```

 <span data-ttu-id="4f242-114">**int**</span><span class="sxs-lookup"><span data-stu-id="4f242-114">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f242-115">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4f242-115">Attributes and elements</span></span>

<span data-ttu-id="4f242-116">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4f242-116">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f242-117">Attributs</span><span class="sxs-lookup"><span data-stu-id="4f242-117">Attributes</span></span>

<span data-ttu-id="4f242-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4f242-118">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f242-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4f242-119">Child elements</span></span>

<span data-ttu-id="4f242-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4f242-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4f242-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4f242-121">Parent elements</span></span>

|<span data-ttu-id="4f242-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4f242-122">**Element**</span></span>|<span data-ttu-id="4f242-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f242-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f242-124">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="4f242-124">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="4f242-125">Contient des informations de conflit agrégation sur le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="4f242-125">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="4f242-126">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="4f242-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4f242-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="4f242-127">Remarks</span></span>

<span data-ttu-id="4f242-128">La valeur maximale de l’élément **NumberOfMembers** est 100.</span><span class="sxs-lookup"><span data-stu-id="4f242-128">The maximum value of the **NumberOfMembers** element is 100.</span></span> 
  
<span data-ttu-id="4f242-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4f242-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f242-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4f242-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f242-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4f242-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4f242-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4f242-132">Schema Name</span></span>  <br/> |<span data-ttu-id="4f242-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4f242-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="4f242-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4f242-134">Validation File</span></span>  <br/> |<span data-ttu-id="4f242-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4f242-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4f242-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4f242-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="4f242-137">False</span><span class="sxs-lookup"><span data-stu-id="4f242-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f242-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4f242-138">See also</span></span>



[<span data-ttu-id="4f242-139">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4f242-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="4f242-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4f242-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="4f242-141">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="4f242-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

