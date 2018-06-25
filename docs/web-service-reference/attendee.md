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
description: L’élément Attendee représente les participants et les ressources pour une réunion.
ms.openlocfilehash: 60cb0839c2f6de69b833c11f4594d40c14cd8887
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755341"
---
# <a name="attendee"></a><span data-ttu-id="c088e-103">Participant</span><span class="sxs-lookup"><span data-stu-id="c088e-103">Attendee</span></span>

<span data-ttu-id="c088e-104">L’élément **Attendee** représente les participants et les ressources pour une réunion.</span><span class="sxs-lookup"><span data-stu-id="c088e-104">The **Attendee** element represents attendees and resources for a meeting.</span></span> 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 <span data-ttu-id="c088e-105">**AttendeeType**</span><span class="sxs-lookup"><span data-stu-id="c088e-105">**AttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c088e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c088e-106">Attributes and elements</span></span>

<span data-ttu-id="c088e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c088e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c088e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c088e-108">Attributes</span></span>

<span data-ttu-id="c088e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c088e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c088e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c088e-110">Child elements</span></span>

|<span data-ttu-id="c088e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c088e-111">**Element**</span></span>|<span data-ttu-id="c088e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c088e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c088e-113">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="c088e-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="c088e-114">Identifie une adresse de messagerie entièrement résolu.</span><span class="sxs-lookup"><span data-stu-id="c088e-114">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="c088e-115">ResponseType</span><span class="sxs-lookup"><span data-stu-id="c088e-115">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="c088e-116">Représente le type de destinataire réponse reçue pour une réunion.</span><span class="sxs-lookup"><span data-stu-id="c088e-116">Represents the type of recipient response that is received for a meeting.</span></span> <span data-ttu-id="c088e-117">Cette propriété n’est pas pertinente pour l’élément de calendrier de l’organisateur d’une réunion.</span><span class="sxs-lookup"><span data-stu-id="c088e-117">This property is only relevant to a meeting organizer's calendar item.</span></span>  <br/> |
|[<span data-ttu-id="c088e-118">LastResponseTime</span><span class="sxs-lookup"><span data-stu-id="c088e-118">LastResponseTime</span></span>](lastresponsetime.md) <br/> |<span data-ttu-id="c088e-119">Représente la date et l’heure de la dernière réponse reçue.</span><span class="sxs-lookup"><span data-stu-id="c088e-119">Represents the date and time of the latest response that is received.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c088e-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c088e-120">Parent elements</span></span>

|<span data-ttu-id="c088e-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c088e-121">**Element**</span></span>|<span data-ttu-id="c088e-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="c088e-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c088e-123">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="c088e-123">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="c088e-124">Représente les participants qui sont nécessaires pour participer à une réunion.</span><span class="sxs-lookup"><span data-stu-id="c088e-124">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="c088e-125">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="c088e-125">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="c088e-126">Représente les participants qui ne sont pas indispensables à participer à une réunion.</span><span class="sxs-lookup"><span data-stu-id="c088e-126">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="c088e-127">Ressources</span><span class="sxs-lookup"><span data-stu-id="c088e-127">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="c088e-128">Représente une ressource pour une réunion planifiée.</span><span class="sxs-lookup"><span data-stu-id="c088e-128">Represents a scheduled resource for a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c088e-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="c088e-129">Remarks</span></span>

<span data-ttu-id="c088e-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c088e-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c088e-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c088e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c088e-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c088e-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c088e-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c088e-133">Schema name</span></span>  <br/> |<span data-ttu-id="c088e-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c088e-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="c088e-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c088e-135">Validation file</span></span>  <br/> |<span data-ttu-id="c088e-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c088e-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c088e-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c088e-137">Can be empty</span></span>  <br/> |<span data-ttu-id="c088e-138">False</span><span class="sxs-lookup"><span data-stu-id="c088e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c088e-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c088e-139">See also</span></span>

- [<span data-ttu-id="c088e-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c088e-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

