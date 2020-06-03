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
description: L’élément RequiredAttendees représente les participants qui sont requis pour participer à une réunion.
ms.openlocfilehash: a67800687f24dc323c3d80e4166ca9dd34dfc4fc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468291"
---
# <a name="requiredattendees"></a><span data-ttu-id="1a9e2-103">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="1a9e2-103">RequiredAttendees</span></span>

<span data-ttu-id="1a9e2-104">L’élément **RequiredAttendees** représente les participants qui sont requis pour participer à une réunion.</span><span class="sxs-lookup"><span data-stu-id="1a9e2-104">The **RequiredAttendees** element represents attendees that are required to attend a meeting.</span></span> 
  
```xml
<RequiredAttendees>
   <Attendee/>
</RequiredAttendees>
```

 <span data-ttu-id="1a9e2-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="1a9e2-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a9e2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1a9e2-106">Attributes and elements</span></span>

<span data-ttu-id="1a9e2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1a9e2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a9e2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1a9e2-108">Attributes</span></span>

<span data-ttu-id="1a9e2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1a9e2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a9e2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1a9e2-110">Child elements</span></span>

|<span data-ttu-id="1a9e2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1a9e2-111">**Element**</span></span>|<span data-ttu-id="1a9e2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a9e2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a9e2-113">Participant</span><span class="sxs-lookup"><span data-stu-id="1a9e2-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="1a9e2-114">Représente les participants et les ressources d’une réunion.</span><span class="sxs-lookup"><span data-stu-id="1a9e2-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a9e2-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1a9e2-115">Parent elements</span></span>

|<span data-ttu-id="1a9e2-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1a9e2-116">**Element**</span></span>|<span data-ttu-id="1a9e2-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a9e2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a9e2-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="1a9e2-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="1a9e2-119">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a9e2-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="1a9e2-120">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="1a9e2-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="1a9e2-121">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a9e2-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1a9e2-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="1a9e2-122">Remarks</span></span>

<span data-ttu-id="1a9e2-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1a9e2-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a9e2-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1a9e2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a9e2-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1a9e2-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a9e2-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1a9e2-126">Schema name</span></span>  <br/> |<span data-ttu-id="1a9e2-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1a9e2-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="1a9e2-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1a9e2-128">Validation file</span></span>  <br/> |<span data-ttu-id="1a9e2-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1a9e2-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a9e2-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1a9e2-130">Can be empty</span></span>  <br/> |<span data-ttu-id="1a9e2-131">False</span><span class="sxs-lookup"><span data-stu-id="1a9e2-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a9e2-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1a9e2-132">See also</span></span>



- [<span data-ttu-id="1a9e2-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1a9e2-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

