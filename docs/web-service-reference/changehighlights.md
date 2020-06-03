---
title: ChangeHighlights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: L’élément ChangeHighlights spécifie les modifications apportées entre deux versions d’un message de demande de réunion.
ms.openlocfilehash: 6c78d2c96449ee41032859f90bf51d6e0faa92ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463278"
---
# <a name="changehighlights"></a><span data-ttu-id="c4bb2-103">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="c4bb2-103">ChangeHighlights</span></span>

<span data-ttu-id="c4bb2-104">L’élément **ChangeHighlights** spécifie les modifications apportées entre deux versions d’un message de demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-104">The **ChangeHighlights** element specifies what has changed between two versions of a meeting request message.</span></span> 
  
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

 <span data-ttu-id="c4bb2-105">**ChangeHighlightsType**</span><span class="sxs-lookup"><span data-stu-id="c4bb2-105">**ChangeHighlightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4bb2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c4bb2-106">Attributes and elements</span></span>

<span data-ttu-id="c4bb2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4bb2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c4bb2-108">Attributes</span></span>

<span data-ttu-id="c4bb2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4bb2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c4bb2-110">Child elements</span></span>

|<span data-ttu-id="c4bb2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c4bb2-111">**Element**</span></span>|<span data-ttu-id="c4bb2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c4bb2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4bb2-113">HasLocationChanged</span><span class="sxs-lookup"><span data-stu-id="c4bb2-113">HasLocationChanged</span></span>](haslocationchanged.md) <br/> |<span data-ttu-id="c4bb2-114">Indique si la propriété Location d’une réunion a été modifiée.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-114">Specifies whether the location property of a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="c4bb2-115">Emplacement</span><span class="sxs-lookup"><span data-stu-id="c4bb2-115">Location</span></span>](location.md) <br/> |<span data-ttu-id="c4bb2-116">Représente l’emplacement d’une réunion ou d’un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-116">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="c4bb2-117">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="c4bb2-117">HasStartTimeChanged</span></span>](hasstarttimechanged.md) <br/> |<span data-ttu-id="c4bb2-118">Indique si l’heure de début d’une réunion a changé.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-118">Specifies whether the start time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="c4bb2-119">Démarrage</span><span class="sxs-lookup"><span data-stu-id="c4bb2-119">Start</span></span>](start.md) <br/> |<span data-ttu-id="c4bb2-120">Représente le début d’une durée.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-120">Represents the start of a duration.</span></span>  <br/> |
|[<span data-ttu-id="c4bb2-121">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="c4bb2-121">HasEndTimeChanged</span></span>](hasendtimechanged.md) <br/> |<span data-ttu-id="c4bb2-122">Indique si l’heure de fin d’une réunion a changé.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-122">Specifies whether the end time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="c4bb2-123">Fin</span><span class="sxs-lookup"><span data-stu-id="c4bb2-123">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c4bb2-124">Représente la fin d’une durée.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-124">Represents the end of a duration.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c4bb2-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c4bb2-125">Parent elements</span></span>

|<span data-ttu-id="c4bb2-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c4bb2-126">**Element**</span></span>|<span data-ttu-id="c4bb2-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="c4bb2-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4bb2-128">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="c4bb2-128">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c4bb2-129">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-129">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c4bb2-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="c4bb2-130">Remarks</span></span>

<span data-ttu-id="c4bb2-131">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-131">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c4bb2-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4bb2-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4bb2-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c4bb2-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4bb2-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c4bb2-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c4bb2-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c4bb2-135">Schema Name</span></span>  <br/> |<span data-ttu-id="c4bb2-136">Schéma type</span><span class="sxs-lookup"><span data-stu-id="c4bb2-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="c4bb2-137">Validation File</span><span class="sxs-lookup"><span data-stu-id="c4bb2-137">Validation File</span></span>  <br/> |<span data-ttu-id="c4bb2-138">types. xsd</span><span class="sxs-lookup"><span data-stu-id="c4bb2-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c4bb2-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c4bb2-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c4bb2-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c4bb2-140">See also</span></span>



- [<span data-ttu-id="c4bb2-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c4bb2-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

