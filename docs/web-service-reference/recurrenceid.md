---
title: RecurrenceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurrenceId
api_type:
- schema
ms.assetid: 9ef3569d-ee56-4b22-b008-609fb3337da7
description: L’élément RecurrenceId est utilisé pour identifier une instance spécifique d’un élément de calendrier périodique.
ms.openlocfilehash: 078bec85e1ca1530137f9935365d7dd3e530ea34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829005"
---
# <a name="recurrenceid"></a><span data-ttu-id="996c8-103">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="996c8-103">RecurrenceId</span></span>

<span data-ttu-id="996c8-104">L’élément **RecurrenceId** est utilisé pour identifier une instance spécifique d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="996c8-104">The **RecurrenceId** element is used to identify a specific instance of a recurring calendar item.</span></span> 
  
```xml
<RecurrenceId/>
```

 <span data-ttu-id="996c8-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="996c8-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="996c8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="996c8-106">Attributes and elements</span></span>

<span data-ttu-id="996c8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="996c8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="996c8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="996c8-108">Attributes</span></span>

<span data-ttu-id="996c8-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="996c8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="996c8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="996c8-110">Child elements</span></span>

<span data-ttu-id="996c8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="996c8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="996c8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="996c8-112">Parent elements</span></span>

|<span data-ttu-id="996c8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="996c8-113">**Element**</span></span>|<span data-ttu-id="996c8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="996c8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="996c8-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="996c8-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="996c8-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="996c8-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="996c8-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="996c8-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="996c8-118">Représente un message de réunion.</span><span class="sxs-lookup"><span data-stu-id="996c8-118">Represents a meeting message.</span></span>  <br/> |
|[<span data-ttu-id="996c8-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="996c8-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="996c8-120">Représente une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="996c8-120">Represents a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="996c8-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="996c8-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="996c8-122">Représente une réponse à une réunion.</span><span class="sxs-lookup"><span data-stu-id="996c8-122">Represents a meeting response.</span></span>  <br/> |
|[<span data-ttu-id="996c8-123">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="996c8-123">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="996c8-124">Représente une annulation de réunion.</span><span class="sxs-lookup"><span data-stu-id="996c8-124">Represents a meeting cancellation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="996c8-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="996c8-125">Text value</span></span>

<span data-ttu-id="996c8-126">La valeur de texte représente une valeur de date/heure qui identifie une occurrence de calendrier.</span><span class="sxs-lookup"><span data-stu-id="996c8-126">The text value represents a date/time value that identifies a calendar occurrence.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="996c8-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="996c8-127">Remarks</span></span>

<span data-ttu-id="996c8-128">Cette propriété est utilisée avec la propriété [UID](uid.md) pour identifier une instance spécifique d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="996c8-128">This property is used with the [UID](uid.md) property to identify a specific instance of a recurring calendar item.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="996c8-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="996c8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="996c8-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="996c8-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="996c8-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="996c8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="996c8-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="996c8-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="996c8-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="996c8-133">Validation File</span></span>  <br/> |<span data-ttu-id="996c8-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="996c8-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="996c8-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="996c8-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="996c8-136">False</span><span class="sxs-lookup"><span data-stu-id="996c8-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="996c8-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="996c8-137">See also</span></span>



- [<span data-ttu-id="996c8-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="996c8-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

