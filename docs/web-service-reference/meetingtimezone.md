---
title: MeetingTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTimeZone
api_type:
- schema
ms.assetid: 413b47d9-8126-462c-9a4f-4e771a5e8889
description: L’élément MeetingTimeZone représente le fuseau horaire de l’emplacement où la réunion est hébergée.
ms.openlocfilehash: aef4ac4e7571ded6920cbaf90e2895d421068f55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465470"
---
# <a name="meetingtimezone"></a><span data-ttu-id="a7fdc-103">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="a7fdc-103">MeetingTimeZone</span></span>

<span data-ttu-id="a7fdc-104">L’élément **MeetingTimeZone** représente le fuseau horaire de l’emplacement où la réunion est hébergée.</span><span class="sxs-lookup"><span data-stu-id="a7fdc-104">The **MeetingTimeZone** element represents the time zone of the location where the meeting is hosted.</span></span> 
  
```xml
<MeetingTimeZone>
   <BaseOffset/>
   <Standard/>
   <Daylight/>
</MeetingTimeZone>
```

 <span data-ttu-id="a7fdc-105">**TimeZoneType**</span><span class="sxs-lookup"><span data-stu-id="a7fdc-105">**TimeZoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7fdc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a7fdc-106">Attributes and elements</span></span>

<span data-ttu-id="a7fdc-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a7fdc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7fdc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a7fdc-108">Attributes</span></span>

|<span data-ttu-id="a7fdc-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="a7fdc-109">**Attribute**</span></span>|<span data-ttu-id="a7fdc-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7fdc-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7fdc-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="a7fdc-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="a7fdc-112">Décrit le nom du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="a7fdc-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a7fdc-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a7fdc-113">Child elements</span></span>

|<span data-ttu-id="a7fdc-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a7fdc-114">**Element**</span></span>|<span data-ttu-id="a7fdc-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7fdc-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7fdc-116">BaseOffset</span><span class="sxs-lookup"><span data-stu-id="a7fdc-116">BaseOffset</span></span>](baseoffset.md) <br/> |<span data-ttu-id="a7fdc-117">Représente le décalage horaire par rapport à l’heure UTC pour le fuseau horaire actuel.</span><span class="sxs-lookup"><span data-stu-id="a7fdc-117">Represents the hourly offset from UTC for the current time zone.</span></span>  <br/> |
|[<span data-ttu-id="a7fdc-118">Standard</span><span class="sxs-lookup"><span data-stu-id="a7fdc-118">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="a7fdc-119">Représente la date et l’heure auxquelles l’heure passe de l’heure d’été à l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="a7fdc-119">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="a7fdc-120">Auxquelles</span><span class="sxs-lookup"><span data-stu-id="a7fdc-120">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="a7fdc-121">Représente la date et l’heure auxquelles l’heure passe de l’heure standard à l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="a7fdc-121">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a7fdc-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a7fdc-122">Parent elements</span></span>

|<span data-ttu-id="a7fdc-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a7fdc-123">**Element**</span></span>|<span data-ttu-id="a7fdc-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7fdc-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7fdc-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a7fdc-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a7fdc-126">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7fdc-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a7fdc-127">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="a7fdc-127">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a7fdc-128">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7fdc-128">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a7fdc-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="a7fdc-129">Remarks</span></span>

<span data-ttu-id="a7fdc-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a7fdc-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7fdc-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a7fdc-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7fdc-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a7fdc-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7fdc-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a7fdc-133">Schema Name</span></span>  <br/> |<span data-ttu-id="a7fdc-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a7fdc-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7fdc-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a7fdc-135">Validation File</span></span>  <br/> |<span data-ttu-id="a7fdc-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a7fdc-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7fdc-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a7fdc-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7fdc-138">False</span><span class="sxs-lookup"><span data-stu-id="a7fdc-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7fdc-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a7fdc-139">See also</span></span>



- [<span data-ttu-id="a7fdc-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a7fdc-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

