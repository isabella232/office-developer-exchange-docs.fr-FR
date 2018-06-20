---
title: MinimumSuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MinimumSuggestionQuality
api_type:
- schema
ms.assetid: 3725cbd4-9bc1-4f7d-8929-b2c68cb46114
description: L’élément MinimumSuggestionQuality définit la qualité des suggestions de réunion à renvoyer dans la réponse.
ms.openlocfilehash: ac79682bd761f678f23fc2d698a50fd7704f6fab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828468"
---
# <a name="minimumsuggestionquality"></a><span data-ttu-id="bbc76-103">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="bbc76-103">MinimumSuggestionQuality</span></span>

<span data-ttu-id="bbc76-104">L’élément **MinimumSuggestionQuality** définit la qualité des suggestions de réunion à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="bbc76-104">The **MinimumSuggestionQuality** element defines the quality of meeting suggestions to be returned in the response.</span></span> 
  
[<span data-ttu-id="bbc76-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="bbc76-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="bbc76-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="bbc76-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="bbc76-107">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="bbc76-107">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
```

 <span data-ttu-id="bbc76-108">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="bbc76-108">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bbc76-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bbc76-109">Attributes and elements</span></span>

<span data-ttu-id="bbc76-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bbc76-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bbc76-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="bbc76-111">Attributes</span></span>

<span data-ttu-id="bbc76-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bbc76-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bbc76-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bbc76-113">Child elements</span></span>

<span data-ttu-id="bbc76-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bbc76-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bbc76-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bbc76-115">Parent elements</span></span>

|<span data-ttu-id="bbc76-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bbc76-116">**Element**</span></span>|<span data-ttu-id="bbc76-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="bbc76-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bbc76-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="bbc76-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="bbc76-119">Contient les options permettant d’obtenir des informations de suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="bbc76-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="bbc76-120">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="bbc76-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bbc76-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bbc76-121">Text value</span></span>

<span data-ttu-id="bbc76-122">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="bbc76-122">A text value is required.</span></span> <span data-ttu-id="bbc76-123">Le tableau suivant répertorie les valeurs possibles de cet élément :</span><span class="sxs-lookup"><span data-stu-id="bbc76-123">The following table lists the possible values for this element:</span></span>
  
|<span data-ttu-id="bbc76-124">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="bbc76-124">**Value**</span></span>|<span data-ttu-id="bbc76-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="bbc76-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bbc76-126">**Excellente**</span><span class="sxs-lookup"><span data-stu-id="bbc76-126">**Excellent**</span></span> <br/> |<span data-ttu-id="bbc76-127">0 % des participants ont un conflit avec l’heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="bbc76-127">0% of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
|<span data-ttu-id="bbc76-128">**Une bonne**</span><span class="sxs-lookup"><span data-stu-id="bbc76-128">**Good**</span></span> <br/> |<span data-ttu-id="bbc76-129">Le pourcentage est considérée comme bonne est défini à l’aide de l’élément [GoodThreshold](goodthreshold.md) .</span><span class="sxs-lookup"><span data-stu-id="bbc76-129">The percentage that is considered good is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="bbc76-130">**Juste**</span><span class="sxs-lookup"><span data-stu-id="bbc76-130">**Fair**</span></span> <br/> |<span data-ttu-id="bbc76-131">Le pourcentage est considéré comme étant juste est défini à l’aide de l’élément [GoodThreshold](goodthreshold.md) .</span><span class="sxs-lookup"><span data-stu-id="bbc76-131">The percentage that is considered fair is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="bbc76-132">**Une mauvaise**</span><span class="sxs-lookup"><span data-stu-id="bbc76-132">**Poor**</span></span> <br/> |<span data-ttu-id="bbc76-133">50 % ou plus des participants ont un conflit avec l’heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="bbc76-133">50% or more of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bbc76-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="bbc76-134">Remarks</span></span>

<span data-ttu-id="bbc76-135">Cet élément est obligatoire si l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="bbc76-135">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bbc76-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="bbc76-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="bbc76-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bbc76-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bbc76-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bbc76-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bbc76-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bbc76-139">Schema Name</span></span>  <br/> |<span data-ttu-id="bbc76-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bbc76-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="bbc76-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bbc76-141">Validation File</span></span>  <br/> |<span data-ttu-id="bbc76-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bbc76-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bbc76-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bbc76-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="bbc76-144">False</span><span class="sxs-lookup"><span data-stu-id="bbc76-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bbc76-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bbc76-145">See also</span></span>



[<span data-ttu-id="bbc76-146">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="bbc76-146">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="bbc76-147">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="bbc76-147">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

