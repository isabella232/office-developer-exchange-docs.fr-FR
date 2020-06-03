---
title: SuggestionArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionArray
api_type:
- schema
ms.assetid: c1c26008-7b14-4563-8db5-bceb0f475b1b
description: L’élément SuggestionArray contient un tableau de suggestions de réunion.
ms.openlocfilehash: ec982417c39569820beef82ae837eacbe316740c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466674"
---
# <a name="suggestionarray"></a><span data-ttu-id="b0810-103">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="b0810-103">SuggestionArray</span></span>

<span data-ttu-id="b0810-104">L’élément **SuggestionArray** contient un tableau de suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="b0810-104">The **SuggestionArray** element contains an array of meeting suggestions.</span></span> 
  
[<span data-ttu-id="b0810-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b0810-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="b0810-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="b0810-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="b0810-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="b0810-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="b0810-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="b0810-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="b0810-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="b0810-109">SuggestionArray</span></span>](suggestionarray.md)
  
```xml
<SuggestionArray>
   <Suggestion>...</Suggestion>
</SuggestionArray>
```

 <span data-ttu-id="b0810-110">**ArrayOfSuggestion**</span><span class="sxs-lookup"><span data-stu-id="b0810-110">**ArrayOfSuggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0810-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b0810-111">Attributes and elements</span></span>

<span data-ttu-id="b0810-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b0810-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0810-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="b0810-113">Attributes</span></span>

<span data-ttu-id="b0810-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b0810-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0810-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b0810-115">Child elements</span></span>

|<span data-ttu-id="b0810-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b0810-116">**Element**</span></span>|<span data-ttu-id="b0810-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0810-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0810-118">Suggérer</span><span class="sxs-lookup"><span data-stu-id="b0810-118">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="b0810-119">Représente une seule suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="b0810-119">Represents a single meeting suggestion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0810-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b0810-120">Parent elements</span></span>

|<span data-ttu-id="b0810-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b0810-121">**Element**</span></span>|<span data-ttu-id="b0810-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0810-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0810-123">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="b0810-123">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="b0810-124">Représente un jour qui contient des heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="b0810-124">Represents a single day that contains suggested meeting times.</span></span>  <br/> <span data-ttu-id="b0810-125">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="b0810-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b0810-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="b0810-126">Remarks</span></span>

<span data-ttu-id="b0810-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b0810-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0810-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b0810-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0810-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b0810-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0810-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b0810-130">Schema Name</span></span>  <br/> |<span data-ttu-id="b0810-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b0810-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0810-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b0810-132">Validation File</span></span>  <br/> |<span data-ttu-id="b0810-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b0810-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0810-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b0810-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0810-135">False</span><span class="sxs-lookup"><span data-stu-id="b0810-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0810-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b0810-136">See also</span></span>



[<span data-ttu-id="b0810-137">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b0810-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b0810-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b0810-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b0810-139">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="b0810-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

