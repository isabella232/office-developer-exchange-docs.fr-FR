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
ms.openlocfilehash: 90eea4fc545fae083e5675225665e517b502ba6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756168"
---
# <a name="end"></a><span data-ttu-id="3e48c-103">End</span><span class="sxs-lookup"><span data-stu-id="3e48c-103">End</span></span>

<span data-ttu-id="3e48c-104">L’élément **End** représente la fin d’une durée.</span><span class="sxs-lookup"><span data-stu-id="3e48c-104">The **End** element represents the end of a duration.</span></span> 
  
```xml
<End/>
```

 <span data-ttu-id="3e48c-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="3e48c-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e48c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3e48c-106">Attributes and elements</span></span>

<span data-ttu-id="3e48c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3e48c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e48c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3e48c-108">Attributes</span></span>

<span data-ttu-id="3e48c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3e48c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e48c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3e48c-110">Child elements</span></span>

<span data-ttu-id="3e48c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3e48c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3e48c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3e48c-112">Parent elements</span></span>

|<span data-ttu-id="3e48c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e48c-113">**Element**</span></span>|<span data-ttu-id="3e48c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e48c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e48c-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="3e48c-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3e48c-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e48c-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3e48c-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="3e48c-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="3e48c-118">Représente la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="3e48c-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3e48c-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="3e48c-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="3e48c-120">Représente la dernière occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="3e48c-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3e48c-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3e48c-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3e48c-122">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e48c-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3e48c-123">Occurrence</span><span class="sxs-lookup"><span data-stu-id="3e48c-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="3e48c-124">Représente une seule occurrence de modification d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="3e48c-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3e48c-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3e48c-125">Text value</span></span>

<span data-ttu-id="3e48c-126">La valeur de texte représente la fin d’une durée.</span><span class="sxs-lookup"><span data-stu-id="3e48c-126">The text value represents the end of a duration.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3e48c-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="3e48c-127">Remarks</span></span>

<span data-ttu-id="3e48c-128">L’opération UpdateItem peut définir l’heure de [début](start.md) et **fin** d’un élément de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e48c-128">The UpdateItem operation can set the [Start](start.md) and **End** time of an Exchange store item.</span></span> <span data-ttu-id="3e48c-129">Dans une demande UpdateItem, vous pouvez définir l’heure de [début](start.md) sans également définir l’heure de **fin** .</span><span class="sxs-lookup"><span data-stu-id="3e48c-129">In an UpdateItem request, you can set the [Start](start.md) time without also setting the **End** time.</span></span> <span data-ttu-id="3e48c-130">Cela peut provoquer une erreur si l’heure de [début](start.md) est postérieure à l’heure de **fin** .</span><span class="sxs-lookup"><span data-stu-id="3e48c-130">This can cause an error if the [Start](start.md) time is later than the **End** time.</span></span> <span data-ttu-id="3e48c-131">Sachez que les applications clientes doivent exécuter à l’heure de **fin** lorsque que l’heure de [début](start.md) est modifiée afin de conserver la durée de corrections.</span><span class="sxs-lookup"><span data-stu-id="3e48c-131">Be aware that client applications must perform adjustments to the **End** time when that [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
 <span data-ttu-id="3e48c-132">**Remarque** Les informations de décalage de fuseau horaire sont perdues si les dates de [début](start.md) et de **fin** de l’élément périodique principal n’ont pas de date qui est égale à la première occurrence d’une périodicité hebdomadaire.</span><span class="sxs-lookup"><span data-stu-id="3e48c-132">**Note** The time zone offset information is lost if the [Start](start.md) and **End** dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="3e48c-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3e48c-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e48c-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3e48c-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e48c-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3e48c-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3e48c-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3e48c-136">Schema Name</span></span>  <br/> |<span data-ttu-id="3e48c-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3e48c-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="3e48c-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3e48c-138">Validation File</span></span>  <br/> |<span data-ttu-id="3e48c-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3e48c-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3e48c-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3e48c-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="3e48c-141">False</span><span class="sxs-lookup"><span data-stu-id="3e48c-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3e48c-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3e48c-142">See also</span></span>



[<span data-ttu-id="3e48c-143">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="3e48c-143">WeeklyRecurrence</span></span>](weeklyrecurrence.md)
  
 <span data-ttu-id="3e48c-144">**End**</span><span class="sxs-lookup"><span data-stu-id="3e48c-144">**End**</span></span>


- [<span data-ttu-id="3e48c-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3e48c-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

