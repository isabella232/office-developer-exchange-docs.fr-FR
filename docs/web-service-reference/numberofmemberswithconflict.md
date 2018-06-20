---
title: NumberOfMembersWithConflict
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersWithConflict
api_type:
- schema
ms.assetid: e61154f7-d262-43ec-b2bf-1ba6804b28dc
description: L’élément NumberOfMembersWithConflict représente le nombre de membres de liste de distribution qui ont un conflit avec une heure de réunion proposée. Cet élément représente des membres qui ont l’état occupé (e), absent du bureau ou provisoire.
ms.openlocfilehash: 227783b4bed32686e8e098f88498fe8ebb25e3cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828634"
---
# <a name="numberofmemberswithconflict"></a><span data-ttu-id="81e12-104">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="81e12-104">NumberOfMembersWithConflict</span></span>

<span data-ttu-id="81e12-105">L’élément **NumberOfMembersWithConflict** représente le nombre de membres de liste de distribution qui ont un conflit avec une heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="81e12-105">The **NumberOfMembersWithConflict** element represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="81e12-106">Cet élément représente des membres qui ont l’état **occupé (e)**, **absent du bureau**ou **provisoire**.</span><span class="sxs-lookup"><span data-stu-id="81e12-106">This element represents members who have a status of **Busy**, **OOF**, or **Tentative**.</span></span>
  
[<span data-ttu-id="81e12-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="81e12-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="81e12-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="81e12-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="81e12-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="81e12-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="81e12-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="81e12-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="81e12-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="81e12-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="81e12-112">Suggestion</span><span class="sxs-lookup"><span data-stu-id="81e12-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="81e12-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="81e12-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="81e12-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="81e12-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="81e12-115">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="81e12-115">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md)
  
```xml
<NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
```

 <span data-ttu-id="81e12-116">**int**</span><span class="sxs-lookup"><span data-stu-id="81e12-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81e12-117">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="81e12-117">Attributes and elements</span></span>

<span data-ttu-id="81e12-118">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="81e12-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81e12-119">Attributs</span><span class="sxs-lookup"><span data-stu-id="81e12-119">Attributes</span></span>

<span data-ttu-id="81e12-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="81e12-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81e12-121">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="81e12-121">Child elements</span></span>

<span data-ttu-id="81e12-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="81e12-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="81e12-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="81e12-123">Parent elements</span></span>

|<span data-ttu-id="81e12-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="81e12-124">**Element**</span></span>|<span data-ttu-id="81e12-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="81e12-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81e12-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="81e12-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="81e12-127">Contient des informations de conflit agrégation sur le nombre d’utilisateurs qui sont disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="81e12-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="81e12-128">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="81e12-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="81e12-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="81e12-129">Remarks</span></span>

<span data-ttu-id="81e12-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="81e12-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81e12-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="81e12-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81e12-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="81e12-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="81e12-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="81e12-133">Schema Name</span></span>  <br/> |<span data-ttu-id="81e12-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="81e12-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="81e12-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="81e12-135">Validation File</span></span>  <br/> |<span data-ttu-id="81e12-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="81e12-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="81e12-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="81e12-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="81e12-138">False</span><span class="sxs-lookup"><span data-stu-id="81e12-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81e12-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="81e12-139">See also</span></span>



[<span data-ttu-id="81e12-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="81e12-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="81e12-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="81e12-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="81e12-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="81e12-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

