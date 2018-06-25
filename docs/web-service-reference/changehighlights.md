---
title: ChangeHighlights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: Demander les ChangeHighlights élément spécifie ce qui a changé entre deux versions d’une réunion.
ms.openlocfilehash: 5fe7aa95f60ae95f1af24e8f7a0463ad49716f65
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755501"
---
# <a name="changehighlights"></a><span data-ttu-id="b67db-103">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="b67db-103">ChangeHighlights</span></span>

<span data-ttu-id="b67db-104">L’élément **ChangeHighlights** spécifie ce qui a changé entre deux versions d’une réunion message de demande.</span><span class="sxs-lookup"><span data-stu-id="b67db-104">The **ChangeHighlights** element specifies what has changed between two versions of a meeting request message.</span></span> 
  
```XML
<ChangeHighlights>
    <HasLocationChanged></HasLocationChanged>
    <Location></Location>
    <HasStartTimeChanged></HasStartTimeChanged>
    <Start></Start>
    <HasEndTimeChanged></HasEndTimeChanged>
    <End></End>
</ChangeHighlights>
```

 <span data-ttu-id="b67db-105">**ChangeHighlightsType**</span><span class="sxs-lookup"><span data-stu-id="b67db-105">**ChangeHighlightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b67db-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b67db-106">Attributes and elements</span></span>

<span data-ttu-id="b67db-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b67db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b67db-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b67db-108">Attributes</span></span>

<span data-ttu-id="b67db-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b67db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b67db-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b67db-110">Child elements</span></span>

|<span data-ttu-id="b67db-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b67db-111">**Element**</span></span>|<span data-ttu-id="b67db-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b67db-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b67db-113">HasLocationChanged</span><span class="sxs-lookup"><span data-stu-id="b67db-113">HasLocationChanged</span></span>](haslocationchanged.md) <br/> |<span data-ttu-id="b67db-114">Spécifie si la propriété location d’une réunion a été modifiée.</span><span class="sxs-lookup"><span data-stu-id="b67db-114">Specifies whether the location property of a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="b67db-115">Location</span><span class="sxs-lookup"><span data-stu-id="b67db-115">Location</span></span>](location.md) <br/> |<span data-ttu-id="b67db-116">Représente l’emplacement d’une réunion ou un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="b67db-116">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="b67db-117">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="b67db-117">HasStartTimeChanged</span></span>](hasstarttimechanged.md) <br/> |<span data-ttu-id="b67db-118">Spécifie si l’heure de début d’une réunion a été modifiée.</span><span class="sxs-lookup"><span data-stu-id="b67db-118">Specifies whether the start time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="b67db-119">Début</span><span class="sxs-lookup"><span data-stu-id="b67db-119">Start</span></span>](start.md) <br/> |<span data-ttu-id="b67db-120">Représente le début d’une durée.</span><span class="sxs-lookup"><span data-stu-id="b67db-120">Represents the start of a duration.</span></span>  <br/> |
|[<span data-ttu-id="b67db-121">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="b67db-121">HasEndTimeChanged</span></span>](hasendtimechanged.md) <br/> |<span data-ttu-id="b67db-122">Spécifie si l’heure de fin d’une réunion a été modifiée.</span><span class="sxs-lookup"><span data-stu-id="b67db-122">Specifies whether the end time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="b67db-123">Fin</span><span class="sxs-lookup"><span data-stu-id="b67db-123">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b67db-124">Représente la fin d’une durée.</span><span class="sxs-lookup"><span data-stu-id="b67db-124">Represents the end of a duration.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b67db-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b67db-125">Parent elements</span></span>

|<span data-ttu-id="b67db-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b67db-126">**Element**</span></span>|<span data-ttu-id="b67db-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="b67db-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b67db-128">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b67db-128">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b67db-129">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b67db-129">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b67db-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="b67db-130">Remarks</span></span>

<span data-ttu-id="b67db-131">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b67db-131">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b67db-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b67db-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b67db-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b67db-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b67db-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b67db-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b67db-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b67db-135">Schema Name</span></span>  <br/> |<span data-ttu-id="b67db-136">Schéma type</span><span class="sxs-lookup"><span data-stu-id="b67db-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="b67db-137">Validation File</span><span class="sxs-lookup"><span data-stu-id="b67db-137">Validation File</span></span>  <br/> |<span data-ttu-id="b67db-138">types.xsd</span><span class="sxs-lookup"><span data-stu-id="b67db-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b67db-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b67db-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b67db-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b67db-140">See also</span></span>



- [<span data-ttu-id="b67db-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b67db-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

