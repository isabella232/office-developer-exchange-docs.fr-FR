---
title: MeetingRequestWasSent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestWasSent
api_type:
- schema
ms.assetid: 9192400a-8eef-4147-9f94-aa8ea91b41d8
description: L’élément MeetingRequestWasSent indique si une demande de réunion a été envoyée aux participants demandés.
ms.openlocfilehash: 0a87b1d773997e08ab96726375e4c8ce010faaf7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828438"
---
# <a name="meetingrequestwassent"></a><span data-ttu-id="de259-103">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="de259-103">MeetingRequestWasSent</span></span>

<span data-ttu-id="de259-104">L’élément **MeetingRequestWasSent** indique si une demande de réunion a été envoyée aux participants demandés.</span><span class="sxs-lookup"><span data-stu-id="de259-104">The **MeetingRequestWasSent** element indicates whether a meeting request has been sent to requested attendees.</span></span> 
  
```xml
<MeetingRequestWasSent/>
```

 <span data-ttu-id="de259-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="de259-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de259-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="de259-106">Attributes and elements</span></span>

<span data-ttu-id="de259-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="de259-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de259-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="de259-108">Attributes</span></span>

<span data-ttu-id="de259-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="de259-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de259-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="de259-110">Child elements</span></span>

<span data-ttu-id="de259-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="de259-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="de259-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="de259-112">Parent elements</span></span>

|<span data-ttu-id="de259-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="de259-113">**Element**</span></span>|<span data-ttu-id="de259-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="de259-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de259-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="de259-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="de259-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="de259-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="de259-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="de259-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="de259-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="de259-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="de259-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="de259-119">Text value</span></span>

<span data-ttu-id="de259-120">Une valeur de texte qui représente une valeur Boolean est requise si cet élément est inclus.</span><span class="sxs-lookup"><span data-stu-id="de259-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="de259-121">La valeur **true** indique qu’une demande de réunion a été envoyée.</span><span class="sxs-lookup"><span data-stu-id="de259-121">A value of **true** indicates that a meeting request was sent.</span></span> <span data-ttu-id="de259-122">La valeur **false** indique qu’une demande de réunion n’a pas été envoyée.</span><span class="sxs-lookup"><span data-stu-id="de259-122">A value of **false** indicates that a meeting request has not been sent.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="de259-123">Note</span><span class="sxs-lookup"><span data-stu-id="de259-123">Remarks</span></span>

<span data-ttu-id="de259-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="de259-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de259-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="de259-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de259-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="de259-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="de259-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="de259-127">Schema name</span></span>  <br/> |<span data-ttu-id="de259-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="de259-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="de259-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="de259-129">Validation file</span></span>  <br/> |<span data-ttu-id="de259-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="de259-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="de259-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="de259-131">Can be empty</span></span>  <br/> |<span data-ttu-id="de259-132">False</span><span class="sxs-lookup"><span data-stu-id="de259-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de259-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="de259-133">See also</span></span>



- [<span data-ttu-id="de259-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="de259-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

