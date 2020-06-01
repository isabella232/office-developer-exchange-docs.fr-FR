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
description: L’élément SuggestionDayResult représente un jour qui contient des heures de réunion suggérées.
ms.openlocfilehash: af907b62acefb4913814907722b98d326bd0535b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457990"
---
# <a name="suggestiondayresult"></a><span data-ttu-id="730b0-103">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="730b0-103">SuggestionDayResult</span></span>

<span data-ttu-id="730b0-104">L’élément **SuggestionDayResult** représente un jour qui contient des heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="730b0-104">The **SuggestionDayResult** element represents a single day that contains suggested meeting times.</span></span> 
  
[<span data-ttu-id="730b0-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="730b0-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="730b0-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="730b0-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="730b0-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="730b0-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="730b0-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="730b0-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
```xml
<SuggestionDayResult>
   <Date>...</Date>
   <DayQuality>...</DayQuality>
   <SuggestionArray>...</SuggestionArray>
</SuggestionDayResult>
```

 <span data-ttu-id="730b0-109">**SuggestionDayResult**</span><span class="sxs-lookup"><span data-stu-id="730b0-109">**SuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="730b0-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="730b0-110">Attributes and elements</span></span>

<span data-ttu-id="730b0-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="730b0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="730b0-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="730b0-112">Attributes</span></span>

<span data-ttu-id="730b0-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="730b0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="730b0-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="730b0-114">Child elements</span></span>

|<span data-ttu-id="730b0-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="730b0-115">**Element**</span></span>|<span data-ttu-id="730b0-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="730b0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="730b0-117">Date</span><span class="sxs-lookup"><span data-stu-id="730b0-117">Date</span></span>](date.md) <br/> |<span data-ttu-id="730b0-118">Représente la date qui contient les heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="730b0-118">Represents the date that contains the suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="730b0-119">DayQuality</span><span class="sxs-lookup"><span data-stu-id="730b0-119">DayQuality</span></span>](dayquality.md) <br/> |<span data-ttu-id="730b0-120">Représente la qualité du jour pour le temps de réunion suggéré.</span><span class="sxs-lookup"><span data-stu-id="730b0-120">Represents the quality of the day for containing quality suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="730b0-121">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="730b0-121">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="730b0-122">Contient un tableau de suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="730b0-122">Contains an array of meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="730b0-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="730b0-123">Parent elements</span></span>

|<span data-ttu-id="730b0-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="730b0-124">**Element**</span></span>|<span data-ttu-id="730b0-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="730b0-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="730b0-126">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="730b0-126">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="730b0-127">Contient un tableau des suggestions de réunion organisées par date.</span><span class="sxs-lookup"><span data-stu-id="730b0-127">Contains an array of meeting suggestions organized by date.</span></span>  <br/> <span data-ttu-id="730b0-128">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="730b0-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="730b0-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="730b0-129">Remarks</span></span>

<span data-ttu-id="730b0-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="730b0-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="730b0-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="730b0-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="730b0-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="730b0-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="730b0-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="730b0-133">Schema Name</span></span>  <br/> |<span data-ttu-id="730b0-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="730b0-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="730b0-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="730b0-135">Validation File</span></span>  <br/> |<span data-ttu-id="730b0-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="730b0-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="730b0-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="730b0-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="730b0-138">False</span><span class="sxs-lookup"><span data-stu-id="730b0-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="730b0-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="730b0-139">See also</span></span>



[<span data-ttu-id="730b0-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="730b0-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="730b0-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="730b0-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="730b0-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="730b0-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

