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
description: L’élément standard représente la date et l’heure auxquelles l’heure passe de l’heure d’été à l’heure standard.
ms.openlocfilehash: 1214a1debb53c9a31ca7c92a0c9e5c0722960d75
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467563"
---
# <a name="standard"></a><span data-ttu-id="1bc38-103">Standard</span><span class="sxs-lookup"><span data-stu-id="1bc38-103">Standard</span></span>

<span data-ttu-id="1bc38-104">L’élément **standard** représente la date et l’heure auxquelles l’heure passe de l’heure d’été à l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="1bc38-104">The **Standard** element represents the date and time when the time changes from daylight saving time to standard time.</span></span> 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
```

```xml
<Standard TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Standard>
```

<span data-ttu-id="1bc38-105">**TimeChangeType**</span><span class="sxs-lookup"><span data-stu-id="1bc38-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1bc38-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1bc38-106">Attributes and elements</span></span>

<span data-ttu-id="1bc38-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1bc38-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1bc38-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1bc38-108">Attributes</span></span>

|<span data-ttu-id="1bc38-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1bc38-109">**Attribute**</span></span>|<span data-ttu-id="1bc38-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="1bc38-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1bc38-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="1bc38-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="1bc38-112">Décrit le nom du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="1bc38-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1bc38-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1bc38-113">Child elements</span></span>

|<span data-ttu-id="1bc38-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1bc38-114">**Element**</span></span>|<span data-ttu-id="1bc38-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="1bc38-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bc38-116">Offset</span><span class="sxs-lookup"><span data-stu-id="1bc38-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="1bc38-117">Décrit le décalage par rapport à l' [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="1bc38-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="1bc38-118">Avec l’élément **BaseOffset** , l’élément **offset** identifie s’il s’agit de l’heure standard ou de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="1bc38-118">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="1bc38-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="1bc38-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="1bc38-120">Décrit un modèle de périodicité annuelle relative pour une date de transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="1bc38-120">Describes a relative yearly recurrence pattern for a time zone transition date.</span></span>  <br/> |
|[<span data-ttu-id="1bc38-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="1bc38-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="1bc38-122">Représente la date à laquelle le temps passe de l’heure standard ou de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="1bc38-122">Represents the date when the time changes from standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="1bc38-123">Heure (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="1bc38-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="1bc38-124">Décrit le moment où l’heure change entre l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="1bc38-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1bc38-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1bc38-125">Parent elements</span></span>

|<span data-ttu-id="1bc38-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1bc38-126">**Element**</span></span>|<span data-ttu-id="1bc38-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="1bc38-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1bc38-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="1bc38-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="1bc38-129">Représente le fuseau horaire de l’emplacement où la réunion est hébergée.</span><span class="sxs-lookup"><span data-stu-id="1bc38-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1bc38-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="1bc38-130">Remarks</span></span>

<span data-ttu-id="1bc38-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1bc38-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1bc38-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1bc38-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1bc38-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1bc38-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1bc38-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1bc38-134">Schema Name</span></span>  <br/> |<span data-ttu-id="1bc38-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1bc38-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="1bc38-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1bc38-136">Validation File</span></span>  <br/> |<span data-ttu-id="1bc38-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1bc38-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1bc38-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1bc38-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="1bc38-139">False</span><span class="sxs-lookup"><span data-stu-id="1bc38-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1bc38-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1bc38-140">See also</span></span>

- [<span data-ttu-id="1bc38-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1bc38-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

