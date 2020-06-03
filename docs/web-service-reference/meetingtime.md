---
title: MeetingTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTime
api_type:
- schema
ms.assetid: 6e6d2d8b-e8a2-43e6-a715-0fc7d6dd44b9
description: L’élément MeetingTime représente une suggestion de réunion.
ms.openlocfilehash: 3a7031e70eb8b22adc8030c1cec09d33399332ee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530449"
---
# <a name="meetingtime"></a><span data-ttu-id="d1bd9-103">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="d1bd9-103">MeetingTime</span></span>

<span data-ttu-id="d1bd9-104">L’élément **MeetingTime** représente une suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="d1bd9-104">The **MeetingTime** element represents a suggested meeting time.</span></span> 
  
[<span data-ttu-id="d1bd9-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d1bd9-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d1bd9-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="d1bd9-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="d1bd9-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="d1bd9-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="d1bd9-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="d1bd9-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="d1bd9-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="d1bd9-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="d1bd9-110">Suggérer</span><span class="sxs-lookup"><span data-stu-id="d1bd9-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="d1bd9-111">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="d1bd9-111">MeetingTime</span></span>](meetingtime.md)
  
```xml
<MeetingTime>...</MeetingTime
```

 <span data-ttu-id="d1bd9-112">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="d1bd9-112">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1bd9-113">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d1bd9-113">Attributes and elements</span></span>

<span data-ttu-id="d1bd9-114">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d1bd9-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1bd9-115">Attributs</span><span class="sxs-lookup"><span data-stu-id="d1bd9-115">Attributes</span></span>

<span data-ttu-id="d1bd9-116">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d1bd9-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1bd9-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d1bd9-117">Child elements</span></span>

<span data-ttu-id="d1bd9-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d1bd9-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1bd9-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d1bd9-119">Parent elements</span></span>

|<span data-ttu-id="d1bd9-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d1bd9-120">**Element**</span></span>|<span data-ttu-id="d1bd9-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="d1bd9-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1bd9-122">Suggérer</span><span class="sxs-lookup"><span data-stu-id="d1bd9-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="d1bd9-123">Représente une seule suggestion de temps de réunion.</span><span class="sxs-lookup"><span data-stu-id="d1bd9-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="d1bd9-124">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="d1bd9-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d1bd9-125">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="d1bd9-125">Text value</span></span>

<span data-ttu-id="d1bd9-126">Une valeur de texte qui représente une valeur **DateTime** est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="d1bd9-126">A text value that represents a **dateTime** value is required.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d1bd9-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="d1bd9-127">Remarks</span></span>

<span data-ttu-id="d1bd9-128">L’élément [MeetingTime](meetingtime.md) est un élément enfant obligatoire de l’élément [suggestions](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="d1bd9-128">The [MeetingTime](meetingtime.md) element is a required child element of the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="d1bd9-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d1bd9-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1bd9-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d1bd9-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1bd9-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d1bd9-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1bd9-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d1bd9-132">Schema Name</span></span>  <br/> |<span data-ttu-id="d1bd9-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d1bd9-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d1bd9-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d1bd9-134">Validation File</span></span>  <br/> |<span data-ttu-id="d1bd9-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d1bd9-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1bd9-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d1bd9-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="d1bd9-137">False</span><span class="sxs-lookup"><span data-stu-id="d1bd9-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1bd9-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d1bd9-138">See also</span></span>



[<span data-ttu-id="d1bd9-139">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d1bd9-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d1bd9-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d1bd9-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d1bd9-141">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="d1bd9-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

