---
title: IndividualAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndividualAttendeeConflictData
api_type:
- schema
ms.assetid: d45d3c34-abe1-40da-afd3-23bc5c3ef474
description: L’élément IndividualAttendeeConflictData contient le statut de disponibilité d’un utilisateur ou d’un contact pour une fenêtre de temps qui se produit en même temps que la réunion suggérée, identifiée dans l’élément de suggestion.
ms.openlocfilehash: 55210230259b78e5ed9c4f0744aae003cf2e7ae5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459313"
---
# <a name="individualattendeeconflictdata"></a><span data-ttu-id="fa9d5-103">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="fa9d5-103">IndividualAttendeeConflictData</span></span>

<span data-ttu-id="fa9d5-104">L’élément **IndividualAttendeeConflictData** contient le statut de disponibilité d’un utilisateur ou d’un contact pour une fenêtre de temps qui se produit en même temps que la réunion suggérée, identifiée dans l’élément de [suggestion](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="fa9d5-104">The **IndividualAttendeeConflictData** element contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
[<span data-ttu-id="fa9d5-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fa9d5-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="fa9d5-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="fa9d5-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="fa9d5-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="fa9d5-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="fa9d5-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="fa9d5-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="fa9d5-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="fa9d5-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="fa9d5-110">Suggérer</span><span class="sxs-lookup"><span data-stu-id="fa9d5-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="fa9d5-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="fa9d5-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="fa9d5-112">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="fa9d5-112">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md)
  
```xml
<IndividualAttendeeConflictData>
   <BusyType>...</BusyType>
</IndividualAttendeeConflictData>
```

 <span data-ttu-id="fa9d5-113">**IndividualAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="fa9d5-113">**IndividualAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa9d5-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fa9d5-114">Attributes and elements</span></span>

<span data-ttu-id="fa9d5-115">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fa9d5-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa9d5-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="fa9d5-116">Attributes</span></span>

<span data-ttu-id="fa9d5-117">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fa9d5-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa9d5-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fa9d5-118">Child elements</span></span>

|<span data-ttu-id="fa9d5-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fa9d5-119">**Element**</span></span>|<span data-ttu-id="fa9d5-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="fa9d5-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa9d5-121">BusyType</span><span class="sxs-lookup"><span data-stu-id="fa9d5-121">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="fa9d5-122">Représente l’état de disponibilité d’un utilisateur pour une suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="fa9d5-122">Represents the free/busy status of a user for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fa9d5-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fa9d5-123">Parent elements</span></span>

|<span data-ttu-id="fa9d5-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fa9d5-124">**Element**</span></span>|<span data-ttu-id="fa9d5-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="fa9d5-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa9d5-126">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="fa9d5-126">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="fa9d5-127">Contient un tableau de données en conflit pour les participants identifiés dans le [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span><span class="sxs-lookup"><span data-stu-id="fa9d5-127">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="fa9d5-128">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="fa9d5-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fa9d5-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="fa9d5-129">Remarks</span></span>

<span data-ttu-id="fa9d5-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fa9d5-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa9d5-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fa9d5-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa9d5-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fa9d5-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa9d5-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fa9d5-133">Schema Name</span></span>  <br/> |<span data-ttu-id="fa9d5-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fa9d5-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="fa9d5-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fa9d5-135">Validation File</span></span>  <br/> |<span data-ttu-id="fa9d5-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fa9d5-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa9d5-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fa9d5-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="fa9d5-138">False</span><span class="sxs-lookup"><span data-stu-id="fa9d5-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa9d5-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fa9d5-139">See also</span></span>



[<span data-ttu-id="fa9d5-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="fa9d5-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="fa9d5-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fa9d5-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="fa9d5-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="fa9d5-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

