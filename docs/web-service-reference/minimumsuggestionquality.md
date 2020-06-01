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
ms.openlocfilehash: c85cbf65a63ac0b09408c14e01889f97a05b27b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467479"
---
# <a name="minimumsuggestionquality"></a><span data-ttu-id="4f270-103">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="4f270-103">MinimumSuggestionQuality</span></span>

<span data-ttu-id="4f270-104">L’élément **MinimumSuggestionQuality** définit la qualité des suggestions de réunion à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="4f270-104">The **MinimumSuggestionQuality** element defines the quality of meeting suggestions to be returned in the response.</span></span> 
  
[<span data-ttu-id="4f270-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="4f270-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="4f270-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="4f270-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="4f270-107">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="4f270-107">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
```

 <span data-ttu-id="4f270-108">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="4f270-108">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f270-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4f270-109">Attributes and elements</span></span>

<span data-ttu-id="4f270-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4f270-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f270-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="4f270-111">Attributes</span></span>

<span data-ttu-id="4f270-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4f270-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f270-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4f270-113">Child elements</span></span>

<span data-ttu-id="4f270-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4f270-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4f270-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4f270-115">Parent elements</span></span>

|<span data-ttu-id="4f270-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4f270-116">**Element**</span></span>|<span data-ttu-id="4f270-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f270-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f270-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="4f270-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="4f270-119">Contient les options permettant d’obtenir des informations sur les suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="4f270-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="4f270-120">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="4f270-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4f270-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4f270-121">Text value</span></span>

<span data-ttu-id="4f270-122">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="4f270-122">A text value is required.</span></span> <span data-ttu-id="4f270-123">Le tableau suivant répertorie les valeurs possibles pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="4f270-123">The following table lists the possible values for this element:</span></span>
  
|<span data-ttu-id="4f270-124">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4f270-124">**Value**</span></span>|<span data-ttu-id="4f270-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f270-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4f270-126">**Excellente**</span><span class="sxs-lookup"><span data-stu-id="4f270-126">**Excellent**</span></span> <br/> |<span data-ttu-id="4f270-127">0% des participants ont un conflit avec l’heure de la réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="4f270-127">0% of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
|<span data-ttu-id="4f270-128">**Good**</span><span class="sxs-lookup"><span data-stu-id="4f270-128">**Good**</span></span> <br/> |<span data-ttu-id="4f270-129">Le pourcentage considéré comme approprié est défini à l’aide de l’élément [GoodThreshold](goodthreshold.md) .</span><span class="sxs-lookup"><span data-stu-id="4f270-129">The percentage that is considered good is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="4f270-130">**Beau**</span><span class="sxs-lookup"><span data-stu-id="4f270-130">**Fair**</span></span> <br/> |<span data-ttu-id="4f270-131">Le pourcentage considéré comme équitable est défini à l’aide de l’élément [GoodThreshold](goodthreshold.md) .</span><span class="sxs-lookup"><span data-stu-id="4f270-131">The percentage that is considered fair is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="4f270-132">**Mauvais**</span><span class="sxs-lookup"><span data-stu-id="4f270-132">**Poor**</span></span> <br/> |<span data-ttu-id="4f270-133">50% ou plus des participants ont un conflit avec l’heure de la réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="4f270-133">50% or more of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4f270-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="4f270-134">Remarks</span></span>

<span data-ttu-id="4f270-135">Cet élément est requis si l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="4f270-135">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4f270-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4f270-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="4f270-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4f270-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f270-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4f270-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4f270-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4f270-139">Schema Name</span></span>  <br/> |<span data-ttu-id="4f270-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4f270-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="4f270-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4f270-141">Validation File</span></span>  <br/> |<span data-ttu-id="4f270-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4f270-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4f270-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4f270-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="4f270-144">False</span><span class="sxs-lookup"><span data-stu-id="4f270-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f270-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4f270-145">See also</span></span>



[<span data-ttu-id="4f270-146">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4f270-146">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="4f270-147">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="4f270-147">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

