---
title: Périodes
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
description: L’élément périodes représente un tableau de points qui définissent le décalage de temps à différents stades du fuseau horaire.
ms.openlocfilehash: f2f9cf7c724b453d2b1975fcf72c55bc02caa54b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828729"
---
# <a name="periods"></a><span data-ttu-id="71ad3-103">Périodes</span><span class="sxs-lookup"><span data-stu-id="71ad3-103">Periods</span></span>

<span data-ttu-id="71ad3-104">L’élément **périodes** représente un tableau de points qui définissent le décalage de temps à différents stades du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="71ad3-104">The **Periods** element represents an array of periods that define the time offset at different stages of the time zone.</span></span> 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 <span data-ttu-id="71ad3-105">**NonEmptyArrayOfPeriodsType**</span><span class="sxs-lookup"><span data-stu-id="71ad3-105">**NonEmptyArrayOfPeriodsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71ad3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="71ad3-106">Attributes and elements</span></span>

<span data-ttu-id="71ad3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="71ad3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71ad3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="71ad3-108">Attributes</span></span>

<span data-ttu-id="71ad3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="71ad3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71ad3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="71ad3-110">Child elements</span></span>

|<span data-ttu-id="71ad3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="71ad3-111">**Element**</span></span>|<span data-ttu-id="71ad3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="71ad3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71ad3-113">Period</span><span class="sxs-lookup"><span data-stu-id="71ad3-113">Period</span></span>](period.md) <br/> |<span data-ttu-id="71ad3-114">Définit le nom, le décalage et l’identificateur unique pour une étape spécifique du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="71ad3-114">Defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71ad3-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="71ad3-115">Parent elements</span></span>

|<span data-ttu-id="71ad3-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="71ad3-116">**Element**</span></span>|<span data-ttu-id="71ad3-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="71ad3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71ad3-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="71ad3-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="71ad3-119">Définit le fuseau horaire pour l’heure de début d’un [CalendarItem](calendaritem.md) [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="71ad3-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="71ad3-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="71ad3-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="71ad3-121">Définit le fuseau horaire pour l’heure de fin d’un [CalendarItem](calendaritem.md) [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="71ad3-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="71ad3-122">Définition de fuseau horaire</span><span class="sxs-lookup"><span data-stu-id="71ad3-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="71ad3-123">Définit un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="71ad3-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="71ad3-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="71ad3-124">Remarks</span></span>

<span data-ttu-id="71ad3-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="71ad3-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71ad3-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="71ad3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71ad3-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="71ad3-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71ad3-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="71ad3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="71ad3-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="71ad3-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="71ad3-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="71ad3-130">Validation File</span></span>  <br/> |<span data-ttu-id="71ad3-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="71ad3-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71ad3-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="71ad3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="71ad3-133">False</span><span class="sxs-lookup"><span data-stu-id="71ad3-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71ad3-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="71ad3-134">See also</span></span>



- [<span data-ttu-id="71ad3-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="71ad3-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

