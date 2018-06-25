---
title: LegacyFreeBusyStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LegacyFreeBusyStatus
api_type:
- schema
ms.assetid: ee5f3046-b79f-4f68-9455-1a688cee2745
description: L’élément LegacyFreeBusyStatus représente l’état de disponibilité de l’élément de calendrier.
ms.openlocfilehash: 681d7256dbef09c6c43d33ea1fc92b5d05e73a41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828247"
---
# <a name="legacyfreebusystatus"></a><span data-ttu-id="30aa5-103">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="30aa5-103">LegacyFreeBusyStatus</span></span>

<span data-ttu-id="30aa5-104">L’élément **LegacyFreeBusyStatus** représente l’état de disponibilité de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="30aa5-104">The **LegacyFreeBusyStatus** element represents the free/busy status of the calendar item.</span></span> 
  
```xml
<LegacyFreeBusyStatus/>
```

<span data-ttu-id="30aa5-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="30aa5-105">**LegacyFreeBusyType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="30aa5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="30aa5-106">Attributes and elements</span></span>

<span data-ttu-id="30aa5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="30aa5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30aa5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="30aa5-108">Attributes</span></span>

<span data-ttu-id="30aa5-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="30aa5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30aa5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="30aa5-110">Child elements</span></span>

<span data-ttu-id="30aa5-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="30aa5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="30aa5-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="30aa5-112">Parent elements</span></span>

|<span data-ttu-id="30aa5-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="30aa5-113">**Element**</span></span>|<span data-ttu-id="30aa5-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="30aa5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30aa5-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="30aa5-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="30aa5-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="30aa5-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="30aa5-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="30aa5-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="30aa5-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="30aa5-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="30aa5-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="30aa5-119">Text value</span></span>

<span data-ttu-id="30aa5-120">Une valeur de texte est nécessaire pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="30aa5-120">A text value is required for this element.</span></span> <span data-ttu-id="30aa5-121">Les valeurs de texte possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="30aa5-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="30aa5-122">Gratuit</span><span class="sxs-lookup"><span data-stu-id="30aa5-122">Free</span></span> 
- <span data-ttu-id="30aa5-123">Provisoire</span><span class="sxs-lookup"><span data-stu-id="30aa5-123">Tentative</span></span>
- <span data-ttu-id="30aa5-124">Occupé(e)</span><span class="sxs-lookup"><span data-stu-id="30aa5-124">Busy</span></span>
- <span data-ttu-id="30aa5-125">ABSENCE DU BUREAU</span><span class="sxs-lookup"><span data-stu-id="30aa5-125">OOF</span></span>
- <span data-ttu-id="30aa5-126">WorkingElsewhere</span><span class="sxs-lookup"><span data-stu-id="30aa5-126">WorkingElsewhere</span></span>
- <span data-ttu-id="30aa5-127">NoData</span><span class="sxs-lookup"><span data-stu-id="30aa5-127">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="30aa5-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="30aa5-128">Remarks</span></span>

<span data-ttu-id="30aa5-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="30aa5-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30aa5-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="30aa5-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30aa5-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="30aa5-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="30aa5-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="30aa5-132">Schema name</span></span>  <br/> |<span data-ttu-id="30aa5-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="30aa5-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="30aa5-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="30aa5-134">Validation file</span></span>  <br/> |<span data-ttu-id="30aa5-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="30aa5-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="30aa5-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="30aa5-136">Can be empty</span></span>  <br/> |<span data-ttu-id="30aa5-137">False</span><span class="sxs-lookup"><span data-stu-id="30aa5-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30aa5-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="30aa5-138">See also</span></span>

- [<span data-ttu-id="30aa5-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="30aa5-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

