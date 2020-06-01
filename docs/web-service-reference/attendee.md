---
title: Participant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attendee
api_type:
- schema
ms.assetid: 393c3d7e-7416-458a-b976-270b88eaaa03
description: L’élément participant représente les participants et les ressources d’une réunion.
ms.openlocfilehash: f376e59b27017e0a9d27692cb1a4ae759cd1af0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457647"
---
# <a name="attendee"></a><span data-ttu-id="655b4-103">Participant</span><span class="sxs-lookup"><span data-stu-id="655b4-103">Attendee</span></span>

<span data-ttu-id="655b4-104">L’élément **participant** représente les participants et les ressources d’une réunion.</span><span class="sxs-lookup"><span data-stu-id="655b4-104">The **Attendee** element represents attendees and resources for a meeting.</span></span> 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 <span data-ttu-id="655b4-105">**AttendeeType**</span><span class="sxs-lookup"><span data-stu-id="655b4-105">**AttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="655b4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="655b4-106">Attributes and elements</span></span>

<span data-ttu-id="655b4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="655b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="655b4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="655b4-108">Attributes</span></span>

<span data-ttu-id="655b4-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="655b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="655b4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="655b4-110">Child elements</span></span>

|<span data-ttu-id="655b4-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="655b4-111">**Element**</span></span>|<span data-ttu-id="655b4-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="655b4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="655b4-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="655b4-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="655b4-114">Identifie une adresse de messagerie entièrement résolue.</span><span class="sxs-lookup"><span data-stu-id="655b4-114">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="655b4-115">ResponseType</span><span class="sxs-lookup"><span data-stu-id="655b4-115">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="655b4-116">Représente le type de réponse de destinataire reçue pour une réunion.</span><span class="sxs-lookup"><span data-stu-id="655b4-116">Represents the type of recipient response that is received for a meeting.</span></span> <span data-ttu-id="655b4-117">Cette propriété s’applique uniquement à l’élément de calendrier d’un organisateur de réunion.</span><span class="sxs-lookup"><span data-stu-id="655b4-117">This property is only relevant to a meeting organizer's calendar item.</span></span>  <br/> |
|[<span data-ttu-id="655b4-118">LastResponseTime</span><span class="sxs-lookup"><span data-stu-id="655b4-118">LastResponseTime</span></span>](lastresponsetime.md) <br/> |<span data-ttu-id="655b4-119">Représente la date et l’heure de la dernière réponse reçue.</span><span class="sxs-lookup"><span data-stu-id="655b4-119">Represents the date and time of the latest response that is received.</span></span>  <br/> |
|[<span data-ttu-id="655b4-120">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="655b4-120">ProposedStart</span></span>](proposedstart-attendeetype.md) <br/> |<span data-ttu-id="655b4-121">Représente l’heure de début proposée par un participant à une réunion.</span><span class="sxs-lookup"><span data-stu-id="655b4-121">Represents an attendee's proposed start time for a meeting.</span></span> <br/> |
|[<span data-ttu-id="655b4-122">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="655b4-122">ProposedEnd</span></span>](proposedend-attendeetype.md) <br/> |<span data-ttu-id="655b4-123">Représente l’heure de fin proposée par un participant à une réunion.</span><span class="sxs-lookup"><span data-stu-id="655b4-123">Represents an attendee's proposed end time for a meeting.</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="655b4-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="655b4-124">Parent elements</span></span>

|<span data-ttu-id="655b4-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="655b4-125">**Element**</span></span>|<span data-ttu-id="655b4-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="655b4-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="655b4-127">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="655b4-127">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="655b4-128">Représente les participants qui sont requis pour participer à une réunion.</span><span class="sxs-lookup"><span data-stu-id="655b4-128">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="655b4-129">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="655b4-129">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="655b4-130">Représente les participants qui ne sont pas tenus de participer à une réunion.</span><span class="sxs-lookup"><span data-stu-id="655b4-130">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="655b4-131">Resources</span><span class="sxs-lookup"><span data-stu-id="655b4-131">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="655b4-132">Représente une ressource planifiée pour une réunion.</span><span class="sxs-lookup"><span data-stu-id="655b4-132">Represents a scheduled resource for a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="655b4-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="655b4-133">Remarks</span></span>

<span data-ttu-id="655b4-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="655b4-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="655b4-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="655b4-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="655b4-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="655b4-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="655b4-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="655b4-137">Schema name</span></span>  <br/> |<span data-ttu-id="655b4-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="655b4-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="655b4-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="655b4-139">Validation file</span></span>  <br/> |<span data-ttu-id="655b4-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="655b4-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="655b4-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="655b4-141">Can be empty</span></span>  <br/> |<span data-ttu-id="655b4-142">False</span><span class="sxs-lookup"><span data-stu-id="655b4-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="655b4-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="655b4-143">See also</span></span>

- [<span data-ttu-id="655b4-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="655b4-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

