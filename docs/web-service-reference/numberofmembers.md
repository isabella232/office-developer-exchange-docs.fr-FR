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
description: L’élément NumberOfMembers représente le nombre d’utilisateurs, de ressources et de salles dans une liste de distribution.
ms.openlocfilehash: c91087f42d806afb0a0d3d607cc84f14a1a6c1b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462597"
---
# <a name="numberofmembers"></a><span data-ttu-id="dc193-103">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="dc193-103">NumberOfMembers</span></span>

<span data-ttu-id="dc193-104">L’élément **NumberOfMembers** représente le nombre d’utilisateurs, de ressources et de salles dans une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="dc193-104">The **NumberOfMembers** element represents the number of users, resources, and rooms in a distribution list.</span></span> 
  
[<span data-ttu-id="dc193-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="dc193-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="dc193-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="dc193-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="dc193-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="dc193-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="dc193-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="dc193-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="dc193-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="dc193-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="dc193-110">Suggérer</span><span class="sxs-lookup"><span data-stu-id="dc193-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="dc193-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="dc193-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="dc193-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="dc193-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="dc193-113">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="dc193-113">NumberOfMembers</span></span>](numberofmembers.md)
  
```xml
<NumberOfMembers>...</NumberOfMembers>
```

 <span data-ttu-id="dc193-114">**int**</span><span class="sxs-lookup"><span data-stu-id="dc193-114">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc193-115">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dc193-115">Attributes and elements</span></span>

<span data-ttu-id="dc193-116">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dc193-116">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc193-117">Attributs</span><span class="sxs-lookup"><span data-stu-id="dc193-117">Attributes</span></span>

<span data-ttu-id="dc193-118">Aucune.</span><span class="sxs-lookup"><span data-stu-id="dc193-118">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc193-119">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dc193-119">Child elements</span></span>

<span data-ttu-id="dc193-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dc193-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dc193-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dc193-121">Parent elements</span></span>

|<span data-ttu-id="dc193-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dc193-122">**Element**</span></span>|<span data-ttu-id="dc193-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="dc193-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc193-124">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="dc193-124">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="dc193-125">Contient des informations sur les conflits d’agrégation concernant le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="dc193-125">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="dc193-126">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="dc193-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dc193-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="dc193-127">Remarks</span></span>

<span data-ttu-id="dc193-128">La valeur maximale de l’élément **NumberOfMembers** est 100.</span><span class="sxs-lookup"><span data-stu-id="dc193-128">The maximum value of the **NumberOfMembers** element is 100.</span></span> 
  
<span data-ttu-id="dc193-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="dc193-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc193-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dc193-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc193-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dc193-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dc193-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dc193-132">Schema Name</span></span>  <br/> |<span data-ttu-id="dc193-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="dc193-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="dc193-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dc193-134">Validation File</span></span>  <br/> |<span data-ttu-id="dc193-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dc193-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dc193-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dc193-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc193-137">False</span><span class="sxs-lookup"><span data-stu-id="dc193-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc193-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dc193-138">See also</span></span>



[<span data-ttu-id="dc193-139">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="dc193-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="dc193-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="dc193-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="dc193-141">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="dc193-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

