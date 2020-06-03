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
description: L’élément NumberOfMembersWithConflict représente le nombre de membres de la liste de distribution qui ont un conflit avec une heure de réunion suggérée. Cet élément représente les membres dont l’État est Busy, OOF ou provisoire.
ms.openlocfilehash: 3ed81fc8adece140e8a94b08a9c2d94c2d9787c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529034"
---
# <a name="numberofmemberswithconflict"></a><span data-ttu-id="94178-104">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="94178-104">NumberOfMembersWithConflict</span></span>

<span data-ttu-id="94178-105">L’élément **NumberOfMembersWithConflict** représente le nombre de membres de la liste de distribution qui ont un conflit avec une heure de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="94178-105">The **NumberOfMembersWithConflict** element represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="94178-106">Cet élément représente les membres dont l’État est **Busy**, **OOF**ou **provisoire**.</span><span class="sxs-lookup"><span data-stu-id="94178-106">This element represents members who have a status of **Busy**, **OOF**, or **Tentative**.</span></span>
  
[<span data-ttu-id="94178-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="94178-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="94178-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="94178-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="94178-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="94178-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="94178-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="94178-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="94178-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="94178-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="94178-112">Suggérer</span><span class="sxs-lookup"><span data-stu-id="94178-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="94178-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="94178-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="94178-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="94178-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="94178-115">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="94178-115">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md)
  
```xml
<NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
```

 <span data-ttu-id="94178-116">**int**</span><span class="sxs-lookup"><span data-stu-id="94178-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94178-117">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="94178-117">Attributes and elements</span></span>

<span data-ttu-id="94178-118">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="94178-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94178-119">Attributs</span><span class="sxs-lookup"><span data-stu-id="94178-119">Attributes</span></span>

<span data-ttu-id="94178-120">Aucune.</span><span class="sxs-lookup"><span data-stu-id="94178-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94178-121">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="94178-121">Child elements</span></span>

<span data-ttu-id="94178-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="94178-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="94178-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="94178-123">Parent elements</span></span>

|<span data-ttu-id="94178-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="94178-124">**Element**</span></span>|<span data-ttu-id="94178-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="94178-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94178-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="94178-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="94178-127">Contient des informations sur les conflits d’agrégation concernant le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="94178-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="94178-128">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="94178-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="94178-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="94178-129">Remarks</span></span>

<span data-ttu-id="94178-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="94178-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94178-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="94178-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94178-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="94178-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94178-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="94178-133">Schema Name</span></span>  <br/> |<span data-ttu-id="94178-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="94178-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="94178-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="94178-135">Validation File</span></span>  <br/> |<span data-ttu-id="94178-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="94178-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94178-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="94178-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="94178-138">False</span><span class="sxs-lookup"><span data-stu-id="94178-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94178-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="94178-139">See also</span></span>



[<span data-ttu-id="94178-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="94178-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="94178-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="94178-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="94178-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="94178-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

