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
description: L’élément AttendeeConflictDataArray contient un tableau de données de conflit pour les participants interrogées identifiés dans l’opération GetUserAvailability.
ms.openlocfilehash: 169312b8a3d37c014ba58fbfe094d786b134fc90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755343"
---
# <a name="attendeeconflictdataarray"></a><span data-ttu-id="0cf44-103">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="0cf44-103">AttendeeConflictDataArray</span></span>

<span data-ttu-id="0cf44-104">L’élément **AttendeeConflictDataArray** contient un tableau de données de conflit pour les participants interrogées identifiés dans l' [opération GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0cf44-104">The **AttendeeConflictDataArray** element contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>
  
- [<span data-ttu-id="0cf44-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0cf44-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="0cf44-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="0cf44-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
- [<span data-ttu-id="0cf44-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="0cf44-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
- [<span data-ttu-id="0cf44-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="0cf44-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
- [<span data-ttu-id="0cf44-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="0cf44-109">SuggestionArray</span></span>](suggestionarray.md)
  
- [<span data-ttu-id="0cf44-110">Suggestion</span><span class="sxs-lookup"><span data-stu-id="0cf44-110">Suggestion</span></span>](suggestion.md)
  
- [<span data-ttu-id="0cf44-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="0cf44-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
```xml
<ArrayOfAttendeeConflictData>
   <UnknownAttendeeConflictData>...</UnknownAttendeeConflictData>
   <IndividualAttendeeConflictData>...</IndividualAttendeeConflictData>
   <TooBigGroupAttendeeConflictData>...</TooBigGroupAttendeeConflictData>
   <GroupAttendeeConflictData>...</GroupAttendeeConflictData>
</ArrayOfAttendeeConflictData>
```

 <span data-ttu-id="0cf44-112">**ArrayOfAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="0cf44-112">**ArrayOfAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0cf44-113">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0cf44-113">Attributes and elements</span></span>

<span data-ttu-id="0cf44-114">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0cf44-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0cf44-115">Attributs</span><span class="sxs-lookup"><span data-stu-id="0cf44-115">Attributes</span></span>

<span data-ttu-id="0cf44-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0cf44-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0cf44-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0cf44-117">Child elements</span></span>

|<span data-ttu-id="0cf44-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0cf44-118">**Element**</span></span>|<span data-ttu-id="0cf44-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="0cf44-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cf44-120">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="0cf44-120">UnknownAttendeeConflictData</span></span>](unknownattendeeconflictdata.md) <br/> |<span data-ttu-id="0cf44-121">Représente un participant insolubles ou un participant qui n’est pas un utilisateur, une liste de distribution ou un contact.</span><span class="sxs-lookup"><span data-stu-id="0cf44-121">Represents an unresolvable attendee or an attendee that is not a user, distribution list, or contact.</span></span>  <br/> |
|[<span data-ttu-id="0cf44-122">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="0cf44-122">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="0cf44-123">Contient un utilisateur ou un contact disponibilité pour une fenêtre de temps qui se produit en même temps que suggérés temps identifié dans l’élément de la [Suggestion](suggestion.md) de réunion.</span><span class="sxs-lookup"><span data-stu-id="0cf44-123">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span>  <br/> |
|[<span data-ttu-id="0cf44-124">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="0cf44-124">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md) <br/> |<span data-ttu-id="0cf44-125">Représente un participant résolu comme une liste de distribution qui était trop volumineuse pour la développer.</span><span class="sxs-lookup"><span data-stu-id="0cf44-125">Represents an attendee that resolved as a distribution list that was too large to expand.</span></span>  <br/> |
|[<span data-ttu-id="0cf44-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="0cf44-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="0cf44-127">Contient des informations de conflit agrégation sur le nombre d’utilisateurs disponibles, le nombre d’utilisateurs qui ont des conflits et le nombre d’utilisateurs qui n’ont pas d’informations de disponibilité dans une liste de distribution pour une heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="0cf44-127">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0cf44-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0cf44-128">Parent elements</span></span>

|<span data-ttu-id="0cf44-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0cf44-129">**Element**</span></span>|<span data-ttu-id="0cf44-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="0cf44-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cf44-131">Suggestion</span><span class="sxs-lookup"><span data-stu-id="0cf44-131">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="0cf44-132">Représente une seule suggestion de l’heure de la réunion.</span><span class="sxs-lookup"><span data-stu-id="0cf44-132">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="0cf44-133">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="0cf44-133">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0cf44-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="0cf44-134">Remarks</span></span>

<span data-ttu-id="0cf44-135">La position de chaque élément dans **AttendeeConflictDataArray** correspond à la position des participants dans l’élément [MailboxDataArray](mailboxdataarray.md) interrogées.</span><span class="sxs-lookup"><span data-stu-id="0cf44-135">The position of each element in the **AttendeeConflictDataArray** corresponds to the position of the queried attendees in the [MailboxDataArray](mailboxdataarray.md) element.</span></span> <span data-ttu-id="0cf44-136">Chaque participant interrogée doit correspondre à un des éléments enfants **AttendeeConflictDataArray** .</span><span class="sxs-lookup"><span data-stu-id="0cf44-136">Each queried attendee must correspond to one of the **AttendeeConflictDataArray** child elements.</span></span> <span data-ttu-id="0cf44-137">Ces éléments représentent un conflit avec l’heure de réunion proposée identifié dans l’élément [Suggestion](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="0cf44-137">These elements represent a single conflict with the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="0cf44-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0cf44-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0cf44-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0cf44-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0cf44-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0cf44-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0cf44-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0cf44-141">Schema Name</span></span>  <br/> |<span data-ttu-id="0cf44-142">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0cf44-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="0cf44-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0cf44-143">Validation File</span></span>  <br/> |<span data-ttu-id="0cf44-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0cf44-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0cf44-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0cf44-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="0cf44-146">False</span><span class="sxs-lookup"><span data-stu-id="0cf44-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0cf44-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0cf44-147">See also</span></span>

- [<span data-ttu-id="0cf44-148">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0cf44-148">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="0cf44-149">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0cf44-149">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="0cf44-150">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="0cf44-150">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

