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
description: L’élément GroupAttendeeConflictData contient des informations sur les conflits globaux sur le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion suggérée.
ms.openlocfilehash: c75a4e6f8fdff7fb2514f448350fee9f1acb9775
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462928"
---
# <a name="groupattendeeconflictdata"></a><span data-ttu-id="abed6-103">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="abed6-103">GroupAttendeeConflictData</span></span>

<span data-ttu-id="abed6-104">L’élément **GroupAttendeeConflictData** contient des informations sur les conflits globaux sur le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="abed6-104">The **GroupAttendeeConflictData** element contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span> 
  
- [<span data-ttu-id="abed6-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="abed6-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="abed6-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="abed6-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
- [<span data-ttu-id="abed6-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="abed6-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
- [<span data-ttu-id="abed6-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="abed6-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
- [<span data-ttu-id="abed6-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="abed6-109">SuggestionArray</span></span>](suggestionarray.md)
- [<span data-ttu-id="abed6-110">Suggérer</span><span class="sxs-lookup"><span data-stu-id="abed6-110">Suggestion</span></span>](suggestion.md)
- [<span data-ttu-id="abed6-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="abed6-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
- [<span data-ttu-id="abed6-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="abed6-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

<span data-ttu-id="abed6-113">**GroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="abed6-113">**GroupAttendeeConflictData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="abed6-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="abed6-114">Attributes and elements</span></span>

<span data-ttu-id="abed6-115">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="abed6-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="abed6-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="abed6-116">Attributes</span></span>

<span data-ttu-id="abed6-117">Aucune.</span><span class="sxs-lookup"><span data-stu-id="abed6-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="abed6-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="abed6-118">Child elements</span></span>

|<span data-ttu-id="abed6-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="abed6-119">**Element**</span></span>|<span data-ttu-id="abed6-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="abed6-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abed6-121">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="abed6-121">NumberOfMembers</span></span>](numberofmembers.md) <br/> |<span data-ttu-id="abed6-122">Représente le nombre d’utilisateurs, de ressources et de salles dans une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="abed6-122">Represents the number of users, resources, and rooms in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="abed6-123">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="abed6-123">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md) <br/> |<span data-ttu-id="abed6-124">Représente le nombre de membres de la liste de distribution qui sont disponibles pour une heure de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="abed6-124">Represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="abed6-125">Cet élément représente les membres pour lesquels l’État est **libre**.</span><span class="sxs-lookup"><span data-stu-id="abed6-125">This element represents members for whom the status is **Free**.</span></span>  <br/> |
|[<span data-ttu-id="abed6-126">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="abed6-126">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md) <br/> |<span data-ttu-id="abed6-127">Représente le nombre de membres de la liste de distribution qui ont un conflit avec une heure de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="abed6-127">Represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="abed6-128">Cet élément représente les membres qui ont un état occupé, absent (e), **absent**( **e**) ou **provisoire** .</span><span class="sxs-lookup"><span data-stu-id="abed6-128">This element represents members who have a **Busy**, **OOF**, or **Tentative** status.</span></span>  <br/> |
|[<span data-ttu-id="abed6-129">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="abed6-129">NumberOfMembersWithNoData</span></span>](numberofmemberswithnodata.md) <br/> |<span data-ttu-id="abed6-130">Représente le nombre de membres du groupe qui n’ont pas de données de disponibilité publiées à comparer à une heure de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="abed6-130">Represents the number of group members who do not have published free/busy data to compare to a suggested meeting time.</span></span> <span data-ttu-id="abed6-131">Cet élément représente les membres d’une liste de distribution qui est trop grande ou dont les membres n’ont pas d’état de **données** .</span><span class="sxs-lookup"><span data-stu-id="abed6-131">This element represents members of a distribution list that is too large or members who have **No Data** status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="abed6-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="abed6-132">Parent elements</span></span>

|<span data-ttu-id="abed6-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="abed6-133">**Element**</span></span>|<span data-ttu-id="abed6-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="abed6-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="abed6-135">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="abed6-135">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="abed6-136">Contient un tableau de données conflictuelles pour les participants interrogés identifiés dans l' [opération GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="abed6-136">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="abed6-137">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="abed6-137">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="abed6-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="abed6-138">Remarks</span></span>

<span data-ttu-id="abed6-139">L’élément **GroupAttendeeConflictData** est présent dans la réponse lorsqu’un participant de la [GetUserAvailabilityRequest](getuseravailabilityrequest.md) est résolu en une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="abed6-139">The **GroupAttendeeConflictData** element is present in the response when an attendee in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) is resolved to a distribution list.</span></span> <span data-ttu-id="abed6-140">L’élément **GroupAttendeeConflictData** identifie trois États pour les membres d’une liste de distribution : disponible, en conflit ou sans données.</span><span class="sxs-lookup"><span data-stu-id="abed6-140">The **GroupAttendeeConflictData** element identifies three states for members of a distribution list: available, conflicted, or no data.</span></span> <span data-ttu-id="abed6-141">L’extension de la liste de distribution prendra en charge jusqu’à 100 membres.</span><span class="sxs-lookup"><span data-stu-id="abed6-141">Distribution list expansion will support up to 100 members.</span></span> <span data-ttu-id="abed6-142">Par conséquent, l’élément [NumberOfMembers](numberofmembers.md) peut contenir un maximum de 100 membres.</span><span class="sxs-lookup"><span data-stu-id="abed6-142">Therefore, the [NumberOfMembers](numberofmembers.md) element can contain a maximum of 100 members.</span></span> <span data-ttu-id="abed6-143">L’extension de la liste de distribution est récursive.</span><span class="sxs-lookup"><span data-stu-id="abed6-143">Distribution list expansion is recursive.</span></span> <span data-ttu-id="abed6-144">Si une liste de distribution contient une liste de distribution enfant qui étend l’appartenance totale au parent à plus de 100 membres, la liste de distribution enfant n’est pas étendue et compte comme une seule entrée du nombre d’éléments [NumberOfMembersWithNoData](numberofmemberswithnodata.md) .</span><span class="sxs-lookup"><span data-stu-id="abed6-144">If a distribution list contains a child distribution list that expands the total parent membership to over 100 members, the child distribution list will not be expanded and will count as a single entry of the [NumberOfMembersWithNoData](numberofmemberswithnodata.md) element count.</span></span> <span data-ttu-id="abed6-145">Si une liste de distribution enfant peut être étendue et que l’appartenance au groupe parent ne dépasse pas 100 membres, son appartenance est étendue et le nombre de membres est ajouté aux éléments enfants de l’élément **GroupAttendeeConflictData** .</span><span class="sxs-lookup"><span data-stu-id="abed6-145">If a child distribution list can be expanded and the total parent membership does not expand to over 100 members, its membership is expanded and the member counts are added to the child elements of the **GroupAttendeeConflictData** element.</span></span> 
  
<span data-ttu-id="abed6-146">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="abed6-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="abed6-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="abed6-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="abed6-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="abed6-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="abed6-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="abed6-149">Schema Name</span></span>  <br/> |<span data-ttu-id="abed6-150">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="abed6-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="abed6-151">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="abed6-151">Validation File</span></span>  <br/> |<span data-ttu-id="abed6-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="abed6-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="abed6-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="abed6-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="abed6-154">False</span><span class="sxs-lookup"><span data-stu-id="abed6-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="abed6-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="abed6-155">See also</span></span>

- [<span data-ttu-id="abed6-156">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="abed6-156">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="abed6-157">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="abed6-157">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="abed6-158">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="abed6-158">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

