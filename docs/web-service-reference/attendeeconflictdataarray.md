---
title: AttendeeConflictDataArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeConflictDataArray
api_type:
- schema
ms.assetid: 1d758547-28c5-4649-8334-427480c282d6
description: L’élément AttendeeConflictDataArray contient un tableau de données conflictuelles pour les participants interrogés identifiés dans l’opération GetUserAvailability.
ms.openlocfilehash: 770e8c00ca248ec3562180dc9d3626fd5b58f4d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455799"
---
# <a name="attendeeconflictdataarray"></a><span data-ttu-id="a89bb-103">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="a89bb-103">AttendeeConflictDataArray</span></span>

<span data-ttu-id="a89bb-104">L’élément **AttendeeConflictDataArray** contient un tableau de données conflictuelles pour les participants interrogés identifiés dans l' [opération GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a89bb-104">The **AttendeeConflictDataArray** element contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>
  
- [<span data-ttu-id="a89bb-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a89bb-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="a89bb-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="a89bb-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
- [<span data-ttu-id="a89bb-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="a89bb-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
- [<span data-ttu-id="a89bb-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="a89bb-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
- [<span data-ttu-id="a89bb-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="a89bb-109">SuggestionArray</span></span>](suggestionarray.md)
  
- [<span data-ttu-id="a89bb-110">Suggérer</span><span class="sxs-lookup"><span data-stu-id="a89bb-110">Suggestion</span></span>](suggestion.md)
  
- [<span data-ttu-id="a89bb-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="a89bb-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
```xml
<ArrayOfAttendeeConflictData>
   <UnknownAttendeeConflictData>...</UnknownAttendeeConflictData>
   <IndividualAttendeeConflictData>...</IndividualAttendeeConflictData>
   <TooBigGroupAttendeeConflictData>...</TooBigGroupAttendeeConflictData>
   <GroupAttendeeConflictData>...</GroupAttendeeConflictData>
</ArrayOfAttendeeConflictData>
```

 <span data-ttu-id="a89bb-112">**ArrayOfAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="a89bb-112">**ArrayOfAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a89bb-113">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a89bb-113">Attributes and elements</span></span>

<span data-ttu-id="a89bb-114">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a89bb-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a89bb-115">Attributs</span><span class="sxs-lookup"><span data-stu-id="a89bb-115">Attributes</span></span>

<span data-ttu-id="a89bb-116">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a89bb-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a89bb-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a89bb-117">Child elements</span></span>

|<span data-ttu-id="a89bb-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a89bb-118">**Element**</span></span>|<span data-ttu-id="a89bb-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="a89bb-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a89bb-120">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="a89bb-120">UnknownAttendeeConflictData</span></span>](unknownattendeeconflictdata.md) <br/> |<span data-ttu-id="a89bb-121">Représente un participant non résolu ou un participant qui n’est pas un utilisateur, une liste de distribution ou un contact.</span><span class="sxs-lookup"><span data-stu-id="a89bb-121">Represents an unresolvable attendee or an attendee that is not a user, distribution list, or contact.</span></span>  <br/> |
|[<span data-ttu-id="a89bb-122">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="a89bb-122">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="a89bb-123">Contient le statut de disponibilité d’un utilisateur ou d’un contact pour une fenêtre de temps qui se produit en même temps que la réunion suggérée, identifiée dans l’élément de [suggestion](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="a89bb-123">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span>  <br/> |
|[<span data-ttu-id="a89bb-124">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="a89bb-124">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md) <br/> |<span data-ttu-id="a89bb-125">Représente un participant résolu en tant que liste de distribution trop grande pour être développée.</span><span class="sxs-lookup"><span data-stu-id="a89bb-125">Represents an attendee that resolved as a distribution list that was too large to expand.</span></span>  <br/> |
|[<span data-ttu-id="a89bb-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="a89bb-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="a89bb-127">Contient des informations sur les conflits d’agrégation concernant le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="a89bb-127">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a89bb-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a89bb-128">Parent elements</span></span>

|<span data-ttu-id="a89bb-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a89bb-129">**Element**</span></span>|<span data-ttu-id="a89bb-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="a89bb-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a89bb-131">Suggérer</span><span class="sxs-lookup"><span data-stu-id="a89bb-131">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="a89bb-132">Représente une seule suggestion de temps de réunion.</span><span class="sxs-lookup"><span data-stu-id="a89bb-132">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="a89bb-133">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="a89bb-133">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a89bb-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="a89bb-134">Remarks</span></span>

<span data-ttu-id="a89bb-135">La position de chaque élément dans le **AttendeeConflictDataArray** correspond à la position des participants interrogés dans l’élément [MailboxDataArray](mailboxdataarray.md) .</span><span class="sxs-lookup"><span data-stu-id="a89bb-135">The position of each element in the **AttendeeConflictDataArray** corresponds to the position of the queried attendees in the [MailboxDataArray](mailboxdataarray.md) element.</span></span> <span data-ttu-id="a89bb-136">Chaque participant interrogé doit correspondre à l’un des éléments enfants **AttendeeConflictDataArray** .</span><span class="sxs-lookup"><span data-stu-id="a89bb-136">Each queried attendee must correspond to one of the **AttendeeConflictDataArray** child elements.</span></span> <span data-ttu-id="a89bb-137">Ces éléments représentent un conflit unique avec l’heure de réunion suggérée identifiée dans l’élément de [suggestion](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="a89bb-137">These elements represent a single conflict with the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="a89bb-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a89bb-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a89bb-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a89bb-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a89bb-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a89bb-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a89bb-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a89bb-141">Schema Name</span></span>  <br/> |<span data-ttu-id="a89bb-142">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a89bb-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="a89bb-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a89bb-143">Validation File</span></span>  <br/> |<span data-ttu-id="a89bb-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a89bb-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a89bb-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a89bb-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="a89bb-146">False</span><span class="sxs-lookup"><span data-stu-id="a89bb-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a89bb-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a89bb-147">See also</span></span>

- [<span data-ttu-id="a89bb-148">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a89bb-148">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="a89bb-149">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a89bb-149">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="a89bb-150">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a89bb-150">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

