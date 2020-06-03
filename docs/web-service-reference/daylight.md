---
title: Auxquelles
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
description: L’élément d’heure représente la date et l’heure auxquelles le temps passe de l’heure standard à l’heure d’été.
ms.openlocfilehash: bf2041cb4677f837ddb5b399041f1c19a7b5f577
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457458"
---
# <a name="daylight"></a><span data-ttu-id="3220e-103">Auxquelles</span><span class="sxs-lookup"><span data-stu-id="3220e-103">Daylight</span></span>

<span data-ttu-id="3220e-104">L’élément d' **heure** représente la date et l’heure auxquelles le temps passe de l’heure standard à l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="3220e-104">The **Daylight** element represents the date and time when the time changes from standard time to daylight saving time.</span></span> 
  
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

<span data-ttu-id="3220e-105">**TimeChangeType**</span><span class="sxs-lookup"><span data-stu-id="3220e-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3220e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3220e-106">Attributes and elements</span></span>

<span data-ttu-id="3220e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3220e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3220e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3220e-108">Attributes</span></span>

|<span data-ttu-id="3220e-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="3220e-109">**Attribute**</span></span>|<span data-ttu-id="3220e-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="3220e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3220e-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="3220e-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="3220e-112">Décrit le nom du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="3220e-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3220e-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3220e-113">Child elements</span></span>

|<span data-ttu-id="3220e-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3220e-114">**Element**</span></span>|<span data-ttu-id="3220e-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="3220e-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3220e-116">Offset</span><span class="sxs-lookup"><span data-stu-id="3220e-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="3220e-117">Décrit le décalage par rapport à l' [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="3220e-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="3220e-118">Le décalage de base en plus de ce décalage identifie le temps en fonction de l’heure standard ou de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="3220e-118">The base offset in addition to this offset identifies the time according to whether it is standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="3220e-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="3220e-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="3220e-120">Décrit un modèle de périodicité annuelle relative pour un modèle de date de transition de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="3220e-120">Describes a relative yearly recurrence pattern for a time zone transition date pattern.</span></span>  <br/> |
|[<span data-ttu-id="3220e-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="3220e-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="3220e-122">Représente la date à laquelle le temps passe de standard ou de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="3220e-122">Represents the date when the time changes from standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="3220e-123">Heure (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="3220e-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="3220e-124">Décrit le moment où l’heure change entre l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="3220e-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3220e-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3220e-125">Parent elements</span></span>

|<span data-ttu-id="3220e-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3220e-126">**Element**</span></span>|<span data-ttu-id="3220e-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="3220e-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3220e-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="3220e-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="3220e-129">Représente le fuseau horaire de l’emplacement où la réunion est hébergée.</span><span class="sxs-lookup"><span data-stu-id="3220e-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3220e-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="3220e-130">Remarks</span></span>

<span data-ttu-id="3220e-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3220e-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3220e-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3220e-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3220e-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3220e-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3220e-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3220e-134">Schema Name</span></span>  <br/> |<span data-ttu-id="3220e-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3220e-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="3220e-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3220e-136">Validation File</span></span>  <br/> |<span data-ttu-id="3220e-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3220e-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3220e-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3220e-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="3220e-139">False</span><span class="sxs-lookup"><span data-stu-id="3220e-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3220e-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3220e-140">See also</span></span>

- [<span data-ttu-id="3220e-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3220e-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

