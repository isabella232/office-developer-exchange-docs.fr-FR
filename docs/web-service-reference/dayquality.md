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
description: L’élément DayQuality représente la qualité du jour pour le temps de réunion suggéré pour la qualité.
ms.openlocfilehash: 41cc8313dccb1a5172fefc167e6ed90a21109ec5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455113"
---
# <a name="dayquality"></a><span data-ttu-id="904ac-103">DayQuality</span><span class="sxs-lookup"><span data-stu-id="904ac-103">DayQuality</span></span>

<span data-ttu-id="904ac-104">L’élément **DayQuality** représente la qualité du jour pour le temps de réunion suggéré pour la qualité.</span><span class="sxs-lookup"><span data-stu-id="904ac-104">The **DayQuality** element represents the quality of the day for containing quality suggested meeting times.</span></span> 
  
- [<span data-ttu-id="904ac-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="904ac-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="904ac-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="904ac-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="904ac-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="904ac-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="904ac-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="904ac-108">SuggestionDayResult</span></span>](suggestiondayresult.md) 
- [<span data-ttu-id="904ac-109">DayQuality</span><span class="sxs-lookup"><span data-stu-id="904ac-109">DayQuality</span></span>](dayquality.md)
  
```xml
<DayQuality>Excellent or Good or Fair or Poor</DayQuality>
```

<span data-ttu-id="904ac-110">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="904ac-110">**SuggestionQuality**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="904ac-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="904ac-111">Attributes and elements</span></span>

<span data-ttu-id="904ac-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="904ac-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="904ac-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="904ac-113">Attributes</span></span>

<span data-ttu-id="904ac-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="904ac-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="904ac-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="904ac-115">Child elements</span></span>

<span data-ttu-id="904ac-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="904ac-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="904ac-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="904ac-117">Parent elements</span></span>

|<span data-ttu-id="904ac-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="904ac-118">**Element**</span></span>|<span data-ttu-id="904ac-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="904ac-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="904ac-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="904ac-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="904ac-121">Représente un jour qui contient des heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="904ac-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="904ac-122">Voici l’expression XPath 2,0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="904ac-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="904ac-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="904ac-123">Text value</span></span>

<span data-ttu-id="904ac-124">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="904ac-124">A text value is required.</span></span> <span data-ttu-id="904ac-125">Les valeurs possibles pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="904ac-125">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="904ac-126">**Excellente**</span><span class="sxs-lookup"><span data-stu-id="904ac-126">**Excellent**</span></span>   
- <span data-ttu-id="904ac-127">**Good**</span><span class="sxs-lookup"><span data-stu-id="904ac-127">**Good**</span></span>    
- <span data-ttu-id="904ac-128">**Beau**</span><span class="sxs-lookup"><span data-stu-id="904ac-128">**Fair**</span></span>    
- <span data-ttu-id="904ac-129">**Mauvais**</span><span class="sxs-lookup"><span data-stu-id="904ac-129">**Poor**</span></span>
    
## <a name="remarks"></a><span data-ttu-id="904ac-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="904ac-130">Remarks</span></span>

<span data-ttu-id="904ac-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="904ac-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="904ac-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="904ac-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="904ac-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="904ac-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="904ac-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="904ac-134">Schema Name</span></span>  <br/> |<span data-ttu-id="904ac-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="904ac-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="904ac-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="904ac-136">Validation File</span></span>  <br/> |<span data-ttu-id="904ac-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="904ac-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="904ac-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="904ac-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="904ac-139">False</span><span class="sxs-lookup"><span data-stu-id="904ac-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="904ac-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="904ac-140">See also</span></span>

- [<span data-ttu-id="904ac-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="904ac-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="904ac-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="904ac-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="904ac-143">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="904ac-143">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

