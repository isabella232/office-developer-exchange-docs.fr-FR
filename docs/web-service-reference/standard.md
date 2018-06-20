---
title: Standard
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Standard
api_type:
- schema
ms.assetid: d598f0a6-e296-423f-8ce5-3da57cfd8189
description: L’élément Standard représente la date et l’heure de l’heure de modification de l’heure à l’heure standard.
ms.openlocfilehash: 1c9be4cf35773583078bc8e16ddf44433d3ad98c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829536"
---
# <a name="standard"></a><span data-ttu-id="2628c-103">Standard</span><span class="sxs-lookup"><span data-stu-id="2628c-103">Standard</span></span>

<span data-ttu-id="2628c-104">L’élément **Standard** représente la date et l’heure de l’heure de modification de l’heure à l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="2628c-104">The **Standard** element represents the date and time when the time changes from daylight saving time to standard time.</span></span> 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
```

 <span data-ttu-id="2628c-105">**TimeChangeType**</span><span class="sxs-lookup"><span data-stu-id="2628c-105">**TimeChangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2628c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2628c-106">Attributes and elements</span></span>

<span data-ttu-id="2628c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2628c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2628c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2628c-108">Attributes</span></span>

|<span data-ttu-id="2628c-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="2628c-109">**Attribute**</span></span>|<span data-ttu-id="2628c-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="2628c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2628c-111">**NomFuseauhoraire**</span><span class="sxs-lookup"><span data-stu-id="2628c-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="2628c-112">Indique le nom du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="2628c-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2628c-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2628c-113">Child elements</span></span>

|<span data-ttu-id="2628c-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2628c-114">**Element**</span></span>|<span data-ttu-id="2628c-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="2628c-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2628c-116">Offset</span><span class="sxs-lookup"><span data-stu-id="2628c-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="2628c-117">Indique le décalage à partir de la [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="2628c-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="2628c-118">Avec l’élément **BaseOffset** , l’élément **décalée** identifie si le temps est l’heure standard ou l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="2628c-118">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="2628c-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="2628c-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="2628c-120">Décrit une périodicité annuelle relative à une date de transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="2628c-120">Describes a relative yearly recurrence pattern for a time zone transition date.</span></span>  <br/> |
|[<span data-ttu-id="2628c-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="2628c-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="2628c-122">Représente la date à laquelle l’heure passe d’heure standard ou l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="2628c-122">Represents the date when the time changes from standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="2628c-123">Heure (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="2628c-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="2628c-124">Indique l’heure de l’heure de modification entre heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="2628c-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2628c-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2628c-125">Parent elements</span></span>

|<span data-ttu-id="2628c-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2628c-126">**Element**</span></span>|<span data-ttu-id="2628c-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="2628c-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2628c-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="2628c-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="2628c-129">Représente le fuseau horaire de l’emplacement où se trouve la réunion.</span><span class="sxs-lookup"><span data-stu-id="2628c-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2628c-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="2628c-130">Remarks</span></span>

<span data-ttu-id="2628c-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2628c-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2628c-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2628c-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2628c-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2628c-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2628c-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2628c-134">Schema Name</span></span>  <br/> |<span data-ttu-id="2628c-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2628c-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="2628c-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2628c-136">Validation File</span></span>  <br/> |<span data-ttu-id="2628c-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2628c-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2628c-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2628c-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="2628c-139">False</span><span class="sxs-lookup"><span data-stu-id="2628c-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2628c-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2628c-140">See also</span></span>



- [<span data-ttu-id="2628c-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2628c-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

