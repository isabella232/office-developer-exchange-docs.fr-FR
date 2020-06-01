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
ms.openlocfilehash: 58a379f2cffa7ff37181e93ad1c45c9752e84f1d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461610"
---
# <a name="recurrenceid"></a><span data-ttu-id="a497c-103">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="a497c-103">RecurrenceId</span></span>

<span data-ttu-id="a497c-104">L’élément **RecurrenceId** est utilisé pour identifier une instance spécifique d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="a497c-104">The **RecurrenceId** element is used to identify a specific instance of a recurring calendar item.</span></span> 
  
```xml
<RecurrenceId/>
```

 <span data-ttu-id="a497c-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="a497c-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a497c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a497c-106">Attributes and elements</span></span>

<span data-ttu-id="a497c-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a497c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a497c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a497c-108">Attributes</span></span>

<span data-ttu-id="a497c-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a497c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a497c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a497c-110">Child elements</span></span>

<span data-ttu-id="a497c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a497c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a497c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a497c-112">Parent elements</span></span>

|<span data-ttu-id="a497c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a497c-113">**Element**</span></span>|<span data-ttu-id="a497c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a497c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a497c-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a497c-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a497c-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="a497c-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a497c-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="a497c-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="a497c-118">Représente un message de réunion.</span><span class="sxs-lookup"><span data-stu-id="a497c-118">Represents a meeting message.</span></span>  <br/> |
|[<span data-ttu-id="a497c-119">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="a497c-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a497c-120">Représente une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="a497c-120">Represents a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="a497c-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="a497c-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="a497c-122">Représente une réponse à une réunion.</span><span class="sxs-lookup"><span data-stu-id="a497c-122">Represents a meeting response.</span></span>  <br/> |
|[<span data-ttu-id="a497c-123">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="a497c-123">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="a497c-124">Représente une annulation de réunion.</span><span class="sxs-lookup"><span data-stu-id="a497c-124">Represents a meeting cancellation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a497c-125">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a497c-125">Text value</span></span>

<span data-ttu-id="a497c-126">La valeur de texte représente une valeur de date/heure qui identifie une occurrence de calendrier.</span><span class="sxs-lookup"><span data-stu-id="a497c-126">The text value represents a date/time value that identifies a calendar occurrence.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a497c-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="a497c-127">Remarks</span></span>

<span data-ttu-id="a497c-128">Cette propriété est utilisée avec la propriété [UID](uid.md) pour identifier une instance spécifique d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="a497c-128">This property is used with the [UID](uid.md) property to identify a specific instance of a recurring calendar item.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="a497c-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a497c-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a497c-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a497c-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a497c-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a497c-131">Schema Name</span></span>  <br/> |<span data-ttu-id="a497c-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a497c-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="a497c-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a497c-133">Validation File</span></span>  <br/> |<span data-ttu-id="a497c-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a497c-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a497c-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a497c-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="a497c-136">False</span><span class="sxs-lookup"><span data-stu-id="a497c-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a497c-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a497c-137">See also</span></span>



- [<span data-ttu-id="a497c-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a497c-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

