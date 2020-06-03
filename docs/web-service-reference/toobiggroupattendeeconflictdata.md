---
title: TooBigGroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TooBigGroupAttendeeConflictData
api_type:
- schema
ms.assetid: 1512428d-ce22-4da9-b1c1-446b4bcd0a21
description: L’élément TooBigGroupAttendeeConflictData représente un participant qui a été résolu en tant que liste de distribution, mais dont la liste de distribution était trop volumineuse pour être développée.
ms.openlocfilehash: 407a4a49e5f32c81439063f47df2e131dd663a4f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468599"
---
# <a name="toobiggroupattendeeconflictdata"></a><span data-ttu-id="2e666-103">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="2e666-103">TooBigGroupAttendeeConflictData</span></span>

<span data-ttu-id="2e666-104">L’élément **TooBigGroupAttendeeConflictData** représente un participant qui a été résolu en tant que liste de distribution, mais dont la liste de distribution était trop volumineuse pour être développée.</span><span class="sxs-lookup"><span data-stu-id="2e666-104">The **TooBigGroupAttendeeConflictData** element represents an attendee that was resolved as a distribution list but the distribution list was too large to expand.</span></span> 
  
[<span data-ttu-id="2e666-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2e666-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="2e666-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="2e666-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="2e666-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="2e666-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="2e666-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="2e666-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="2e666-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="2e666-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="2e666-110">Suggérer</span><span class="sxs-lookup"><span data-stu-id="2e666-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="2e666-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="2e666-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="2e666-112">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="2e666-112">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md)
  
```xml
<TooBigGroupAttendeeConflictData/>
```

 <span data-ttu-id="2e666-113">**TooBigGroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="2e666-113">**TooBigGroupAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e666-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2e666-114">Attributes and elements</span></span>

<span data-ttu-id="2e666-115">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2e666-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e666-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="2e666-116">Attributes</span></span>

<span data-ttu-id="2e666-117">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2e666-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2e666-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2e666-118">Child elements</span></span>

<span data-ttu-id="2e666-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2e666-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2e666-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2e666-120">Parent elements</span></span>

|<span data-ttu-id="2e666-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2e666-121">**Element**</span></span>|<span data-ttu-id="2e666-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="2e666-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e666-123">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="2e666-123">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="2e666-124">Contient un tableau de données en conflit pour les participants identifiés dans le [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span><span class="sxs-lookup"><span data-stu-id="2e666-124">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="2e666-125">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="2e666-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2e666-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="2e666-126">Remarks</span></span>

<span data-ttu-id="2e666-127">Les listes de distribution contenant plus de 100 membres ne peuvent pas être développées.</span><span class="sxs-lookup"><span data-stu-id="2e666-127">Distribution lists that contain more than 100 members cannot be expanded.</span></span>
  
<span data-ttu-id="2e666-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2e666-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e666-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2e666-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e666-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2e666-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2e666-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2e666-131">Schema Name</span></span>  <br/> |<span data-ttu-id="2e666-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2e666-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="2e666-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2e666-133">Validation File</span></span>  <br/> |<span data-ttu-id="2e666-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2e666-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2e666-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2e666-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="2e666-136">False</span><span class="sxs-lookup"><span data-stu-id="2e666-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2e666-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2e666-137">See also</span></span>



[<span data-ttu-id="2e666-138">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2e666-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="2e666-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2e666-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="2e666-140">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="2e666-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

