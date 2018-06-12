---
title: AppointmentState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentState
api_type:
- schema
ms.assetid: ab3f5d04-ace1-4a15-9107-cefa6c41abc7
description: L’élément AppointmentState Spécifie l’état du rendez-vous.
ms.openlocfilehash: 05e92a3fea10a84518b0680c425011a91bc43d93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755306"
---
# <a name="appointmentstate"></a><span data-ttu-id="731ad-103">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="731ad-103">AppointmentState</span></span>

<span data-ttu-id="731ad-104">L’élément **AppointmentState** Spécifie l’état du rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="731ad-104">The **AppointmentState** element specifies the status of the appointment.</span></span> 
  
```XML
<AppointmentState/>
```

 <span data-ttu-id="731ad-105">**int**</span><span class="sxs-lookup"><span data-stu-id="731ad-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="731ad-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="731ad-106">Attributes and elements</span></span>

<span data-ttu-id="731ad-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="731ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="731ad-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="731ad-108">Attributes</span></span>

<span data-ttu-id="731ad-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="731ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="731ad-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="731ad-110">Child elements</span></span>

<span data-ttu-id="731ad-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="731ad-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="731ad-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="731ad-112">Parent elements</span></span>

|<span data-ttu-id="731ad-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="731ad-113">**Element**</span></span>|<span data-ttu-id="731ad-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="731ad-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="731ad-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="731ad-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="731ad-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="731ad-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="731ad-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="731ad-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="731ad-118">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="731ad-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="731ad-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="731ad-119">Text value</span></span>

<span data-ttu-id="731ad-120">Cet élément contient une valeur de texte que représente la valeur bits.</span><span class="sxs-lookup"><span data-stu-id="731ad-120">This element contains a text value that represents set bits.</span></span> <span data-ttu-id="731ad-121">Il s’agit de formulaire entier.</span><span class="sxs-lookup"><span data-stu-id="731ad-121">This is in integer form.</span></span> <span data-ttu-id="731ad-122">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="731ad-122">This element is read-only.</span></span> <span data-ttu-id="731ad-123">Il sera renvoyée uniquement dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="731ad-123">It will only be returned in a response.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="731ad-124">Note</span><span class="sxs-lookup"><span data-stu-id="731ad-124">Remarks</span></span>

<span data-ttu-id="731ad-125">Valeur entière qui est renvoyée représente le masque de bits état rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="731ad-125">The integer value that is returned represents the appointment state bitmask.</span></span> <span data-ttu-id="731ad-126">Le tableau suivant décrit chaque bit.</span><span class="sxs-lookup"><span data-stu-id="731ad-126">The following table describes each bit.</span></span>
  
|<span data-ttu-id="731ad-127">**Name**</span><span class="sxs-lookup"><span data-stu-id="731ad-127">**Name**</span></span>|<span data-ttu-id="731ad-128">**Bit**</span><span class="sxs-lookup"><span data-stu-id="731ad-128">**Bit**</span></span>|<span data-ttu-id="731ad-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="731ad-129">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="731ad-130">None</span><span class="sxs-lookup"><span data-stu-id="731ad-130">None</span></span>  <br/> |<span data-ttu-id="731ad-131">0x0000</span><span class="sxs-lookup"><span data-stu-id="731ad-131">0x0000</span></span>  <br/> |<span data-ttu-id="731ad-132">Aucun indicateur n’ont été définies.</span><span class="sxs-lookup"><span data-stu-id="731ad-132">No flags have been set.</span></span> <span data-ttu-id="731ad-133">Il est uniquement utilisé pour un rendez-vous qui n’inclut pas les participants.</span><span class="sxs-lookup"><span data-stu-id="731ad-133">This is only used for an appointment that does not include attendees.</span></span>  <br/> |
|<span data-ttu-id="731ad-134">Réunion</span><span class="sxs-lookup"><span data-stu-id="731ad-134">Meeting</span></span>  <br/> |<span data-ttu-id="731ad-135">0x0001</span><span class="sxs-lookup"><span data-stu-id="731ad-135">0x0001</span></span>  <br/> |<span data-ttu-id="731ad-136">Ce rendez-vous est une réunion.</span><span class="sxs-lookup"><span data-stu-id="731ad-136">This appointment is a meeting.</span></span>  <br/> |
|<span data-ttu-id="731ad-137">Received</span><span class="sxs-lookup"><span data-stu-id="731ad-137">Received</span></span>  <br/> |<span data-ttu-id="731ad-138">0x0002</span><span class="sxs-lookup"><span data-stu-id="731ad-138">0x0002</span></span>  <br/> |<span data-ttu-id="731ad-139">Ce rendez-vous a été reçu.</span><span class="sxs-lookup"><span data-stu-id="731ad-139">This appointment has been received.</span></span>  <br/> |
|<span data-ttu-id="731ad-140">Annulé</span><span class="sxs-lookup"><span data-stu-id="731ad-140">Canceled</span></span>  <br/> |<span data-ttu-id="731ad-141">0x0004</span><span class="sxs-lookup"><span data-stu-id="731ad-141">0x0004</span></span>  <br/> |<span data-ttu-id="731ad-142">Ce rendez-vous a été annulé.</span><span class="sxs-lookup"><span data-stu-id="731ad-142">This appointment has been canceled.</span></span>  <br/> |
   
<span data-ttu-id="731ad-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="731ad-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="731ad-144">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="731ad-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="731ad-145">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="731ad-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="731ad-146">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="731ad-146">Schema name</span></span>  <br/> |<span data-ttu-id="731ad-147">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="731ad-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="731ad-148">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="731ad-148">Validation file</span></span>  <br/> |<span data-ttu-id="731ad-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="731ad-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="731ad-150">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="731ad-150">Can be empty</span></span>  <br/> |<span data-ttu-id="731ad-151">False</span><span class="sxs-lookup"><span data-stu-id="731ad-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="731ad-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="731ad-152">See also</span></span>

- [<span data-ttu-id="731ad-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="731ad-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

