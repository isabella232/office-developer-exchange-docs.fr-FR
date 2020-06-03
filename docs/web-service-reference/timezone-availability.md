---
title: TimeZone (disponibilité)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: L’élément TimeZone contient des éléments qui identifient les informations de fuseau horaire. Cet élément contient également des informations sur la transition entre l’heure standard et l’heure d’été.
ms.openlocfilehash: ba4b0a4805dba54450e01e89c5e9ef746404b716
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460273"
---
# <a name="timezone-availability"></a><span data-ttu-id="3b002-104">TimeZone (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="3b002-104">TimeZone (Availability)</span></span>

<span data-ttu-id="3b002-105">L’élément **TimeZone** contient des éléments qui identifient les informations de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="3b002-105">The **TimeZone** element contains elements that identify time zone information.</span></span> <span data-ttu-id="3b002-106">Cet élément contient également des informations sur la transition entre l’heure standard et l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="3b002-106">This element also contains information about the transition between standard time and daylight saving time.</span></span> 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 <span data-ttu-id="3b002-107">**SerializableTimeZone**</span><span class="sxs-lookup"><span data-stu-id="3b002-107">**SerializableTimeZone**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b002-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3b002-108">Attributes and elements</span></span>

<span data-ttu-id="3b002-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3b002-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b002-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="3b002-110">Attributes</span></span>

<span data-ttu-id="3b002-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3b002-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b002-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3b002-112">Child elements</span></span>

|<span data-ttu-id="3b002-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3b002-113">**Element**</span></span>|<span data-ttu-id="3b002-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3b002-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b002-115">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="3b002-115">Bias (UTC)</span></span>](bias-utc.md) <br/> |<span data-ttu-id="3b002-116">Représente le décalage général par rapport au temps universel coordonné (UTC).</span><span class="sxs-lookup"><span data-stu-id="3b002-116">Represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="3b002-117">Cette valeur est exprimée en minutes.</span><span class="sxs-lookup"><span data-stu-id="3b002-117">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="3b002-118">StandardTime Element</span><span class="sxs-lookup"><span data-stu-id="3b002-118">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="3b002-119">Représente un décalage par rapport à l’heure par rapport à l’heure UTC représentée par l’élément [bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="3b002-119">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="3b002-120">Cet élément contient également des informations sur la transition vers l’heure standard à partir de l’heure d’été dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="3b002-120">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/> |
|[<span data-ttu-id="3b002-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="3b002-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="3b002-122">Représente un décalage entre l’heure par rapport au temps universel coordonné et l’heure UTC représentée par l’élément [bias (UTC)](bias-utc.md) dans les régions où l’heure d’été est observée.</span><span class="sxs-lookup"><span data-stu-id="3b002-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="3b002-123">Cet élément contient également des informations sur le moment où se produit la transition vers l’heure d’été à partir de l’heure standard.</span><span class="sxs-lookup"><span data-stu-id="3b002-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3b002-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3b002-124">Parent elements</span></span>

|<span data-ttu-id="3b002-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3b002-125">**Element**</span></span>|<span data-ttu-id="3b002-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="3b002-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b002-127">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="3b002-127">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="3b002-128">Contient les arguments utilisés pour obtenir les informations de disponibilité de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="3b002-128">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="3b002-129">Il s’agit d’un élément racine.</span><span class="sxs-lookup"><span data-stu-id="3b002-129">This is a root element.</span></span>  <br/> <span data-ttu-id="3b002-130">L’élément **TimeZone** dans le message GetUserAvailabilityRequest représente le fuseau horaire dans lequel les valeurs DateTime de la demande sont spécifiées.</span><span class="sxs-lookup"><span data-stu-id="3b002-130">The **TimeZone** element in the GetUserAvailabilityRequest message represents the time zone in which the DateTime values in the request are specified.</span></span> <span data-ttu-id="3b002-131">Les valeurs DateTime renvoyées par le service de disponibilité sont également dans ce fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="3b002-131">The DateTime values returned by the Availability service are also in this time zone.</span></span>  <br/> <span data-ttu-id="3b002-132">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="3b002-132">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[<span data-ttu-id="3b002-133">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="3b002-133">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3b002-134">Représente les paramètres de fuseau horaire et les heures de travail de l’utilisateur de boîte aux lettres demandé.</span><span class="sxs-lookup"><span data-stu-id="3b002-134">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="3b002-135">L’élément **TimeZone** dans le message GetUserAvailabilityResponse représente les paramètres de fuseau horaire de l’utilisateur de boîte aux lettres demandé.</span><span class="sxs-lookup"><span data-stu-id="3b002-135">The **TimeZone** element in the GetUserAvailabilityResponse message represents the time zone settings of the requested mailbox user.</span></span>  <br/> <span data-ttu-id="3b002-136">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="3b002-136">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3b002-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="3b002-137">Remarks</span></span>

<span data-ttu-id="3b002-138">Cet élément est requis dans l’élément [GetUserAvailabilityRequest](getuseravailabilityrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="3b002-138">This element is required in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) element.</span></span> <span data-ttu-id="3b002-139">Cet élément se produit au plus une fois ou au moins zéro fois lorsque l’élément parent est l’élément [WorkingHours](workinghours-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="3b002-139">This element occurs at most once or at least zero times when the parent element is the [WorkingHours](workinghours-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="3b002-140">Exemple</span><span class="sxs-lookup"><span data-stu-id="3b002-140">Example</span></span>

<span data-ttu-id="3b002-141">L’exemple suivant montre une partie d’une requête XML qui identifie un décalage par rapport à l’heure UTC de 8 heures dans l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="3b002-141">The following example shows part of an XML request that identifies an offset from UTC of 8 hours in the client application.</span></span>
  
```XML
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>11</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>2</DayOrder>
    <Month>3</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="3b002-142">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3b002-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b002-143">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3b002-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b002-144">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3b002-144">Schema Name</span></span>  <br/> |<span data-ttu-id="3b002-145">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3b002-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="3b002-146">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3b002-146">Validation File</span></span>  <br/> |<span data-ttu-id="3b002-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3b002-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3b002-148">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3b002-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b002-149">False</span><span class="sxs-lookup"><span data-stu-id="3b002-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b002-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3b002-150">See also</span></span>



[<span data-ttu-id="3b002-151">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3b002-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="3b002-152">Bias</span><span class="sxs-lookup"><span data-stu-id="3b002-152">Bias</span></span>](bias.md)


[<span data-ttu-id="3b002-153">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="3b002-153">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

