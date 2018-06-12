---
title: MeetingDurationInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingDurationInMinutes
api_type:
- schema
ms.assetid: bb86b275-9c29-4daf-8196-8d505b87a4f4
description: L’élément MeetingDurationInMinutes spécifie la durée de la réunion suggérée.
ms.openlocfilehash: 2ff60b69fb352c2ac7316f1ca231bb04da67ead2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828433"
---
# <a name="meetingdurationinminutes"></a><span data-ttu-id="91f0f-103">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="91f0f-103">MeetingDurationInMinutes</span></span>

<span data-ttu-id="91f0f-104">L’élément **MeetingDurationInMinutes** spécifie la durée de la réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="91f0f-104">The **MeetingDurationInMinutes** element specifies the duration of the meeting to be suggested.</span></span> 
  
[<span data-ttu-id="91f0f-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="91f0f-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="91f0f-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="91f0f-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="91f0f-107">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="91f0f-107">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md)
  
```xml
<MeetingDurationInMinutes>...</MeetingDurationInMinutes>
```

 <span data-ttu-id="91f0f-108">**int**</span><span class="sxs-lookup"><span data-stu-id="91f0f-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91f0f-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="91f0f-109">Attributes and elements</span></span>

<span data-ttu-id="91f0f-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="91f0f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91f0f-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="91f0f-111">Attributes</span></span>

<span data-ttu-id="91f0f-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="91f0f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91f0f-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="91f0f-113">Child elements</span></span>

<span data-ttu-id="91f0f-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="91f0f-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91f0f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="91f0f-115">Parent elements</span></span>

|<span data-ttu-id="91f0f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="91f0f-116">**Element**</span></span>|<span data-ttu-id="91f0f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="91f0f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91f0f-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="91f0f-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="91f0f-119">Contient les options permettant d’obtenir des informations de suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="91f0f-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="91f0f-120">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="91f0f-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91f0f-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="91f0f-121">Text value</span></span>

<span data-ttu-id="91f0f-122">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="91f0f-122">A text value is required.</span></span> <span data-ttu-id="91f0f-123">La valeur de texte représente un entier.</span><span class="sxs-lookup"><span data-stu-id="91f0f-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="91f0f-124">Note</span><span class="sxs-lookup"><span data-stu-id="91f0f-124">Remarks</span></span>

<span data-ttu-id="91f0f-125">Cet élément est obligatoire si l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="91f0f-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="91f0f-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="91f0f-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="91f0f-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="91f0f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91f0f-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="91f0f-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91f0f-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="91f0f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="91f0f-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="91f0f-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="91f0f-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="91f0f-131">Validation File</span></span>  <br/> |<span data-ttu-id="91f0f-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91f0f-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91f0f-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="91f0f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="91f0f-134">False</span><span class="sxs-lookup"><span data-stu-id="91f0f-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91f0f-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="91f0f-135">See also</span></span>



[<span data-ttu-id="91f0f-136">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="91f0f-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="91f0f-137">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="91f0f-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

