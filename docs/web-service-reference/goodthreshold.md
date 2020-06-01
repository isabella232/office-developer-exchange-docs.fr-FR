---
title: GoodThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GoodThreshold
api_type:
- schema
ms.assetid: 68f607f5-7271-46a6-8ffc-91878185a683
description: L’élément GoodThreshold spécifie le pourcentage de participants qui doivent avoir la période de temps ouverte pour que la période puisse être considérée comme une heure de réunion recommandée.
ms.openlocfilehash: 34ea433ad7315d61df8cf8e22bae1166d3210af3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457311"
---
# <a name="goodthreshold"></a><span data-ttu-id="f582f-103">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="f582f-103">GoodThreshold</span></span>

<span data-ttu-id="f582f-104">L’élément **GoodThreshold** spécifie le pourcentage de participants qui doivent avoir la période de temps ouverte pour que la période puisse être considérée comme une heure de réunion recommandée.</span><span class="sxs-lookup"><span data-stu-id="f582f-104">The **GoodThreshold** element specifies the percentage of attendees that must have the time period open in order for the time period to qualify as a Good suggested meeting time.</span></span> 
  
[<span data-ttu-id="f582f-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="f582f-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="f582f-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="f582f-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="f582f-107">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="f582f-107">GoodThreshold</span></span>](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 <span data-ttu-id="f582f-108">**int**</span><span class="sxs-lookup"><span data-stu-id="f582f-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f582f-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f582f-109">Attributes and elements</span></span>

<span data-ttu-id="f582f-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f582f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f582f-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="f582f-111">Attributes</span></span>

<span data-ttu-id="f582f-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f582f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f582f-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f582f-113">Child elements</span></span>

<span data-ttu-id="f582f-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f582f-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f582f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f582f-115">Parent elements</span></span>

|<span data-ttu-id="f582f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f582f-116">**Element**</span></span>|<span data-ttu-id="f582f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="f582f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f582f-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="f582f-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="f582f-119">Contient les options permettant d’obtenir des informations sur les suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="f582f-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="f582f-120">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="f582f-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f582f-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f582f-121">Text value</span></span>

<span data-ttu-id="f582f-122">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="f582f-122">A text value is required.</span></span> <span data-ttu-id="f582f-123">Les valeurs d’entier attendues sont comprises entre 0 et 50.</span><span class="sxs-lookup"><span data-stu-id="f582f-123">The expected integer values are between 0 and 50.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f582f-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="f582f-124">Remarks</span></span>

<span data-ttu-id="f582f-125">Cet élément est requis si l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="f582f-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> <span data-ttu-id="f582f-126">L’élément **GoodThreshold** détermine également les réunions considérées comme équitable.</span><span class="sxs-lookup"><span data-stu-id="f582f-126">The **GoodThreshold** element also determines what meetings are considered Fair.</span></span> <span data-ttu-id="f582f-127">Si le pourcentage de participants avec des conflits est inférieur au seuil de bonne qualité et supérieur à 50%, la durée de réunion suggérée est considérée comme équitable.</span><span class="sxs-lookup"><span data-stu-id="f582f-127">It the percentage of attendees with conflicts is less than the Good Threshold and higher than 50 percent, the suggested meeting time qualifies as Fair.</span></span> <span data-ttu-id="f582f-128">Le seuil de qualité plus 50 est égal au pourcentage qui définit le seuil correct/équitable.</span><span class="sxs-lookup"><span data-stu-id="f582f-128">The Good Threshold plus 50 equals the percentage that defines the Good/Fair threshold.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f582f-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f582f-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f582f-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f582f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f582f-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f582f-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f582f-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f582f-132">Schema Name</span></span>  <br/> |<span data-ttu-id="f582f-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f582f-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="f582f-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f582f-134">Validation File</span></span>  <br/> |<span data-ttu-id="f582f-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f582f-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f582f-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f582f-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="f582f-137">False</span><span class="sxs-lookup"><span data-stu-id="f582f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f582f-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f582f-138">See also</span></span>



[<span data-ttu-id="f582f-139">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f582f-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="f582f-140">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="f582f-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

