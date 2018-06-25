---
title: MeetingWorkspaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingWorkspaceUrl
api_type:
- schema
ms.assetid: 0ca942fe-8f57-4065-93ad-65790f9a04c3
description: L’élément MeetingWorkspaceUrl contient l’URL de l’espace de travail de réunion qui est inclus dans l’élément de calendrier. Un espace de travail de réunion est un site Web partagé pour la planification de la réunion et de suivi des résultats.
ms.openlocfilehash: 7d84547eafe4e77fb23a792fbf15633dbf93d775
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828436"
---
# <a name="meetingworkspaceurl"></a><span data-ttu-id="7e468-104">MeetingWorkspaceUrl</span><span class="sxs-lookup"><span data-stu-id="7e468-104">MeetingWorkspaceUrl</span></span>

<span data-ttu-id="7e468-105">L’élément **MeetingWorkspaceUrl** contient l’URL de l’espace de travail de réunion qui est inclus dans l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="7e468-105">The **MeetingWorkspaceUrl** element contains the URL for the meeting workspace that is included in the calendar item.</span></span> <span data-ttu-id="7e468-106">Un espace de travail de réunion est un site Web partagé pour la planification de la réunion et de suivi des résultats.</span><span class="sxs-lookup"><span data-stu-id="7e468-106">A meeting workspace is a shared Web site for planning the meeting and tracking the results.</span></span> 
  
```xml
<MeetingWorkspaceUrl/>
```

 <span data-ttu-id="7e468-107">**string**</span><span class="sxs-lookup"><span data-stu-id="7e468-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e468-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7e468-108">Attributes and elements</span></span>

<span data-ttu-id="7e468-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7e468-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e468-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="7e468-110">Attributes</span></span>

<span data-ttu-id="7e468-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7e468-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e468-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7e468-112">Child elements</span></span>

<span data-ttu-id="7e468-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7e468-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e468-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7e468-114">Parent elements</span></span>

|<span data-ttu-id="7e468-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7e468-115">**Element**</span></span>|<span data-ttu-id="7e468-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="7e468-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e468-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7e468-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7e468-118">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e468-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7e468-119">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="7e468-119">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7e468-120">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e468-120">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e468-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7e468-121">Text value</span></span>

<span data-ttu-id="7e468-122">Une valeur de texte qui représente une URL est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="7e468-122">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e468-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="7e468-123">Remarks</span></span>

<span data-ttu-id="7e468-124">MeetingWorkspaceURL, de la propriété est en lecture-écriture pour l’élément de calendrier de l’organisateur de la.</span><span class="sxs-lookup"><span data-stu-id="7e468-124">The MeetingWorkspaceUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="7e468-125">Il est en lecture seule pour les demandes de réunion et des éléments de calendrier des participants.</span><span class="sxs-lookup"><span data-stu-id="7e468-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="7e468-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7e468-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e468-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7e468-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e468-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7e468-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e468-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7e468-129">Schema name</span></span>  <br/> |<span data-ttu-id="7e468-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7e468-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e468-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7e468-131">Validation file</span></span>  <br/> |<span data-ttu-id="7e468-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e468-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e468-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7e468-133">Can be empty</span></span>  <br/> |<span data-ttu-id="7e468-134">False</span><span class="sxs-lookup"><span data-stu-id="7e468-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e468-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7e468-135">See also</span></span>



- [<span data-ttu-id="7e468-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7e468-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

