---
title: AllowNewTimeProposal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowNewTimeProposal
api_type:
- schema
ms.assetid: afdb4ec9-2daf-48a1-a0bb-a7f647f212f2
description: L’élément AllowNewTimeProposal indique si une nouvelle heure de réunion peut être proposée pour une réunion à un participant.
ms.openlocfilehash: d5deed5044769c477ffe54cc533d5261ba2e1932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755195"
---
# <a name="allownewtimeproposal"></a><span data-ttu-id="f02e9-103">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="f02e9-103">AllowNewTimeProposal</span></span>

<span data-ttu-id="f02e9-104">L’élément **AllowNewTimeProposal** indique si une nouvelle heure de réunion peut être proposée pour une réunion à un participant.</span><span class="sxs-lookup"><span data-stu-id="f02e9-104">The **AllowNewTimeProposal** element indicates whether a new meeting time can be proposed for a meeting by an attendee.</span></span> 
  
```xml
<AllowNewTimeProposal/>
```

 <span data-ttu-id="f02e9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f02e9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f02e9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f02e9-106">Attributes and elements</span></span>

<span data-ttu-id="f02e9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f02e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f02e9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f02e9-108">Attributes</span></span>

<span data-ttu-id="f02e9-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="f02e9-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f02e9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f02e9-110">Child elements</span></span>

<span data-ttu-id="f02e9-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f02e9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f02e9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f02e9-112">Parent elements</span></span>

|<span data-ttu-id="f02e9-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f02e9-113">**Element**</span></span>|<span data-ttu-id="f02e9-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f02e9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f02e9-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f02e9-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f02e9-116">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f02e9-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f02e9-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f02e9-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f02e9-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="f02e9-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f02e9-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f02e9-119">Text value</span></span>

<span data-ttu-id="f02e9-120">Une valeur de texte qui représente une valeur Boolean est requise.</span><span class="sxs-lookup"><span data-stu-id="f02e9-120">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="f02e9-121">La valeur **true** indique qu’une nouvelle proposition de l’heure de la réunion peut être créée ; la valeur **false** indique que les nouvelles propositions d’horaires ne sont pas autorisées.</span><span class="sxs-lookup"><span data-stu-id="f02e9-121">A value of **true** indicates that a new proposal for the meeting time can be created; a value of **false** indicates that new time proposals are not allowed.</span></span> <span data-ttu-id="f02e9-122">L’organisateur définit cette valeur dans la demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="f02e9-122">The organizer sets this value in the meeting request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f02e9-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="f02e9-123">Remarks</span></span>

<span data-ttu-id="f02e9-124">La propriété AllowNewTimeProposal est en lecture-écriture pour l’élément de calendrier de l’organisateur de la.</span><span class="sxs-lookup"><span data-stu-id="f02e9-124">The AllowNewTimeProposal property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="f02e9-125">Il est en lecture seule pour les demandes de réunion et des éléments de calendrier des participants.</span><span class="sxs-lookup"><span data-stu-id="f02e9-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="f02e9-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f02e9-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f02e9-127">Services Web Exchange ne gère pas les nouveaux messages de proposition de temps.</span><span class="sxs-lookup"><span data-stu-id="f02e9-127">Exchange Web Services does not support new time proposal messages.</span></span> <span data-ttu-id="f02e9-128">Pour obtenir les propriétés liées aux nouveaux messages de proposition de temps, utilisez les propriétés étendues.</span><span class="sxs-lookup"><span data-stu-id="f02e9-128">To get properties that are related to new time proposal messages, use extended properties.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f02e9-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f02e9-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f02e9-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f02e9-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f02e9-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f02e9-131">Schema name</span></span>  <br/> |<span data-ttu-id="f02e9-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f02e9-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="f02e9-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f02e9-133">Validation file</span></span>  <br/> |<span data-ttu-id="f02e9-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f02e9-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f02e9-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f02e9-135">Can be empty</span></span>  <br/> |<span data-ttu-id="f02e9-136">False</span><span class="sxs-lookup"><span data-stu-id="f02e9-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f02e9-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f02e9-137">See also</span></span>

- [<span data-ttu-id="f02e9-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f02e9-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

