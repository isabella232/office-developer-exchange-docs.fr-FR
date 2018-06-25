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
description: L’élément MeetingTimeZone représente le fuseau horaire de l’emplacement où se trouve la réunion.
ms.openlocfilehash: ce014ac6d8841e451927a94049cb4e8860886fdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828440"
---
# <a name="meetingtimezone"></a><span data-ttu-id="d4878-103">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="d4878-103">MeetingTimeZone</span></span>

<span data-ttu-id="d4878-104">L’élément **MeetingTimeZone** représente le fuseau horaire de l’emplacement où se trouve la réunion.</span><span class="sxs-lookup"><span data-stu-id="d4878-104">The **MeetingTimeZone** element represents the time zone of the location where the meeting is hosted.</span></span> 
  
```xml
<MeetingTimeZone>
   <BaseOffset/>
   <Standard/>
   <Daylight/>
</MeetingTimeZone>
```

 <span data-ttu-id="d4878-105">**TimeZoneType**</span><span class="sxs-lookup"><span data-stu-id="d4878-105">**TimeZoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4878-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4878-106">Attributes and elements</span></span>

<span data-ttu-id="d4878-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4878-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4878-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4878-108">Attributes</span></span>

|<span data-ttu-id="d4878-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d4878-109">**Attribute**</span></span>|<span data-ttu-id="d4878-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4878-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4878-111">**NomFuseauhoraire**</span><span class="sxs-lookup"><span data-stu-id="d4878-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="d4878-112">Indique le nom du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="d4878-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d4878-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4878-113">Child elements</span></span>

|<span data-ttu-id="d4878-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4878-114">**Element**</span></span>|<span data-ttu-id="d4878-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4878-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4878-116">BaseOffset</span><span class="sxs-lookup"><span data-stu-id="d4878-116">BaseOffset</span></span>](baseoffset.md) <br/> |<span data-ttu-id="d4878-117">Représente les heures décalée par rapport à l’heure UTC pour le fuseau horaire actuel.</span><span class="sxs-lookup"><span data-stu-id="d4878-117">Represents the hourly offset from UTC for the current time zone.</span></span>  <br/> |
|[<span data-ttu-id="d4878-118">Standard</span><span class="sxs-lookup"><span data-stu-id="d4878-118">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="d4878-119">Représente la date et l’heure de l’heure de modification de l’heure à l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="d4878-119">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="d4878-120">Heure d’été</span><span class="sxs-lookup"><span data-stu-id="d4878-120">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="d4878-121">Représente la date et l’heure de l’heure de modification de l’heure standard à l’heure.</span><span class="sxs-lookup"><span data-stu-id="d4878-121">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4878-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4878-122">Parent elements</span></span>

|<span data-ttu-id="d4878-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4878-123">**Element**</span></span>|<span data-ttu-id="d4878-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4878-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4878-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d4878-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d4878-126">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4878-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d4878-127">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d4878-127">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d4878-128">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4878-128">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d4878-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="d4878-129">Remarks</span></span>

<span data-ttu-id="d4878-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d4878-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4878-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4878-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4878-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4878-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4878-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4878-133">Schema Name</span></span>  <br/> |<span data-ttu-id="d4878-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d4878-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4878-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4878-135">Validation File</span></span>  <br/> |<span data-ttu-id="d4878-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4878-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4878-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4878-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4878-138">False</span><span class="sxs-lookup"><span data-stu-id="d4878-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4878-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4878-139">See also</span></span>



- [<span data-ttu-id="d4878-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d4878-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

