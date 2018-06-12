---
title: IsOrganizer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a31ac268-5061-4272-a433-ffaea2fbcfa9
description: L’élément IsOrganizer spécifie une valeur de type Boolean qui indique si cette personne est l’organisateur de la réunion.
ms.openlocfilehash: 5fd775cfc0a296c08d19d0468d96aa36ba67ddd0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828063"
---
# <a name="isorganizer"></a><span data-ttu-id="8ad23-103">IsOrganizer</span><span class="sxs-lookup"><span data-stu-id="8ad23-103">IsOrganizer</span></span>

<span data-ttu-id="8ad23-104">L’élément **IsOrganizer** spécifie une valeur de type Boolean qui indique si cette personne est l’organisateur de la réunion.</span><span class="sxs-lookup"><span data-stu-id="8ad23-104">The **IsOrganizer** element specifies a Boolean value that indicates whether this person is the organizer of the meeting.</span></span> 
  
```XML
<IsOrganizer>true | false</IsOrganizer>
```

 <span data-ttu-id="8ad23-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="8ad23-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ad23-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8ad23-106">Attributes and elements</span></span>

<span data-ttu-id="8ad23-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8ad23-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ad23-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8ad23-108">Attributes</span></span>

<span data-ttu-id="8ad23-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8ad23-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ad23-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8ad23-110">Child elements</span></span>

<span data-ttu-id="8ad23-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8ad23-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ad23-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8ad23-112">Parent elements</span></span>

|<span data-ttu-id="8ad23-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8ad23-113">**Element**</span></span>|<span data-ttu-id="8ad23-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="8ad23-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ad23-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="8ad23-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8ad23-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ad23-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8ad23-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="8ad23-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="8ad23-118">Représente un message de réunion.</span><span class="sxs-lookup"><span data-stu-id="8ad23-118">Represents a meeting message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ad23-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8ad23-119">Text value</span></span>

<span data-ttu-id="8ad23-120">Une valeur de texte de **la valeur true** pour l’élément **IsOrganizer** indique que le message du calendrier élément ou la réunion a été créé par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8ad23-120">A text value of **true** for the **IsOrganizer** element indicates that the calendar item or meeting message was created by the user.</span></span> <span data-ttu-id="8ad23-121">La valeur **false** indique que le message du calendrier élément ou la réunion a été créé pas VC l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8ad23-121">A value of **false** indicates that the calendar item or meeting message was not created bv the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8ad23-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="8ad23-122">Remarks</span></span>

<span data-ttu-id="8ad23-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8ad23-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8ad23-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ad23-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ad23-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8ad23-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ad23-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8ad23-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8ad23-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8ad23-127">Schema Name</span></span>  <br/> |<span data-ttu-id="8ad23-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="8ad23-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="8ad23-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="8ad23-129">Validation File</span></span>  <br/> |<span data-ttu-id="8ad23-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="8ad23-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8ad23-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8ad23-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8ad23-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8ad23-132">See also</span></span>



- [<span data-ttu-id="8ad23-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8ad23-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

