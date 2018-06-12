---
title: SuggestionDayResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionDayResult
api_type:
- schema
ms.assetid: 916b1cbb-f2e3-471d-84b0-e33467616652
description: L’élément SuggestionDayResult représente une journée qui contient les heures de réunion proposée.
ms.openlocfilehash: 7b75258a9e70f1ec6feed6a0b18beb76f356c7f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838647"
---
# <a name="suggestiondayresult"></a><span data-ttu-id="055b9-103">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="055b9-103">SuggestionDayResult</span></span>

<span data-ttu-id="055b9-104">L’élément **SuggestionDayResult** représente une journée qui contient les heures de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="055b9-104">The **SuggestionDayResult** element represents a single day that contains suggested meeting times.</span></span> 
  
[<span data-ttu-id="055b9-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="055b9-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="055b9-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="055b9-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="055b9-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="055b9-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="055b9-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="055b9-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
```xml
<SuggestionDayResult>
   <Date>...</Date>
   <DayQuality>...</DayQuality>
   <SuggestionArray>...</SuggestionArray>
</SuggestionDayResult>
```

 <span data-ttu-id="055b9-109">**SuggestionDayResult**</span><span class="sxs-lookup"><span data-stu-id="055b9-109">**SuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="055b9-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="055b9-110">Attributes and elements</span></span>

<span data-ttu-id="055b9-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="055b9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="055b9-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="055b9-112">Attributes</span></span>

<span data-ttu-id="055b9-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="055b9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="055b9-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="055b9-114">Child elements</span></span>

|<span data-ttu-id="055b9-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="055b9-115">**Element**</span></span>|<span data-ttu-id="055b9-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="055b9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="055b9-117">Date</span><span class="sxs-lookup"><span data-stu-id="055b9-117">Date</span></span>](date.md) <br/> |<span data-ttu-id="055b9-118">Représente la date qui contient les heures de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="055b9-118">Represents the date that contains the suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="055b9-119">DayQuality</span><span class="sxs-lookup"><span data-stu-id="055b9-119">DayQuality</span></span>](dayquality.md) <br/> |<span data-ttu-id="055b9-120">Représente la qualité de la journée contenant les heures de réunions suggéré de qualité.</span><span class="sxs-lookup"><span data-stu-id="055b9-120">Represents the quality of the day for containing quality suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="055b9-121">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="055b9-121">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="055b9-122">Contient un tableau de suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="055b9-122">Contains an array of meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="055b9-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="055b9-123">Parent elements</span></span>

|<span data-ttu-id="055b9-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="055b9-124">**Element**</span></span>|<span data-ttu-id="055b9-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="055b9-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="055b9-126">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="055b9-126">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="055b9-127">Contient un tableau de suggestions organisées par date de réunion.</span><span class="sxs-lookup"><span data-stu-id="055b9-127">Contains an array of meeting suggestions organized by date.</span></span>  <br/> <span data-ttu-id="055b9-128">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="055b9-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="055b9-129">Note</span><span class="sxs-lookup"><span data-stu-id="055b9-129">Remarks</span></span>

<span data-ttu-id="055b9-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="055b9-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="055b9-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="055b9-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="055b9-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="055b9-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="055b9-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="055b9-133">Schema Name</span></span>  <br/> |<span data-ttu-id="055b9-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="055b9-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="055b9-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="055b9-135">Validation File</span></span>  <br/> |<span data-ttu-id="055b9-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="055b9-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="055b9-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="055b9-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="055b9-138">False</span><span class="sxs-lookup"><span data-stu-id="055b9-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="055b9-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="055b9-139">See also</span></span>



[<span data-ttu-id="055b9-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="055b9-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="055b9-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="055b9-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="055b9-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="055b9-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

