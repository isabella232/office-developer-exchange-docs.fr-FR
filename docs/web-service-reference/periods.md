---
title: Periods
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Periods
api_type:
- schema
ms.assetid: 7920d81d-abba-4232-8bfe-49267b6c9a36
description: L’élément periods représente un tableau de périodes qui définissent le décalage temporel à différentes étapes du fuseau horaire.
ms.openlocfilehash: 773457a6e4c0237eaeaf23109a7022427cc7dd0d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467773"
---
# <a name="periods"></a><span data-ttu-id="22032-103">Periods</span><span class="sxs-lookup"><span data-stu-id="22032-103">Periods</span></span>

<span data-ttu-id="22032-104">L’élément **periods** représente un tableau de périodes qui définissent le décalage temporel à différentes étapes du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="22032-104">The **Periods** element represents an array of periods that define the time offset at different stages of the time zone.</span></span> 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 <span data-ttu-id="22032-105">**NonEmptyArrayOfPeriodsType**</span><span class="sxs-lookup"><span data-stu-id="22032-105">**NonEmptyArrayOfPeriodsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22032-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="22032-106">Attributes and elements</span></span>

<span data-ttu-id="22032-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="22032-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22032-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="22032-108">Attributes</span></span>

<span data-ttu-id="22032-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="22032-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22032-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="22032-110">Child elements</span></span>

|<span data-ttu-id="22032-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22032-111">**Element**</span></span>|<span data-ttu-id="22032-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="22032-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22032-113">Period</span><span class="sxs-lookup"><span data-stu-id="22032-113">Period</span></span>](period.md) <br/> |<span data-ttu-id="22032-114">Définit le nom, le décalage temporel et l’identificateur unique pour une étape spécifique du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="22032-114">Defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22032-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="22032-115">Parent elements</span></span>

|<span data-ttu-id="22032-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22032-116">**Element**</span></span>|<span data-ttu-id="22032-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="22032-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22032-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="22032-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="22032-119">Définit le fuseau horaire pour l’heure de début d’une [CalendarItem](calendaritem.md) ou d’un [propriété meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="22032-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="22032-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="22032-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="22032-121">Définit le fuseau horaire pour l’heure de fin d’une [CalendarItem](calendaritem.md) ou d’un [propriété meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="22032-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="22032-122">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="22032-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="22032-123">Définit un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="22032-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="22032-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="22032-124">Remarks</span></span>

<span data-ttu-id="22032-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="22032-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22032-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="22032-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22032-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="22032-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22032-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="22032-128">Schema Name</span></span>  <br/> |<span data-ttu-id="22032-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="22032-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="22032-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="22032-130">Validation File</span></span>  <br/> |<span data-ttu-id="22032-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="22032-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="22032-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="22032-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="22032-133">False</span><span class="sxs-lookup"><span data-stu-id="22032-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22032-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="22032-134">See also</span></span>



- [<span data-ttu-id="22032-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="22032-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

