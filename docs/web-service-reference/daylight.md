---
title: Heure d’été
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Daylight
api_type:
- schema
ms.assetid: ea400839-fba8-4a5e-a5d1-9b677afc0ff9
description: L’élément de l’heure d’été représente la date et l’heure de l’heure de modification de l’heure standard à l’heure.
ms.openlocfilehash: cdb6ed305f1d77a73b952f8c659991f3b2a8df7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755815"
---
# <a name="daylight"></a><span data-ttu-id="bbe71-103">Heure d’été</span><span class="sxs-lookup"><span data-stu-id="bbe71-103">Daylight</span></span>

<span data-ttu-id="bbe71-104">L’élément de **l’heure d’été** représente la date et l’heure de l’heure de modification de l’heure standard à l’heure.</span><span class="sxs-lookup"><span data-stu-id="bbe71-104">The **Daylight** element represents the date and time when the time changes from standard time to daylight saving time.</span></span> 
  
```xml
<Daylight TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Daylight>
```

```xml
<Daylight TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Daylight>
```

<span data-ttu-id="bbe71-105">**TimeChangeType**</span><span class="sxs-lookup"><span data-stu-id="bbe71-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bbe71-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bbe71-106">Attributes and elements</span></span>

<span data-ttu-id="bbe71-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bbe71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bbe71-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bbe71-108">Attributes</span></span>

|<span data-ttu-id="bbe71-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bbe71-109">**Attribute**</span></span>|<span data-ttu-id="bbe71-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="bbe71-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bbe71-111">**NomFuseauhoraire**</span><span class="sxs-lookup"><span data-stu-id="bbe71-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="bbe71-112">Indique le nom du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bbe71-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bbe71-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bbe71-113">Child elements</span></span>

|<span data-ttu-id="bbe71-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bbe71-114">**Element**</span></span>|<span data-ttu-id="bbe71-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="bbe71-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bbe71-116">Offset</span><span class="sxs-lookup"><span data-stu-id="bbe71-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="bbe71-117">Indique le décalage à partir de la [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="bbe71-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="bbe71-118">La base de décalage Outre cet offset identifie l’heure selon qu’il soit standard ou de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="bbe71-118">The base offset in addition to this offset identifies the time according to whether it is standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="bbe71-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="bbe71-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="bbe71-120">Décrit une périodicité annuelle relative d’un modèle de date de transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bbe71-120">Describes a relative yearly recurrence pattern for a time zone transition date pattern.</span></span>  <br/> |
|[<span data-ttu-id="bbe71-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="bbe71-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="bbe71-122">Représente la date à laquelle l’heure passe à partir de standard ou l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="bbe71-122">Represents the date when the time changes from standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="bbe71-123">Heure (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="bbe71-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="bbe71-124">Indique l’heure de l’heure de modification entre heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="bbe71-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bbe71-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bbe71-125">Parent elements</span></span>

|<span data-ttu-id="bbe71-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bbe71-126">**Element**</span></span>|<span data-ttu-id="bbe71-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="bbe71-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bbe71-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="bbe71-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="bbe71-129">Représente le fuseau horaire de l’emplacement où se trouve la réunion.</span><span class="sxs-lookup"><span data-stu-id="bbe71-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bbe71-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="bbe71-130">Remarks</span></span>

<span data-ttu-id="bbe71-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="bbe71-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bbe71-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bbe71-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bbe71-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bbe71-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bbe71-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bbe71-134">Schema Name</span></span>  <br/> |<span data-ttu-id="bbe71-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bbe71-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="bbe71-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bbe71-136">Validation File</span></span>  <br/> |<span data-ttu-id="bbe71-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bbe71-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bbe71-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bbe71-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="bbe71-139">False</span><span class="sxs-lookup"><span data-stu-id="bbe71-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bbe71-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bbe71-140">See also</span></span>

- [<span data-ttu-id="bbe71-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bbe71-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

