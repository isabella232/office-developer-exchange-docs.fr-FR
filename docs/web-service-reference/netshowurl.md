---
title: NetShowUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NetShowUrl
api_type:
- schema
ms.assetid: a5d48fc1-b141-422c-bcb0-05d0f9ba90dd
description: L’élément NetShowUrl Spécifie l’URL d’une réunion en ligne Microsoft NetShow.
ms.openlocfilehash: 2440e6c1501331d715d0e5ceb31b3b928122f927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828519"
---
# <a name="netshowurl"></a><span data-ttu-id="1185a-103">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="1185a-103">NetShowUrl</span></span>

<span data-ttu-id="1185a-104">L’élément **NetShowUrl** Spécifie l’URL d’une réunion en ligne Microsoft NetShow.</span><span class="sxs-lookup"><span data-stu-id="1185a-104">The **NetShowUrl** element specifies the URL for a Microsoft NetShow online meeting.</span></span> 
  
```xml
<NetShowUrl/>
```

 <span data-ttu-id="1185a-105">**string**</span><span class="sxs-lookup"><span data-stu-id="1185a-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1185a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1185a-106">Attributes and elements</span></span>

<span data-ttu-id="1185a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1185a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1185a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1185a-108">Attributes</span></span>

<span data-ttu-id="1185a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1185a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1185a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1185a-110">Child elements</span></span>

<span data-ttu-id="1185a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1185a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1185a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1185a-112">Parent elements</span></span>

|<span data-ttu-id="1185a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1185a-113">**Element**</span></span>|<span data-ttu-id="1185a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1185a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1185a-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="1185a-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="1185a-116">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1185a-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1185a-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="1185a-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="1185a-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="1185a-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1185a-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1185a-119">Text value</span></span>

<span data-ttu-id="1185a-120">Une valeur de texte qui représente une URL est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="1185a-120">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1185a-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="1185a-121">Remarks</span></span>

<span data-ttu-id="1185a-122">NetShowURL, de cette propriété est en lecture-écriture pour l’élément de calendrier de l’organisateur de la.</span><span class="sxs-lookup"><span data-stu-id="1185a-122">This NetShowUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="1185a-123">Il est en lecture seule pour les demandes de réunion et des participants.</span><span class="sxs-lookup"><span data-stu-id="1185a-123">It is read-only for meeting requests and for attendees.</span></span>
  
<span data-ttu-id="1185a-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1185a-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1185a-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1185a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1185a-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1185a-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1185a-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1185a-127">Schema name</span></span>  <br/> |<span data-ttu-id="1185a-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1185a-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="1185a-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1185a-129">Validation file</span></span>  <br/> |<span data-ttu-id="1185a-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1185a-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1185a-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1185a-131">Can be empty</span></span>  <br/> |<span data-ttu-id="1185a-132">False</span><span class="sxs-lookup"><span data-stu-id="1185a-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1185a-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1185a-133">See also</span></span>



- [<span data-ttu-id="1185a-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1185a-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

