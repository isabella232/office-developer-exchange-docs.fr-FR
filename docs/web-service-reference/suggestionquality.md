---
title: SuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionQuality
api_type:
- schema
ms.assetid: 734f1a58-adda-4830-973e-e84bf7b870d5
description: L’élément SuggestionQuality représente la qualité de l’heure de réunion proposée.
ms.openlocfilehash: e67e0149226b36c22cdd00acd78f6582f826dd3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838648"
---
# <a name="suggestionquality"></a><span data-ttu-id="12646-103">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="12646-103">SuggestionQuality</span></span>

<span data-ttu-id="12646-104">L’élément **SuggestionQuality** représente la qualité de l’heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="12646-104">The **SuggestionQuality** element represents the quality of the suggested meeting time.</span></span> 
  
[<span data-ttu-id="12646-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="12646-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="12646-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="12646-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="12646-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="12646-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="12646-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="12646-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="12646-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="12646-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="12646-110">Suggestion</span><span class="sxs-lookup"><span data-stu-id="12646-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="12646-111">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="12646-111">SuggestionQuality</span></span>](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 <span data-ttu-id="12646-112">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="12646-112">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12646-113">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="12646-113">Attributes and elements</span></span>

<span data-ttu-id="12646-114">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="12646-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12646-115">Attributs</span><span class="sxs-lookup"><span data-stu-id="12646-115">Attributes</span></span>

<span data-ttu-id="12646-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="12646-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12646-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="12646-117">Child elements</span></span>

<span data-ttu-id="12646-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="12646-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12646-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="12646-119">Parent elements</span></span>

|<span data-ttu-id="12646-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="12646-120">**Element**</span></span>|<span data-ttu-id="12646-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="12646-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12646-122">Suggestion</span><span class="sxs-lookup"><span data-stu-id="12646-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="12646-123">Représente une seule suggestion de l’heure de la réunion.</span><span class="sxs-lookup"><span data-stu-id="12646-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="12646-124">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="12646-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12646-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="12646-125">Text value</span></span>

<span data-ttu-id="12646-126">Une valeur de texte qui représente une valeur **SuggestionQuality** est requise.</span><span class="sxs-lookup"><span data-stu-id="12646-126">A text value that represents a **SuggestionQuality** value is required.</span></span> <span data-ttu-id="12646-127">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="12646-127">The following are the possible values:</span></span> 
  
- <span data-ttu-id="12646-128">**Excellent** 100 % des utilisateurs et des ressources sont disponibles pour l’heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="12646-128">**Excellent** 100 percent of users and resources are available for the suggested meeting time.</span></span> 
    
- <span data-ttu-id="12646-129">**Une bonne** Le pourcentage minimal d’utilisateurs et des ressources disponibles est égale ou supérieure à la valeur de l’élément [GoodThreshold](goodthreshold.md) plus de 50.</span><span class="sxs-lookup"><span data-stu-id="12646-129">**Good** The minimum percentage of users and resources available is equal to or greater than the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> 
    
- <span data-ttu-id="12646-130">**Juste** Le pourcentage maximal d’utilisateurs et les ressources disponibles pour une heure de réunion proposée est égal à la valeur de l’élément [GoodThreshold](goodthreshold.md) plus de 50.</span><span class="sxs-lookup"><span data-stu-id="12646-130">**Fair** The maximum percentage of users and resources available for a suggested meeting time is equal to the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> <span data-ttu-id="12646-131">La valeur minimale pour une heure de réunion qualité **juste** est de 50 pour cent.</span><span class="sxs-lookup"><span data-stu-id="12646-131">The minimum value for a **Fair** quality meeting time is 50 percent.</span></span> 
    
- <span data-ttu-id="12646-132">**Une mauvaise** Inférieur à 50 % des utilisateurs et des ressources sont disponibles pour l’heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="12646-132">**Poor** Less than 50 percent of the users and resources are available for the suggested meeting time.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="12646-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="12646-133">Remarks</span></span>

<span data-ttu-id="12646-134">Le type **SuggestionQuality** est également le type de la [DayQuality](dayquality.md) et les éléments [MinimumSuggestionQuality](minimumsuggestionquality.md) .</span><span class="sxs-lookup"><span data-stu-id="12646-134">The **SuggestionQuality** type is also the type for the [DayQuality](dayquality.md) and the [MinimumSuggestionQuality](minimumsuggestionquality.md) elements.</span></span> 
  
<span data-ttu-id="12646-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="12646-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12646-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="12646-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12646-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="12646-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12646-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="12646-138">Schema Name</span></span>  <br/> |<span data-ttu-id="12646-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="12646-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="12646-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="12646-140">Validation File</span></span>  <br/> |<span data-ttu-id="12646-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="12646-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12646-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="12646-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="12646-143">False</span><span class="sxs-lookup"><span data-stu-id="12646-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12646-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="12646-144">See also</span></span>



[<span data-ttu-id="12646-145">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="12646-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="12646-146">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="12646-146">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="12646-147">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="12646-147">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

