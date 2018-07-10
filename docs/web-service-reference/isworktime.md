---
title: IsWorkTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsWorkTime
api_type:
- schema
ms.assetid: 5243dd19-3593-4a81-bb2d-90496e04cb98
description: L’élément IsWorkTime indique l’heure de réunion proposée se produit pendant les heures de travail prévu.
ms.openlocfilehash: c687b29df226ebb28cdf01d3a2da62590f790924
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828135"
---
# <a name="isworktime"></a><span data-ttu-id="4f2d7-103">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="4f2d7-103">IsWorkTime</span></span>

<span data-ttu-id="4f2d7-104">L’élément **IsWorkTime** indique l’heure de réunion proposée se produit pendant les heures de travail prévu.</span><span class="sxs-lookup"><span data-stu-id="4f2d7-104">The **IsWorkTime** element represents whether the suggested meeting time occurs during scheduled work hours.</span></span> 
  
[<span data-ttu-id="4f2d7-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4f2d7-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="4f2d7-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="4f2d7-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="4f2d7-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="4f2d7-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="4f2d7-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="4f2d7-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="4f2d7-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="4f2d7-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="4f2d7-110">Suggestion</span><span class="sxs-lookup"><span data-stu-id="4f2d7-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="4f2d7-111">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="4f2d7-111">IsWorkTime</span></span>](isworktime.md)
  
```xml
<IsWorkTime>true or false</IsWorkTime>
```

 <span data-ttu-id="4f2d7-112">**boolean**</span><span class="sxs-lookup"><span data-stu-id="4f2d7-112">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f2d7-113">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4f2d7-113">Attributes and elements</span></span>

<span data-ttu-id="4f2d7-114">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4f2d7-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f2d7-115">Attributs</span><span class="sxs-lookup"><span data-stu-id="4f2d7-115">Attributes</span></span>

<span data-ttu-id="4f2d7-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4f2d7-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f2d7-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4f2d7-117">Child elements</span></span>

<span data-ttu-id="4f2d7-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4f2d7-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4f2d7-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4f2d7-119">Parent elements</span></span>

|<span data-ttu-id="4f2d7-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4f2d7-120">**Element**</span></span>|<span data-ttu-id="4f2d7-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f2d7-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f2d7-122">Suggestion</span><span class="sxs-lookup"><span data-stu-id="4f2d7-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="4f2d7-123">Représente une seule suggestion de l’heure de la réunion.</span><span class="sxs-lookup"><span data-stu-id="4f2d7-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="4f2d7-124">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="4f2d7-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4f2d7-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4f2d7-125">Text value</span></span>

<span data-ttu-id="4f2d7-126">Une valeur de texte qui représente une valeur Boolean est requise.</span><span class="sxs-lookup"><span data-stu-id="4f2d7-126">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4f2d7-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="4f2d7-127">Remarks</span></span>

<span data-ttu-id="4f2d7-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4f2d7-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f2d7-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4f2d7-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f2d7-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4f2d7-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4f2d7-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4f2d7-131">Schema Name</span></span>  <br/> |<span data-ttu-id="4f2d7-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4f2d7-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="4f2d7-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4f2d7-133">Validation File</span></span>  <br/> |<span data-ttu-id="4f2d7-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4f2d7-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4f2d7-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4f2d7-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="4f2d7-136">False</span><span class="sxs-lookup"><span data-stu-id="4f2d7-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f2d7-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4f2d7-137">See also</span></span>



[<span data-ttu-id="4f2d7-138">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4f2d7-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="4f2d7-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4f2d7-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="4f2d7-140">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="4f2d7-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
