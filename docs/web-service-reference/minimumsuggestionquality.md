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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828468"
---
# <a name="minimumsuggestionquality"></a><span data-ttu-id="79d62-103">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="79d62-103">MinimumSuggestionQuality</span></span>

<span data-ttu-id="79d62-104">L’élément **MinimumSuggestionQuality** définit la qualité des suggestions de réunion à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="79d62-104">The **MinimumSuggestionQuality** element defines the quality of meeting suggestions to be returned in the response.</span></span> 
  
[<span data-ttu-id="79d62-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="79d62-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="79d62-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="79d62-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="79d62-107">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="79d62-107">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
```

 <span data-ttu-id="79d62-108">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="79d62-108">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79d62-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="79d62-109">Attributes and elements</span></span>

<span data-ttu-id="79d62-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="79d62-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79d62-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="79d62-111">Attributes</span></span>

<span data-ttu-id="79d62-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79d62-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79d62-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="79d62-113">Child elements</span></span>

<span data-ttu-id="79d62-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79d62-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79d62-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="79d62-115">Parent elements</span></span>

|<span data-ttu-id="79d62-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="79d62-116">**Element**</span></span>|<span data-ttu-id="79d62-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="79d62-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79d62-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="79d62-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="79d62-119">Contient les options permettant d’obtenir des informations de suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="79d62-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="79d62-120">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="79d62-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79d62-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="79d62-121">Text value</span></span>

<span data-ttu-id="79d62-122">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="79d62-122">A text value is required.</span></span> <span data-ttu-id="79d62-123">Le tableau suivant répertorie les valeurs possibles de cet élément :</span><span class="sxs-lookup"><span data-stu-id="79d62-123">The following table lists the possible values for this element:</span></span>
  
|<span data-ttu-id="79d62-124">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="79d62-124">**Value**</span></span>|<span data-ttu-id="79d62-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="79d62-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="79d62-126">**Excellente**</span><span class="sxs-lookup"><span data-stu-id="79d62-126">**Excellent**</span></span> <br/> |<span data-ttu-id="79d62-127">0 % des participants ont un conflit avec l’heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="79d62-127">0% of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
|<span data-ttu-id="79d62-128">**Une bonne**</span><span class="sxs-lookup"><span data-stu-id="79d62-128">**Good**</span></span> <br/> |<span data-ttu-id="79d62-129">Le pourcentage est considérée comme bonne est défini à l’aide de l’élément [GoodThreshold](goodthreshold.md) .</span><span class="sxs-lookup"><span data-stu-id="79d62-129">The percentage that is considered good is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="79d62-130">**Juste**</span><span class="sxs-lookup"><span data-stu-id="79d62-130">**Fair**</span></span> <br/> |<span data-ttu-id="79d62-131">Le pourcentage est considéré comme étant juste est défini à l’aide de l’élément [GoodThreshold](goodthreshold.md) .</span><span class="sxs-lookup"><span data-stu-id="79d62-131">The percentage that is considered fair is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="79d62-132">**Une mauvaise**</span><span class="sxs-lookup"><span data-stu-id="79d62-132">**Poor**</span></span> <br/> |<span data-ttu-id="79d62-133">50 % ou plus des participants ont un conflit avec l’heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="79d62-133">50% or more of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="79d62-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="79d62-134">Remarks</span></span>

<span data-ttu-id="79d62-135">Cet élément est obligatoire si l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="79d62-135">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="79d62-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="79d62-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="79d62-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="79d62-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79d62-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="79d62-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79d62-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="79d62-139">Schema Name</span></span>  <br/> |<span data-ttu-id="79d62-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="79d62-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="79d62-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="79d62-141">Validation File</span></span>  <br/> |<span data-ttu-id="79d62-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="79d62-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79d62-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="79d62-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="79d62-144">False</span><span class="sxs-lookup"><span data-stu-id="79d62-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79d62-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79d62-145">See also</span></span>



[<span data-ttu-id="79d62-146">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="79d62-146">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="79d62-147">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="79d62-147">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

