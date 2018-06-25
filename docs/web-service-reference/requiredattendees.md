---
title: RequiredAttendees
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequiredAttendees
api_type:
- schema
ms.assetid: 422f8d44-b0eb-49ca-af0f-0e22b54c78d2
description: L’élément RequiredAttendees représente les participants qui sont nécessaires pour participer à une réunion.
ms.openlocfilehash: 9630be828f459808b61602448a4675aac07b0106
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829149"
---
# <a name="requiredattendees"></a><span data-ttu-id="b3b3e-103">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="b3b3e-103">RequiredAttendees</span></span>

<span data-ttu-id="b3b3e-104">L’élément **RequiredAttendees** représente les participants qui sont nécessaires pour participer à une réunion.</span><span class="sxs-lookup"><span data-stu-id="b3b3e-104">The **RequiredAttendees** element represents attendees that are required to attend a meeting.</span></span> 
  
```xml
<RequiredAttendees>
   <Attendee/>
</RequiredAttendees>
```

 <span data-ttu-id="b3b3e-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="b3b3e-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b3b3e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b3b3e-106">Attributes and elements</span></span>

<span data-ttu-id="b3b3e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b3b3e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b3b3e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b3b3e-108">Attributes</span></span>

<span data-ttu-id="b3b3e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b3b3e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b3b3e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b3b3e-110">Child elements</span></span>

|<span data-ttu-id="b3b3e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b3b3e-111">**Element**</span></span>|<span data-ttu-id="b3b3e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b3b3e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3b3e-113">Attendee</span><span class="sxs-lookup"><span data-stu-id="b3b3e-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="b3b3e-114">Représente les participants et les ressources pour une réunion.</span><span class="sxs-lookup"><span data-stu-id="b3b3e-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b3b3e-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b3b3e-115">Parent elements</span></span>

|<span data-ttu-id="b3b3e-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b3b3e-116">**Element**</span></span>|<span data-ttu-id="b3b3e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b3b3e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b3b3e-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="b3b3e-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b3b3e-119">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3b3e-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b3b3e-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b3b3e-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b3b3e-121">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3b3e-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b3b3e-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="b3b3e-122">Remarks</span></span>

<span data-ttu-id="b3b3e-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b3b3e-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b3b3e-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b3b3e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b3b3e-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b3b3e-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b3b3e-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b3b3e-126">Schema name</span></span>  <br/> |<span data-ttu-id="b3b3e-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b3b3e-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="b3b3e-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b3b3e-128">Validation file</span></span>  <br/> |<span data-ttu-id="b3b3e-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b3b3e-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b3b3e-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b3b3e-130">Can be empty</span></span>  <br/> |<span data-ttu-id="b3b3e-131">False</span><span class="sxs-lookup"><span data-stu-id="b3b3e-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b3b3e-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b3b3e-132">See also</span></span>



- [<span data-ttu-id="b3b3e-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b3b3e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

