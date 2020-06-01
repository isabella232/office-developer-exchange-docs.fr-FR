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
description: L’élément SuggestionQuality représente la qualité de l’heure de la réunion suggérée.
ms.openlocfilehash: 3f8c15ccabd03687dc386a0328020cbc0bc802c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457976"
---
# <a name="suggestionquality"></a><span data-ttu-id="32d4a-103">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="32d4a-103">SuggestionQuality</span></span>

<span data-ttu-id="32d4a-104">L’élément **SuggestionQuality** représente la qualité de l’heure de la réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="32d4a-104">The **SuggestionQuality** element represents the quality of the suggested meeting time.</span></span> 
  
[<span data-ttu-id="32d4a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="32d4a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="32d4a-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="32d4a-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="32d4a-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="32d4a-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="32d4a-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="32d4a-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="32d4a-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="32d4a-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="32d4a-110">Suggérer</span><span class="sxs-lookup"><span data-stu-id="32d4a-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="32d4a-111">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="32d4a-111">SuggestionQuality</span></span>](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 <span data-ttu-id="32d4a-112">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="32d4a-112">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32d4a-113">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="32d4a-113">Attributes and elements</span></span>

<span data-ttu-id="32d4a-114">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="32d4a-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32d4a-115">Attributs</span><span class="sxs-lookup"><span data-stu-id="32d4a-115">Attributes</span></span>

<span data-ttu-id="32d4a-116">Aucune.</span><span class="sxs-lookup"><span data-stu-id="32d4a-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32d4a-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="32d4a-117">Child elements</span></span>

<span data-ttu-id="32d4a-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="32d4a-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32d4a-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="32d4a-119">Parent elements</span></span>

|<span data-ttu-id="32d4a-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="32d4a-120">**Element**</span></span>|<span data-ttu-id="32d4a-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="32d4a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32d4a-122">Suggérer</span><span class="sxs-lookup"><span data-stu-id="32d4a-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="32d4a-123">Représente une seule suggestion de temps de réunion.</span><span class="sxs-lookup"><span data-stu-id="32d4a-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="32d4a-124">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="32d4a-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32d4a-125">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="32d4a-125">Text value</span></span>

<span data-ttu-id="32d4a-126">Une valeur de texte qui représente une valeur **SuggestionQuality** est requise.</span><span class="sxs-lookup"><span data-stu-id="32d4a-126">A text value that represents a **SuggestionQuality** value is required.</span></span> <span data-ttu-id="32d4a-127">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="32d4a-127">The following are the possible values:</span></span> 
  
- <span data-ttu-id="32d4a-128">Un **excellent** pourcentage de 100 pour cent des utilisateurs et des ressources est disponible pour la réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="32d4a-128">**Excellent** 100 percent of users and resources are available for the suggested meeting time.</span></span> 
    
- <span data-ttu-id="32d4a-129">**Utile** Le pourcentage minimal d’utilisateurs et de ressources disponibles est supérieur ou égal à la valeur de l’élément [GoodThreshold](goodthreshold.md) plus 50.</span><span class="sxs-lookup"><span data-stu-id="32d4a-129">**Good** The minimum percentage of users and resources available is equal to or greater than the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> 
    
- <span data-ttu-id="32d4a-130">**Équitable** Le pourcentage maximal d’utilisateurs et de ressources disponibles pour une heure de réunion suggérée est égal à la valeur de l’élément [GoodThreshold](goodthreshold.md) plus 50.</span><span class="sxs-lookup"><span data-stu-id="32d4a-130">**Fair** The maximum percentage of users and resources available for a suggested meeting time is equal to the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> <span data-ttu-id="32d4a-131">La valeur minimale pour un temps de réunion de qualité **équitable** est de 50%.</span><span class="sxs-lookup"><span data-stu-id="32d4a-131">The minimum value for a **Fair** quality meeting time is 50 percent.</span></span> 
    
- <span data-ttu-id="32d4a-132">**Médiocre** Moins de 50% des utilisateurs et des ressources sont disponibles pour la réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="32d4a-132">**Poor** Less than 50 percent of the users and resources are available for the suggested meeting time.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="32d4a-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="32d4a-133">Remarks</span></span>

<span data-ttu-id="32d4a-134">Le type **SuggestionQuality** est également le type pour les éléments [DayQuality](dayquality.md) et [MinimumSuggestionQuality](minimumsuggestionquality.md) .</span><span class="sxs-lookup"><span data-stu-id="32d4a-134">The **SuggestionQuality** type is also the type for the [DayQuality](dayquality.md) and the [MinimumSuggestionQuality](minimumsuggestionquality.md) elements.</span></span> 
  
<span data-ttu-id="32d4a-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="32d4a-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32d4a-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="32d4a-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32d4a-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="32d4a-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32d4a-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="32d4a-138">Schema Name</span></span>  <br/> |<span data-ttu-id="32d4a-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="32d4a-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="32d4a-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="32d4a-140">Validation File</span></span>  <br/> |<span data-ttu-id="32d4a-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="32d4a-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="32d4a-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="32d4a-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="32d4a-143">False</span><span class="sxs-lookup"><span data-stu-id="32d4a-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32d4a-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="32d4a-144">See also</span></span>



[<span data-ttu-id="32d4a-145">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="32d4a-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="32d4a-146">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="32d4a-146">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="32d4a-147">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="32d4a-147">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

