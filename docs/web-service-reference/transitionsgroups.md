---
title: TransitionsGroups
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TransitionsGroups
api_type:
- schema
ms.assetid: ad0849f8-5158-4a23-9c36-a49f5be1d1e1
description: L’élément TransitionsGroups représente un tableau de groupes de transition de fuseau horaire.
ms.openlocfilehash: 546dd3c96187bf9f1ebf574b37b689e26e3af997
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838776"
---
# <a name="transitionsgroups"></a><span data-ttu-id="97fd3-103">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="97fd3-103">TransitionsGroups</span></span>

<span data-ttu-id="97fd3-104">L’élément **TransitionsGroups** représente un tableau de groupes de transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="97fd3-104">The **TransitionsGroups** element represents an array of time zone transition groups.</span></span> 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 <span data-ttu-id="97fd3-105">**ArrayOfTransitionsGroupsType**</span><span class="sxs-lookup"><span data-stu-id="97fd3-105">**ArrayOfTransitionsGroupsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97fd3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="97fd3-106">Attributes and elements</span></span>

<span data-ttu-id="97fd3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="97fd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97fd3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="97fd3-108">Attributes</span></span>

<span data-ttu-id="97fd3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="97fd3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97fd3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="97fd3-110">Child elements</span></span>

|<span data-ttu-id="97fd3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="97fd3-111">**Element**</span></span>|<span data-ttu-id="97fd3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="97fd3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97fd3-113">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="97fd3-113">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="97fd3-114">Représente un tableau des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="97fd3-114">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97fd3-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="97fd3-115">Parent elements</span></span>

|<span data-ttu-id="97fd3-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="97fd3-116">**Element**</span></span>|<span data-ttu-id="97fd3-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="97fd3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97fd3-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="97fd3-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="97fd3-119">Définit le fuseau horaire pour l’heure de début d’un [CalendarItem](calendaritem.md) [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="97fd3-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="97fd3-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="97fd3-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="97fd3-121">Définit le fuseau horaire pour l’heure de fin d’un [CalendarItem](calendaritem.md) [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="97fd3-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="97fd3-122">Définition de fuseau horaire</span><span class="sxs-lookup"><span data-stu-id="97fd3-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="97fd3-123">Définit un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="97fd3-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97fd3-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="97fd3-124">Remarks</span></span>

<span data-ttu-id="97fd3-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="97fd3-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97fd3-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="97fd3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97fd3-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="97fd3-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97fd3-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="97fd3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="97fd3-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="97fd3-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="97fd3-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="97fd3-130">Validation File</span></span>  <br/> |<span data-ttu-id="97fd3-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="97fd3-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97fd3-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="97fd3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="97fd3-133">False</span><span class="sxs-lookup"><span data-stu-id="97fd3-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97fd3-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="97fd3-134">See also</span></span>



- [<span data-ttu-id="97fd3-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="97fd3-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

