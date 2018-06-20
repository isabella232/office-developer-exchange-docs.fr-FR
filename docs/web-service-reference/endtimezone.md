---
title: EndTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTimeZone
api_type:
- schema
ms.assetid: 6c53c337-be60-4d22-9e9e-a0c140c5e913
description: L’élément EndTimeZone définit le fuseau horaire pour l’heure de fin d’un CalendarItem MeetingRequest.
ms.openlocfilehash: 65eeedcc7c4d0e616ae54d4e2545fd310e9ad905
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756183"
---
# <a name="endtimezone"></a><span data-ttu-id="3f413-103">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="3f413-103">EndTimeZone</span></span>

<span data-ttu-id="3f413-104">L’élément **EndTimeZone** définit le fuseau horaire pour l’heure de fin d’un [CalendarItem](calendaritem.md) [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="3f413-104">The **EndTimeZone** element defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<EndTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</EndTimeZone>
```

 <span data-ttu-id="3f413-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="3f413-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f413-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3f413-106">Attributes and elements</span></span>

<span data-ttu-id="3f413-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3f413-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f413-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3f413-108">Attributes</span></span>

|<span data-ttu-id="3f413-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="3f413-109">**Attribute**</span></span>|<span data-ttu-id="3f413-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="3f413-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3f413-111">ID</span><span class="sxs-lookup"><span data-stu-id="3f413-111">Id</span></span>  <br/> |<span data-ttu-id="3f413-112">Identificateur unique de la définition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="3f413-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="3f413-113">Nom</span><span class="sxs-lookup"><span data-stu-id="3f413-113">Name</span></span>  <br/> |<span data-ttu-id="3f413-114">Représente le nom descriptif de la définition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="3f413-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3f413-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3f413-115">Child elements</span></span>

|<span data-ttu-id="3f413-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3f413-116">**Element**</span></span>|<span data-ttu-id="3f413-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="3f413-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f413-118">Périodes</span><span class="sxs-lookup"><span data-stu-id="3f413-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="3f413-119">Représente un tableau d’éléments de [période](period.md) qui définissent le décalage de temps à différents stades du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="3f413-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="3f413-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="3f413-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="3f413-121">Représente un tableau d’éléments [TransitionsGroup](transitionsgroup.md) qui spécifient les transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="3f413-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="3f413-122">Transitions</span><span class="sxs-lookup"><span data-stu-id="3f413-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="3f413-123">Représente un tableau des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="3f413-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3f413-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3f413-124">Parent elements</span></span>

|<span data-ttu-id="3f413-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3f413-125">**Element**</span></span>|<span data-ttu-id="3f413-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="3f413-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f413-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="3f413-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3f413-128">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f413-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3f413-129">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3f413-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3f413-130">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f413-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3f413-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="3f413-131">Remarks</span></span>

<span data-ttu-id="3f413-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="3f413-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f413-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3f413-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f413-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3f413-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3f413-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3f413-135">Schema Name</span></span>  <br/> |<span data-ttu-id="3f413-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3f413-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="3f413-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3f413-137">Validation File</span></span>  <br/> |<span data-ttu-id="3f413-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3f413-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3f413-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3f413-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="3f413-140">False</span><span class="sxs-lookup"><span data-stu-id="3f413-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f413-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3f413-141">See also</span></span>



- [<span data-ttu-id="3f413-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3f413-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

