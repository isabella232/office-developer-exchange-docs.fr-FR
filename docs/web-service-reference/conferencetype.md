---
title: ConferenceType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConferenceType
api_type:
- schema
ms.assetid: 6bcf6c18-2695-44b1-aabe-dadc52b2633a
description: L’élément ConferenceType décrit le type de conférence effectuée avec un élément de calendrier.
ms.openlocfilehash: 482fc09d709e2b151b255107af59cb98de236aec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463929"
---
# <a name="conferencetype"></a><span data-ttu-id="86791-103">ConferenceType</span><span class="sxs-lookup"><span data-stu-id="86791-103">ConferenceType</span></span>

<span data-ttu-id="86791-104">L’élément **ConferenceType** décrit le type de conférence effectuée avec un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="86791-104">The **ConferenceType** element describes the type of conferencing that is performed with a calendar item.</span></span> 
  
```xml
<ConferenceType/>
```

 <span data-ttu-id="86791-105">**int**</span><span class="sxs-lookup"><span data-stu-id="86791-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86791-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="86791-106">Attributes and elements</span></span>

<span data-ttu-id="86791-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="86791-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86791-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="86791-108">Attributes</span></span>

<span data-ttu-id="86791-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="86791-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86791-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="86791-110">Child elements</span></span>

<span data-ttu-id="86791-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="86791-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="86791-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="86791-112">Parent elements</span></span>

|<span data-ttu-id="86791-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="86791-113">**Element**</span></span>|<span data-ttu-id="86791-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="86791-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86791-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="86791-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="86791-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="86791-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="86791-117">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="86791-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="86791-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="86791-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="86791-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="86791-119">Text value</span></span>

<span data-ttu-id="86791-120">Une valeur de texte qui représente une valeur entière est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="86791-120">A text value that represents an integer value is required if this element is used.</span></span> <span data-ttu-id="86791-121">Les valeurs possibles pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="86791-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="86791-122">0 = NetMeeting</span><span class="sxs-lookup"><span data-stu-id="86791-122">0 = NetMeeting</span></span>
    
- <span data-ttu-id="86791-123">1 = NetShow</span><span class="sxs-lookup"><span data-stu-id="86791-123">1 = NetShow</span></span>
    
- <span data-ttu-id="86791-124">2 = conversation</span><span class="sxs-lookup"><span data-stu-id="86791-124">2 = Chat</span></span>
    
## <a name="remarks"></a><span data-ttu-id="86791-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="86791-125">Remarks</span></span>

<span data-ttu-id="86791-126">La propriété **MeetingWorkspaceUrl,** est accessible en lecture pour l’élément de calendrier de l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="86791-126">The **MeetingWorkspaceUrl** property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="86791-127">Elle est en lecture seule pour les demandes de réunion et les éléments de calendrier du participant.</span><span class="sxs-lookup"><span data-stu-id="86791-127">It is read-only for meeting requests and for attendee's calendar items.</span></span> 
  
<span data-ttu-id="86791-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="86791-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="86791-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="86791-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86791-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="86791-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86791-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="86791-131">Schema Name</span></span>  <br/> |<span data-ttu-id="86791-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="86791-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="86791-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="86791-133">Validation File</span></span>  <br/> |<span data-ttu-id="86791-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="86791-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="86791-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="86791-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="86791-136">False</span><span class="sxs-lookup"><span data-stu-id="86791-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86791-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="86791-137">See also</span></span>



- [<span data-ttu-id="86791-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="86791-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

