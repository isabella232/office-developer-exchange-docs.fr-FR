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
ms.openlocfilehash: ecbcae0862c9c02c0a4a61012816e4c2c6ea07b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463229"
---
# <a name="legacyfreebusystatus"></a><span data-ttu-id="9479b-103">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="9479b-103">LegacyFreeBusyStatus</span></span>

<span data-ttu-id="9479b-104">L’élément **LegacyFreeBusyStatus** représente l’état de disponibilité de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="9479b-104">The **LegacyFreeBusyStatus** element represents the free/busy status of the calendar item.</span></span> 
  
```xml
<LegacyFreeBusyStatus/>
```

<span data-ttu-id="9479b-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="9479b-105">**LegacyFreeBusyType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9479b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9479b-106">Attributes and elements</span></span>

<span data-ttu-id="9479b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9479b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9479b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9479b-108">Attributes</span></span>

<span data-ttu-id="9479b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9479b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9479b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9479b-110">Child elements</span></span>

<span data-ttu-id="9479b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9479b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9479b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9479b-112">Parent elements</span></span>

|<span data-ttu-id="9479b-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9479b-113">**Element**</span></span>|<span data-ttu-id="9479b-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9479b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9479b-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="9479b-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="9479b-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="9479b-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="9479b-117">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="9479b-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9479b-118">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="9479b-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9479b-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="9479b-119">Text value</span></span>

<span data-ttu-id="9479b-120">Une valeur de texte est requise pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="9479b-120">A text value is required for this element.</span></span> <span data-ttu-id="9479b-121">Voici les valeurs de texte possibles pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="9479b-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="9479b-122">Gratuit</span><span class="sxs-lookup"><span data-stu-id="9479b-122">Free</span></span> 
- <span data-ttu-id="9479b-123">Provisoire</span><span class="sxs-lookup"><span data-stu-id="9479b-123">Tentative</span></span>
- <span data-ttu-id="9479b-124">Occupé(e)</span><span class="sxs-lookup"><span data-stu-id="9479b-124">Busy</span></span>
- <span data-ttu-id="9479b-125">Bureau</span><span class="sxs-lookup"><span data-stu-id="9479b-125">OOF</span></span>
- <span data-ttu-id="9479b-126">WorkingElsewhere</span><span class="sxs-lookup"><span data-stu-id="9479b-126">WorkingElsewhere</span></span>
- <span data-ttu-id="9479b-127">NoData</span><span class="sxs-lookup"><span data-stu-id="9479b-127">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="9479b-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="9479b-128">Remarks</span></span>

<span data-ttu-id="9479b-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9479b-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9479b-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9479b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9479b-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9479b-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9479b-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9479b-132">Schema name</span></span>  <br/> |<span data-ttu-id="9479b-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9479b-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="9479b-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9479b-134">Validation file</span></span>  <br/> |<span data-ttu-id="9479b-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9479b-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9479b-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9479b-136">Can be empty</span></span>  <br/> |<span data-ttu-id="9479b-137">False</span><span class="sxs-lookup"><span data-stu-id="9479b-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9479b-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9479b-138">See also</span></span>

- [<span data-ttu-id="9479b-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9479b-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

