---
title: StartTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeZone
api_type:
- schema
ms.assetid: d38c4dc1-4ecb-42a1-8d57-a451b16a2de2
description: L’élément StartTimeZone définit le fuseau horaire pour l’heure de début d’un CalendarItem ou d’un propriété meetingrequest.
ms.openlocfilehash: fa88f676c0f6a7a2e934f51274942ed3bccbc789
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458522"
---
# <a name="starttimezone"></a><span data-ttu-id="a21e8-103">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="a21e8-103">StartTimeZone</span></span>

<span data-ttu-id="a21e8-104">L’élément **StartTimeZone** définit le fuseau horaire pour l’heure de début d’un [CalendarItem](calendaritem.md) ou d’un [propriété meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="a21e8-104">The **StartTimeZone** element defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<StartTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</StartTimeZone>
```

<span data-ttu-id="a21e8-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="a21e8-105">**TimeZoneDefinitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a21e8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a21e8-106">Attributes and elements</span></span>

<span data-ttu-id="a21e8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a21e8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a21e8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a21e8-108">Attributes</span></span>

|<span data-ttu-id="a21e8-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a21e8-109">**Attribute**</span></span>|<span data-ttu-id="a21e8-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="a21e8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a21e8-111">ID</span><span class="sxs-lookup"><span data-stu-id="a21e8-111">Id</span></span>  <br/> |<span data-ttu-id="a21e8-112">Représente l’identificateur unique de la définition du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="a21e8-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="a21e8-113">Nom</span><span class="sxs-lookup"><span data-stu-id="a21e8-113">Name</span></span>  <br/> |<span data-ttu-id="a21e8-114">Représente le nom descriptif de la définition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="a21e8-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a21e8-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a21e8-115">Child elements</span></span>

|<span data-ttu-id="a21e8-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a21e8-116">**Element**</span></span>|<span data-ttu-id="a21e8-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="a21e8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a21e8-118">Periods</span><span class="sxs-lookup"><span data-stu-id="a21e8-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="a21e8-119">Représente un tableau d’éléments [period](period.md) qui définissent le décalage temporel à différentes étapes du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="a21e8-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="a21e8-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="a21e8-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="a21e8-121">Représente un tableau d’éléments [TransitionsGroup](transitionsgroup.md) qui spécifient des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="a21e8-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="a21e8-122">Transitions</span><span class="sxs-lookup"><span data-stu-id="a21e8-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="a21e8-123">Représente un tableau de transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="a21e8-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a21e8-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a21e8-124">Parent elements</span></span>

|<span data-ttu-id="a21e8-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a21e8-125">**Element**</span></span>|<span data-ttu-id="a21e8-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="a21e8-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a21e8-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a21e8-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a21e8-128">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="a21e8-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a21e8-129">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="a21e8-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a21e8-130">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a21e8-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a21e8-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="a21e8-131">Remarks</span></span>

<span data-ttu-id="a21e8-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a21e8-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a21e8-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a21e8-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a21e8-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a21e8-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a21e8-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a21e8-135">Schema Name</span></span>  <br/> |<span data-ttu-id="a21e8-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a21e8-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="a21e8-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a21e8-137">Validation File</span></span>  <br/> |<span data-ttu-id="a21e8-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a21e8-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a21e8-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a21e8-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="a21e8-140">False</span><span class="sxs-lookup"><span data-stu-id="a21e8-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a21e8-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a21e8-141">See also</span></span>

- [<span data-ttu-id="a21e8-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a21e8-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

