---
title: GroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupAttendeeConflictData
api_type:
- schema
ms.assetid: fd8bf19a-298b-4135-93e8-ead3db7e1142
description: L’élément GroupAttendeeConflictData contient des informations de conflit agrégation sur le nombre d’utilisateurs qui sont disponible, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une distribution de liste pour un suggérés heure de la réunion.
ms.openlocfilehash: 382b4d866c95de98bd444cd6226d71813889d4f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827757"
---
# <a name="groupattendeeconflictdata"></a><span data-ttu-id="09e56-103">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="09e56-103">GroupAttendeeConflictData</span></span>

<span data-ttu-id="09e56-104">L’élément **GroupAttendeeConflictData** contient des informations de conflit agrégation sur le nombre d’utilisateurs qui sont disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="09e56-104">The **GroupAttendeeConflictData** element contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span> 
  
- [<span data-ttu-id="09e56-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="09e56-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="09e56-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="09e56-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
- [<span data-ttu-id="09e56-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="09e56-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
- [<span data-ttu-id="09e56-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="09e56-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
- [<span data-ttu-id="09e56-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="09e56-109">SuggestionArray</span></span>](suggestionarray.md)
- [<span data-ttu-id="09e56-110">Suggestion</span><span class="sxs-lookup"><span data-stu-id="09e56-110">Suggestion</span></span>](suggestion.md)
- [<span data-ttu-id="09e56-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="09e56-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
- [<span data-ttu-id="09e56-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="09e56-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

<span data-ttu-id="09e56-113">**GroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="09e56-113">**GroupAttendeeConflictData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="09e56-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="09e56-114">Attributes and elements</span></span>

<span data-ttu-id="09e56-115">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="09e56-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09e56-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="09e56-116">Attributes</span></span>

<span data-ttu-id="09e56-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="09e56-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09e56-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="09e56-118">Child elements</span></span>

|<span data-ttu-id="09e56-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="09e56-119">**Element**</span></span>|<span data-ttu-id="09e56-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="09e56-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09e56-121">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="09e56-121">NumberOfMembers</span></span>](numberofmembers.md) <br/> |<span data-ttu-id="09e56-122">Représente le nombre d’utilisateurs, des ressources et des salles dans une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="09e56-122">Represents the number of users, resources, and rooms in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="09e56-123">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="09e56-123">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md) <br/> |<span data-ttu-id="09e56-124">Représente le nombre de membres de liste de distribution qui sont disponibles pour une heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="09e56-124">Represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="09e56-125">Cet élément représente des membres pour lesquels l’état est **disponible**.</span><span class="sxs-lookup"><span data-stu-id="09e56-125">This element represents members for whom the status is **Free**.</span></span>  <br/> |
|[<span data-ttu-id="09e56-126">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="09e56-126">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md) <br/> |<span data-ttu-id="09e56-127">Représente le nombre de membres de liste de distribution qui ont un conflit avec une heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="09e56-127">Represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="09e56-128">Cet élément représente des membres qui ont l’état **occupé (e)**, **absent du bureau**ou **provisoire** .</span><span class="sxs-lookup"><span data-stu-id="09e56-128">This element represents members who have a **Busy**, **OOF**, or **Tentative** status.</span></span>  <br/> |
|[<span data-ttu-id="09e56-129">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="09e56-129">NumberOfMembersWithNoData</span></span>](numberofmemberswithnodata.md) <br/> |<span data-ttu-id="09e56-130">Représente le nombre de membres du groupe qui n’ont pas de données et de disponibilité publiées à comparer à une heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="09e56-130">Represents the number of group members who do not have published free/busy data to compare to a suggested meeting time.</span></span> <span data-ttu-id="09e56-131">Cet élément représente les membres d’une liste de distribution est trop grande ou qui ont l’état **Aucune donnée** .</span><span class="sxs-lookup"><span data-stu-id="09e56-131">This element represents members of a distribution list that is too large or members who have **No Data** status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="09e56-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="09e56-132">Parent elements</span></span>

|<span data-ttu-id="09e56-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="09e56-133">**Element**</span></span>|<span data-ttu-id="09e56-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="09e56-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09e56-135">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="09e56-135">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="09e56-136">Contient un tableau de données de conflit pour les participants interrogées identifiés dans l' [opération GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="09e56-136">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="09e56-137">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="09e56-137">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="09e56-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="09e56-138">Remarks</span></span>

<span data-ttu-id="09e56-139">L’élément **GroupAttendeeConflictData** est présent dans la réponse lorsqu’un participant dans la [GetUserAvailabilityRequest](getuseravailabilityrequest.md) est résolu en une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="09e56-139">The **GroupAttendeeConflictData** element is present in the response when an attendee in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) is resolved to a distribution list.</span></span> <span data-ttu-id="09e56-140">L’élément **GroupAttendeeConflictData** identifie les trois états de membres d’une liste de distribution : disponible, en conflit, ou aucune donnée.</span><span class="sxs-lookup"><span data-stu-id="09e56-140">The **GroupAttendeeConflictData** element identifies three states for members of a distribution list: available, conflicted, or no data.</span></span> <span data-ttu-id="09e56-141">Développement de listes de distribution prendront en charge jusqu'à 100 membres.</span><span class="sxs-lookup"><span data-stu-id="09e56-141">Distribution list expansion will support up to 100 members.</span></span> <span data-ttu-id="09e56-142">Par conséquent, l’élément [NumberOfMembers](numberofmembers.md) peut contenir un maximum de 100 membres.</span><span class="sxs-lookup"><span data-stu-id="09e56-142">Therefore, the [NumberOfMembers](numberofmembers.md) element can contain a maximum of 100 members.</span></span> <span data-ttu-id="09e56-143">Développement de listes de distribution est récursive.</span><span class="sxs-lookup"><span data-stu-id="09e56-143">Distribution list expansion is recursive.</span></span> <span data-ttu-id="09e56-144">Si une liste de distribution contient une liste de distribution enfants qui développe l’appartenance total parent à plus de 100 membres, la liste de distribution enfants n’est pas développée et comptera comme une seule entrée du nombre d’éléments [NumberOfMembersWithNoData](numberofmemberswithnodata.md) .</span><span class="sxs-lookup"><span data-stu-id="09e56-144">If a distribution list contains a child distribution list that expands the total parent membership to over 100 members, the child distribution list will not be expanded and will count as a single entry of the [NumberOfMembersWithNoData](numberofmemberswithnodata.md) element count.</span></span> <span data-ttu-id="09e56-145">Si une liste de distribution enfants peut être développée et l’appartenance parent total ne développe pas plus de 100 membres, son appartenance est développé et les nombres de membres sont ajoutées pour les éléments enfants de l’élément **GroupAttendeeConflictData** .</span><span class="sxs-lookup"><span data-stu-id="09e56-145">If a child distribution list can be expanded and the total parent membership does not expand to over 100 members, its membership is expanded and the member counts are added to the child elements of the **GroupAttendeeConflictData** element.</span></span> 
  
<span data-ttu-id="09e56-146">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="09e56-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09e56-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="09e56-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09e56-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="09e56-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="09e56-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="09e56-149">Schema Name</span></span>  <br/> |<span data-ttu-id="09e56-150">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="09e56-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="09e56-151">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="09e56-151">Validation File</span></span>  <br/> |<span data-ttu-id="09e56-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="09e56-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="09e56-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="09e56-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="09e56-154">False</span><span class="sxs-lookup"><span data-stu-id="09e56-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09e56-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="09e56-155">See also</span></span>

- [<span data-ttu-id="09e56-156">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="09e56-156">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="09e56-157">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="09e56-157">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="09e56-158">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="09e56-158">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
