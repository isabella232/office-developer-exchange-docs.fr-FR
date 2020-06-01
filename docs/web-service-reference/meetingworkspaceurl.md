---
title: MeetingWorkspaceUrl,
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
description: L’élément MeetingWorkspaceUrl, contient l’URL de l’espace de travail de réunion qui est inclus dans l’élément de calendrier. Un espace de travail de réunion est un site Web partagé qui permet de planifier la réunion et de suivre les résultats.
ms.openlocfilehash: cd4396e590ab1471278bd44b9a4e0009fe326eaf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466282"
---
# <a name="meetingworkspaceurl"></a><span data-ttu-id="a88b2-104">MeetingWorkspaceUrl,</span><span class="sxs-lookup"><span data-stu-id="a88b2-104">MeetingWorkspaceUrl</span></span>

<span data-ttu-id="a88b2-105">L’élément **MeetingWorkspaceUrl,** contient l’URL de l’espace de travail de réunion qui est inclus dans l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="a88b2-105">The **MeetingWorkspaceUrl** element contains the URL for the meeting workspace that is included in the calendar item.</span></span> <span data-ttu-id="a88b2-106">Un espace de travail de réunion est un site Web partagé qui permet de planifier la réunion et de suivre les résultats.</span><span class="sxs-lookup"><span data-stu-id="a88b2-106">A meeting workspace is a shared Web site for planning the meeting and tracking the results.</span></span> 
  
```xml
<MeetingWorkspaceUrl/>
```

 <span data-ttu-id="a88b2-107">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="a88b2-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a88b2-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a88b2-108">Attributes and elements</span></span>

<span data-ttu-id="a88b2-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a88b2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a88b2-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="a88b2-110">Attributes</span></span>

<span data-ttu-id="a88b2-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a88b2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a88b2-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a88b2-112">Child elements</span></span>

<span data-ttu-id="a88b2-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a88b2-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a88b2-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a88b2-114">Parent elements</span></span>

|<span data-ttu-id="a88b2-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a88b2-115">**Element**</span></span>|<span data-ttu-id="a88b2-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="a88b2-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a88b2-117">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="a88b2-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a88b2-118">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a88b2-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a88b2-119">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a88b2-119">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a88b2-120">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="a88b2-120">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a88b2-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a88b2-121">Text value</span></span>

<span data-ttu-id="a88b2-122">Une valeur de texte qui représente une URL est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="a88b2-122">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a88b2-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="a88b2-123">Remarks</span></span>

<span data-ttu-id="a88b2-124">La propriété MeetingWorkspaceUrl, est accessible en lecture pour l’élément de calendrier de l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="a88b2-124">The MeetingWorkspaceUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="a88b2-125">Elle est en lecture seule pour les demandes de réunion et les éléments de calendrier des participants.</span><span class="sxs-lookup"><span data-stu-id="a88b2-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="a88b2-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a88b2-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a88b2-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a88b2-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a88b2-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a88b2-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a88b2-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a88b2-129">Schema name</span></span>  <br/> |<span data-ttu-id="a88b2-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a88b2-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="a88b2-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a88b2-131">Validation file</span></span>  <br/> |<span data-ttu-id="a88b2-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a88b2-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a88b2-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a88b2-133">Can be empty</span></span>  <br/> |<span data-ttu-id="a88b2-134">False</span><span class="sxs-lookup"><span data-stu-id="a88b2-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a88b2-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a88b2-135">See also</span></span>



- [<span data-ttu-id="a88b2-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a88b2-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

