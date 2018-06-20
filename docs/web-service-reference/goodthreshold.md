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
description: L’élément GoodThreshold indique le pourcentage des participants qui doivent ouvrir la période de temps afin que la période de temps être considérée comme une heure de réunion proposée bonne.
ms.openlocfilehash: 8044cb2b52cb572fad8731253dffa34de9d097fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827746"
---
# <a name="goodthreshold"></a><span data-ttu-id="a562c-103">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="a562c-103">GoodThreshold</span></span>

<span data-ttu-id="a562c-104">L’élément **GoodThreshold** indique le pourcentage des participants qui doivent ouvrir la période de temps afin que la période de temps être considérée comme une heure de réunion proposée bonne.</span><span class="sxs-lookup"><span data-stu-id="a562c-104">The **GoodThreshold** element specifies the percentage of attendees that must have the time period open in order for the time period to qualify as a Good suggested meeting time.</span></span> 
  
[<span data-ttu-id="a562c-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="a562c-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="a562c-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="a562c-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="a562c-107">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="a562c-107">GoodThreshold</span></span>](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 <span data-ttu-id="a562c-108">**int**</span><span class="sxs-lookup"><span data-stu-id="a562c-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a562c-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a562c-109">Attributes and elements</span></span>

<span data-ttu-id="a562c-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a562c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a562c-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="a562c-111">Attributes</span></span>

<span data-ttu-id="a562c-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a562c-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a562c-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a562c-113">Child elements</span></span>

<span data-ttu-id="a562c-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a562c-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a562c-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a562c-115">Parent elements</span></span>

|<span data-ttu-id="a562c-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a562c-116">**Element**</span></span>|<span data-ttu-id="a562c-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="a562c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a562c-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="a562c-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="a562c-119">Contient les options permettant d’obtenir des informations de suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="a562c-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="a562c-120">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="a562c-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a562c-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a562c-121">Text value</span></span>

<span data-ttu-id="a562c-122">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="a562c-122">A text value is required.</span></span> <span data-ttu-id="a562c-123">Les valeurs entières attendue sont compris entre 0 et 50.</span><span class="sxs-lookup"><span data-stu-id="a562c-123">The expected integer values are between 0 and 50.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a562c-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="a562c-124">Remarks</span></span>

<span data-ttu-id="a562c-125">Cet élément est obligatoire si l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="a562c-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> <span data-ttu-id="a562c-126">L’élément **GoodThreshold** détermine également les réunions sont considérés comme étant correcte.</span><span class="sxs-lookup"><span data-stu-id="a562c-126">The **GoodThreshold** element also determines what meetings are considered Fair.</span></span> <span data-ttu-id="a562c-127">Il est que le pourcentage des participants présentant des conflits est qu'inférieure supérieur au seuil d’une bonne et supérieure à 50 %, l’heure de réunion proposée qualifiant aussi juste.</span><span class="sxs-lookup"><span data-stu-id="a562c-127">It the percentage of attendees with conflicts is less than the Good Threshold and higher than 50 percent, the suggested meeting time qualifies as Fair.</span></span> <span data-ttu-id="a562c-128">Le seuil en plus de 50 désigne le pourcentage qui définit le seuil du bon/équitable.</span><span class="sxs-lookup"><span data-stu-id="a562c-128">The Good Threshold plus 50 equals the percentage that defines the Good/Fair threshold.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a562c-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a562c-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="a562c-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a562c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a562c-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a562c-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a562c-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a562c-132">Schema Name</span></span>  <br/> |<span data-ttu-id="a562c-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a562c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="a562c-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a562c-134">Validation File</span></span>  <br/> |<span data-ttu-id="a562c-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a562c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a562c-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a562c-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="a562c-137">False</span><span class="sxs-lookup"><span data-stu-id="a562c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a562c-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a562c-138">See also</span></span>



[<span data-ttu-id="a562c-139">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a562c-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="a562c-140">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="a562c-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

