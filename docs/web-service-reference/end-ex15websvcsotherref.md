---
title: End
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- End
api_type:
- schema
ms.assetid: 72329821-32ff-495d-b6e5-fdc011003c2e
description: L’élément End représente la fin d’une durée.
ms.openlocfilehash: d36f555d2ac9c0c1d82053029720ec17a53f2d92
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456142"
---
# <a name="end"></a><span data-ttu-id="b930f-103">End</span><span class="sxs-lookup"><span data-stu-id="b930f-103">End</span></span>

<span data-ttu-id="b930f-104">L’élément **end** représente la fin d’une durée.</span><span class="sxs-lookup"><span data-stu-id="b930f-104">The **End** element represents the end of a duration.</span></span> 
  
```xml
<End/>
```

 <span data-ttu-id="b930f-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="b930f-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b930f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b930f-106">Attributes and elements</span></span>

<span data-ttu-id="b930f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b930f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b930f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b930f-108">Attributes</span></span>

<span data-ttu-id="b930f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b930f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b930f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b930f-110">Child elements</span></span>

<span data-ttu-id="b930f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b930f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b930f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b930f-112">Parent elements</span></span>

|<span data-ttu-id="b930f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b930f-113">**Element**</span></span>|<span data-ttu-id="b930f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b930f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b930f-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="b930f-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b930f-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="b930f-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b930f-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="b930f-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="b930f-118">Représente la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="b930f-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b930f-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="b930f-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="b930f-120">Représente la dernière occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="b930f-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b930f-121">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="b930f-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b930f-122">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b930f-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b930f-123">Réunions</span><span class="sxs-lookup"><span data-stu-id="b930f-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="b930f-124">Représente une occurrence modifiée unique d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="b930f-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b930f-125">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="b930f-125">Text value</span></span>

<span data-ttu-id="b930f-126">La valeur de texte représente la fin d’une durée.</span><span class="sxs-lookup"><span data-stu-id="b930f-126">The text value represents the end of a duration.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b930f-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="b930f-127">Remarks</span></span>

<span data-ttu-id="b930f-128">L’opération UpdateItem peut définir l’heure de [début](start.md) et de **fin** d’un élément de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="b930f-128">The UpdateItem operation can set the [Start](start.md) and **End** time of an Exchange store item.</span></span> <span data-ttu-id="b930f-129">Dans une requête UpdateItem, vous pouvez définir l’heure de [début](start.md) sans définir également l’heure de **fin** .</span><span class="sxs-lookup"><span data-stu-id="b930f-129">In an UpdateItem request, you can set the [Start](start.md) time without also setting the **End** time.</span></span> <span data-ttu-id="b930f-130">Cela peut entraîner une erreur si l’heure de [début](start.md) est postérieure à l’heure de **fin** .</span><span class="sxs-lookup"><span data-stu-id="b930f-130">This can cause an error if the [Start](start.md) time is later than the **End** time.</span></span> <span data-ttu-id="b930f-131">N’oubliez pas que les applications clientes doivent effectuer des ajustements à l’heure de **fin** lorsque cette heure de [début](start.md) est modifiée afin de conserver la durée.</span><span class="sxs-lookup"><span data-stu-id="b930f-131">Be aware that client applications must perform adjustments to the **End** time when that [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
 <span data-ttu-id="b930f-132">**Note** Les informations de décalage de fuseau horaire sont perdues si les dates de [début](start.md) et de **fin** de l’élément de gabarit périodique n’ont pas de date égale à la première occurrence d’une périodicité hebdomadaire.</span><span class="sxs-lookup"><span data-stu-id="b930f-132">**Note** The time zone offset information is lost if the [Start](start.md) and **End** dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="b930f-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b930f-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b930f-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b930f-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b930f-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b930f-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b930f-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b930f-136">Schema Name</span></span>  <br/> |<span data-ttu-id="b930f-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b930f-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="b930f-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b930f-138">Validation File</span></span>  <br/> |<span data-ttu-id="b930f-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b930f-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b930f-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b930f-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="b930f-141">False</span><span class="sxs-lookup"><span data-stu-id="b930f-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b930f-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b930f-142">See also</span></span>



[<span data-ttu-id="b930f-143">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="b930f-143">WeeklyRecurrence</span></span>](weeklyrecurrence.md)
  
 <span data-ttu-id="b930f-144">**End**</span><span class="sxs-lookup"><span data-stu-id="b930f-144">**End**</span></span>


- [<span data-ttu-id="b930f-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b930f-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

