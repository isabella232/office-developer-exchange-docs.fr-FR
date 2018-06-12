---
title: DayQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayQuality
api_type:
- schema
ms.assetid: cd0eb239-6e7f-4a5a-b245-659f170550b7
description: L’élément DayQuality représente la qualité de la journée contenant les heures de réunions suggéré de qualité.
ms.openlocfilehash: 156d5bc58d481c9c812793da4722272ac76adaad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755827"
---
# <a name="dayquality"></a><span data-ttu-id="ebf62-103">DayQuality</span><span class="sxs-lookup"><span data-stu-id="ebf62-103">DayQuality</span></span>

<span data-ttu-id="ebf62-104">L’élément **DayQuality** représente la qualité de la journée contenant qualité suggérée aux heures de réunion.</span><span class="sxs-lookup"><span data-stu-id="ebf62-104">The **DayQuality** element represents the quality of the day for containing quality suggested meeting times.</span></span> 
  
- [<span data-ttu-id="ebf62-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ebf62-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="ebf62-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="ebf62-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="ebf62-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="ebf62-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="ebf62-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="ebf62-108">SuggestionDayResult</span></span>](suggestiondayresult.md) 
- [<span data-ttu-id="ebf62-109">DayQuality</span><span class="sxs-lookup"><span data-stu-id="ebf62-109">DayQuality</span></span>](dayquality.md)
  
```xml
<DayQuality>Excellent or Good or Fair or Poor</DayQuality>
```

<span data-ttu-id="ebf62-110">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="ebf62-110">**SuggestionQuality**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ebf62-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ebf62-111">Attributes and elements</span></span>

<span data-ttu-id="ebf62-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ebf62-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ebf62-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="ebf62-113">Attributes</span></span>

<span data-ttu-id="ebf62-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ebf62-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ebf62-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ebf62-115">Child elements</span></span>

<span data-ttu-id="ebf62-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ebf62-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ebf62-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ebf62-117">Parent elements</span></span>

|<span data-ttu-id="ebf62-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ebf62-118">**Element**</span></span>|<span data-ttu-id="ebf62-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="ebf62-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ebf62-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="ebf62-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="ebf62-121">Représente un seul jour qui contient les heures de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="ebf62-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="ebf62-122">Vous trouverez ci-dessous l’expression XPath 2.0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="ebf62-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ebf62-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ebf62-123">Text value</span></span>

<span data-ttu-id="ebf62-124">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="ebf62-124">A text value is required.</span></span> <span data-ttu-id="ebf62-125">Les valeurs possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="ebf62-125">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="ebf62-126">**Excellente**</span><span class="sxs-lookup"><span data-stu-id="ebf62-126">**Excellent**</span></span>   
- <span data-ttu-id="ebf62-127">**Une bonne**</span><span class="sxs-lookup"><span data-stu-id="ebf62-127">**Good**</span></span>    
- <span data-ttu-id="ebf62-128">**Juste**</span><span class="sxs-lookup"><span data-stu-id="ebf62-128">**Fair**</span></span>    
- <span data-ttu-id="ebf62-129">**Une mauvaise**</span><span class="sxs-lookup"><span data-stu-id="ebf62-129">**Poor**</span></span>
    
## <a name="remarks"></a><span data-ttu-id="ebf62-130">Note</span><span class="sxs-lookup"><span data-stu-id="ebf62-130">Remarks</span></span>

<span data-ttu-id="ebf62-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ebf62-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ebf62-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ebf62-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ebf62-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ebf62-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ebf62-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ebf62-134">Schema Name</span></span>  <br/> |<span data-ttu-id="ebf62-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ebf62-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="ebf62-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ebf62-136">Validation File</span></span>  <br/> |<span data-ttu-id="ebf62-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ebf62-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ebf62-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ebf62-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="ebf62-139">False</span><span class="sxs-lookup"><span data-stu-id="ebf62-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ebf62-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ebf62-140">See also</span></span>

- [<span data-ttu-id="ebf62-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ebf62-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="ebf62-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ebf62-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="ebf62-143">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="ebf62-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

