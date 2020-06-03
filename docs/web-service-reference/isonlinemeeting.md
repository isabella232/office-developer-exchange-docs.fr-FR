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
description: L’élément IsOnlineMeeting indique si la réunion est en ligne.
ms.openlocfilehash: d2d60c8a51ad7e03c33b57709d9173e79d162268
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460399"
---
# <a name="isonlinemeeting"></a><span data-ttu-id="6a0aa-103">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6a0aa-103">IsOnlineMeeting</span></span>

<span data-ttu-id="6a0aa-104">L’élément **IsOnlineMeeting** indique si la réunion est en ligne.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-104">The **IsOnlineMeeting** element indicates whether the meeting is online.</span></span> 
  
```xml
<IsOnlineMeeting/>
```

 <span data-ttu-id="6a0aa-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6a0aa-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a0aa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6a0aa-106">Attributes and elements</span></span>

<span data-ttu-id="6a0aa-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a0aa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6a0aa-108">Attributes</span></span>

<span data-ttu-id="6a0aa-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a0aa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6a0aa-110">Child elements</span></span>

<span data-ttu-id="6a0aa-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a0aa-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6a0aa-112">Parent elements</span></span>

|<span data-ttu-id="6a0aa-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6a0aa-113">**Element**</span></span>|<span data-ttu-id="6a0aa-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="6a0aa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a0aa-115">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="6a0aa-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="6a0aa-116">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6a0aa-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="6a0aa-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="6a0aa-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6a0aa-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="6a0aa-119">Text value</span></span>

<span data-ttu-id="6a0aa-120">Une valeur de texte qui représente une valeur booléenne est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-120">A text value that represents a Boolean value is required if this element is used.</span></span> <span data-ttu-id="6a0aa-121">La valeur **true** indique que la réunion est en ligne.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-121">A value of **true** indicates that the meeting is online.</span></span> <span data-ttu-id="6a0aa-122">La valeur **false** indique que la réunion n’est pas en ligne.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-122">A value of **false** indicates that the meeting is not online.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6a0aa-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="6a0aa-123">Remarks</span></span>

<span data-ttu-id="6a0aa-124">La propriété IsOnlineMeeting est accessible en lecture pour l’élément de calendrier de l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-124">The IsOnlineMeeting property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="6a0aa-125">Elle est en lecture seule pour les demandes de réunion et les éléments de calendrier des participants.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="6a0aa-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange 2007 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6a0aa-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a0aa-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6a0aa-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a0aa-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6a0aa-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a0aa-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6a0aa-129">Schema name</span></span>  <br/> |<span data-ttu-id="6a0aa-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6a0aa-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a0aa-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6a0aa-131">Validation file</span></span>  <br/> |<span data-ttu-id="6a0aa-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6a0aa-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a0aa-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6a0aa-133">Can be empty</span></span>  <br/> |<span data-ttu-id="6a0aa-134">False</span><span class="sxs-lookup"><span data-stu-id="6a0aa-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a0aa-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6a0aa-135">See also</span></span>



- [<span data-ttu-id="6a0aa-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6a0aa-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

