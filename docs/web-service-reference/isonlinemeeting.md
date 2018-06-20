---
title: IsOnlineMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOnlineMeeting
api_type:
- schema
ms.assetid: c29df676-0f3a-4694-a42f-522c6d16872f
description: L’élément IsOnlineMeeting indique si la réunion en ligne.
ms.openlocfilehash: 5a56b0b9828d6f6bec83fc0ad0f8f9579b471a72
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828061"
---
# <a name="isonlinemeeting"></a><span data-ttu-id="4fc8e-103">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4fc8e-103">IsOnlineMeeting</span></span>

<span data-ttu-id="4fc8e-104">L’élément **IsOnlineMeeting** indique si la réunion en ligne.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-104">The **IsOnlineMeeting** element indicates whether the meeting is online.</span></span> 
  
```xml
<IsOnlineMeeting/>
```

 <span data-ttu-id="4fc8e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4fc8e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fc8e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4fc8e-106">Attributes and elements</span></span>

<span data-ttu-id="4fc8e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fc8e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4fc8e-108">Attributes</span></span>

<span data-ttu-id="4fc8e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fc8e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4fc8e-110">Child elements</span></span>

<span data-ttu-id="4fc8e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4fc8e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4fc8e-112">Parent elements</span></span>

|<span data-ttu-id="4fc8e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4fc8e-113">**Element**</span></span>|<span data-ttu-id="4fc8e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="4fc8e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fc8e-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="4fc8e-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="4fc8e-116">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4fc8e-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="4fc8e-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="4fc8e-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4fc8e-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4fc8e-119">Text value</span></span>

<span data-ttu-id="4fc8e-120">Une valeur de texte qui représente une valeur Boolean est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-120">A text value that represents a Boolean value is required if this element is used.</span></span> <span data-ttu-id="4fc8e-121">La valeur **true** indique que la réunion est en ligne.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-121">A value of **true** indicates that the meeting is online.</span></span> <span data-ttu-id="4fc8e-122">La valeur **false** indique que la réunion n’est pas en ligne.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-122">A value of **false** indicates that the meeting is not online.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4fc8e-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="4fc8e-123">Remarks</span></span>

<span data-ttu-id="4fc8e-124">IsOnlineMeeting, de la propriété est en lecture-écriture pour l’élément de calendrier de l’organisateur de la.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-124">The IsOnlineMeeting property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="4fc8e-125">Il est en lecture seule pour les demandes de réunion et des éléments de calendrier des participants.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="4fc8e-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="4fc8e-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fc8e-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4fc8e-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fc8e-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4fc8e-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4fc8e-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4fc8e-129">Schema name</span></span>  <br/> |<span data-ttu-id="4fc8e-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4fc8e-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="4fc8e-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4fc8e-131">Validation file</span></span>  <br/> |<span data-ttu-id="4fc8e-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4fc8e-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4fc8e-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4fc8e-133">Can be empty</span></span>  <br/> |<span data-ttu-id="4fc8e-134">False</span><span class="sxs-lookup"><span data-stu-id="4fc8e-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fc8e-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4fc8e-135">See also</span></span>



- [<span data-ttu-id="4fc8e-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4fc8e-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

