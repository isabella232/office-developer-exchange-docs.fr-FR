---
title: NumberOfMembersAvailable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersAvailable
api_type:
- schema
ms.assetid: e367a278-1622-4b65-955f-2d4b2fc6e4d7
description: L’élément NumberOfMembersAvailable représente le nombre de membres de la liste de distribution qui sont disponibles pour une heure de réunion suggérée. Cet élément représente les membres pour lesquels l’État est libre.
ms.openlocfilehash: 947e1c133cc49fb7e322962e95e184fe77e09353
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462590"
---
# <a name="numberofmembersavailable"></a><span data-ttu-id="8064e-104">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="8064e-104">NumberOfMembersAvailable</span></span>

<span data-ttu-id="8064e-105">L’élément **NumberOfMembersAvailable** représente le nombre de membres de la liste de distribution qui sont disponibles pour une heure de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="8064e-105">The **NumberOfMembersAvailable** element represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="8064e-106">Cet élément représente les membres pour lesquels l’État est **libre**.</span><span class="sxs-lookup"><span data-stu-id="8064e-106">This element represents members for whom the status is **Free**.</span></span>
  
[<span data-ttu-id="8064e-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="8064e-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="8064e-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="8064e-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="8064e-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="8064e-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="8064e-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="8064e-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="8064e-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="8064e-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="8064e-112">Suggérer</span><span class="sxs-lookup"><span data-stu-id="8064e-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="8064e-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="8064e-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="8064e-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="8064e-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="8064e-115">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="8064e-115">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md)
  
```xml
<NumberOfMembersAvailable>...</NumberOfMembersAvailable>
```

 <span data-ttu-id="8064e-116">**int**</span><span class="sxs-lookup"><span data-stu-id="8064e-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8064e-117">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8064e-117">Attributes and elements</span></span>

<span data-ttu-id="8064e-118">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8064e-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8064e-119">Attributs</span><span class="sxs-lookup"><span data-stu-id="8064e-119">Attributes</span></span>

<span data-ttu-id="8064e-120">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8064e-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8064e-121">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8064e-121">Child elements</span></span>

<span data-ttu-id="8064e-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8064e-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8064e-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8064e-123">Parent elements</span></span>

|<span data-ttu-id="8064e-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8064e-124">**Element**</span></span>|<span data-ttu-id="8064e-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="8064e-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8064e-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="8064e-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="8064e-127">Contient des informations sur les conflits d’agrégation concernant le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="8064e-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="8064e-128">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="8064e-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8064e-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="8064e-129">Remarks</span></span>

<span data-ttu-id="8064e-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8064e-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8064e-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8064e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8064e-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8064e-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8064e-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8064e-133">Schema Name</span></span>  <br/> |<span data-ttu-id="8064e-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8064e-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="8064e-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8064e-135">Validation File</span></span>  <br/> |<span data-ttu-id="8064e-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8064e-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8064e-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8064e-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="8064e-138">False</span><span class="sxs-lookup"><span data-stu-id="8064e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8064e-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8064e-139">See also</span></span>



[<span data-ttu-id="8064e-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="8064e-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="8064e-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="8064e-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="8064e-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="8064e-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

