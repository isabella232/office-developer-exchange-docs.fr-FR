---
title: Date
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Date
api_type:
- schema
ms.assetid: 2f6bc090-fff4-45b1-8d7e-8fd6e060cce2
description: L’élément Date représente la date qui contient les heures de réunion proposée.
ms.openlocfilehash: 98dc9d6c599222c819b2c9ed1bacd05758ae1655
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755795"
---
# <a name="date"></a><span data-ttu-id="8040e-103">Date</span><span class="sxs-lookup"><span data-stu-id="8040e-103">Date</span></span>

<span data-ttu-id="8040e-104">L’élément **Date** représente la date qui contient les heures de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="8040e-104">The **Date** element represents the date that contains the suggested meeting times.</span></span> 
  
- [<span data-ttu-id="8040e-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="8040e-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) 
- [<span data-ttu-id="8040e-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="8040e-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="8040e-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="8040e-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="8040e-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="8040e-108">SuggestionDayResult</span></span>](suggestiondayresult.md)  
- [<span data-ttu-id="8040e-109">Date</span><span class="sxs-lookup"><span data-stu-id="8040e-109">Date</span></span>](date.md)
  
```xml
<Date>...</Date>
```

<span data-ttu-id="8040e-110">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="8040e-110">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8040e-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8040e-111">Attributes and elements</span></span>

<span data-ttu-id="8040e-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8040e-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8040e-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="8040e-113">Attributes</span></span>

<span data-ttu-id="8040e-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8040e-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8040e-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8040e-115">Child elements</span></span>

<span data-ttu-id="8040e-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8040e-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8040e-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8040e-117">Parent elements</span></span>

|<span data-ttu-id="8040e-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8040e-118">**Element**</span></span>|<span data-ttu-id="8040e-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="8040e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8040e-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="8040e-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="8040e-121">Représente un seul jour qui contient les heures de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="8040e-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="8040e-122">Vous trouverez ci-dessous l’expression XPath 2.0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="8040e-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8040e-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8040e-123">Text value</span></span>

<span data-ttu-id="8040e-124">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="8040e-124">A text value is required.</span></span> <span data-ttu-id="8040e-125">Passez en revue les recommandations de type de données de schéma World Wide Web Consortium (W3C) pour le format du type de données primitif dateTime.</span><span class="sxs-lookup"><span data-stu-id="8040e-125">Review the World Wide Web Consortium (W3C) schema datatype recommendations for the format of the dateTime primitive datatype.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8040e-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="8040e-126">Remarks</span></span>

<span data-ttu-id="8040e-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8040e-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8040e-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8040e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8040e-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8040e-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8040e-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8040e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="8040e-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8040e-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="8040e-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8040e-132">Validation File</span></span>  <br/> |<span data-ttu-id="8040e-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8040e-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8040e-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8040e-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="8040e-135">False</span><span class="sxs-lookup"><span data-stu-id="8040e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8040e-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8040e-136">See also</span></span>

- [<span data-ttu-id="8040e-137">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="8040e-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="8040e-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="8040e-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="8040e-139">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="8040e-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

