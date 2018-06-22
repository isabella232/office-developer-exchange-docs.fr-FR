---
title: ExtendedProperty
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExtendedProperty
api_type:
- schema
ms.assetid: f9701409-b620-4afe-b9ee-4c1e95507af7
description: L’élément ExtendedProperty identifie les propriétés MAPI étendues sur les dossiers et éléments.
ms.openlocfilehash: 6a0aecc732ef634c2258127fca89b19461e25762
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756293"
---
# <a name="extendedproperty"></a><span data-ttu-id="10de6-103">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="10de6-103">ExtendedProperty</span></span>

<span data-ttu-id="10de6-104">L’élément **ExtendedProperty** identifie les propriétés MAPI étendues sur les dossiers et éléments.</span><span class="sxs-lookup"><span data-stu-id="10de6-104">The **ExtendedProperty** element identifies extended MAPI properties on folders and items.</span></span> 
  
```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Values/>
</ExtendedProperty>
```

 <span data-ttu-id="10de6-105">**ExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="10de6-105">**ExtendedPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="10de6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="10de6-106">Attributes and elements</span></span>

<span data-ttu-id="10de6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="10de6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10de6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="10de6-108">Attributes</span></span>

<span data-ttu-id="10de6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="10de6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10de6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="10de6-110">Child elements</span></span>

|<span data-ttu-id="10de6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="10de6-111">**Element**</span></span>|<span data-ttu-id="10de6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="10de6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10de6-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="10de6-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="10de6-114">Identifie une propriété MAPI étendue pour obtenir, définir ou créer.</span><span class="sxs-lookup"><span data-stu-id="10de6-114">Identifies an extended MAPI property to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="10de6-115">Values</span><span class="sxs-lookup"><span data-stu-id="10de6-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="10de6-116">Contient une collection de valeurs de propriété MAPI étendue à valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="10de6-116">Contains a collection of values for a multivalued extended MAPI property.</span></span>  <br/> |
|[<span data-ttu-id="10de6-117">Valeur</span><span class="sxs-lookup"><span data-stu-id="10de6-117">Value</span></span>](value.md) <br/> |<span data-ttu-id="10de6-118">Contient la valeur de la propriété étendue de MAPI à valeur unique.</span><span class="sxs-lookup"><span data-stu-id="10de6-118">Contains the value of single-valued MAPI extended property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="10de6-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="10de6-119">Parent elements</span></span>

|<span data-ttu-id="10de6-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="10de6-120">**Element**</span></span>|<span data-ttu-id="10de6-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="10de6-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10de6-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="10de6-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="10de6-123">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="10de6-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="10de6-124">Contact</span><span class="sxs-lookup"><span data-stu-id="10de6-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="10de6-125">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="10de6-125">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="10de6-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="10de6-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="10de6-127">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="10de6-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="10de6-128">Élément</span><span class="sxs-lookup"><span data-stu-id="10de6-128">Item</span></span>](item.md) <br/> |<span data-ttu-id="10de6-129">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="10de6-129">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="10de6-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="10de6-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="10de6-131">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="10de6-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="10de6-132">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="10de6-132">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="10de6-133">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="10de6-133">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="10de6-134">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="10de6-134">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="10de6-135">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="10de6-135">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="10de6-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="10de6-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="10de6-137">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="10de6-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="10de6-138">Message</span><span class="sxs-lookup"><span data-stu-id="10de6-138">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="10de6-139">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="10de6-139">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="10de6-140">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="10de6-140">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="10de6-141">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="10de6-141">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="10de6-142">Tâche</span><span class="sxs-lookup"><span data-stu-id="10de6-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="10de6-143">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="10de6-143">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="10de6-144">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="10de6-144">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="10de6-145">Représente un dossier contenant principalement des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="10de6-145">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="10de6-146">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="10de6-146">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="10de6-147">Représente un dossier contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="10de6-147">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="10de6-148">Folder</span><span class="sxs-lookup"><span data-stu-id="10de6-148">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="10de6-149">Représente un dossier à créer, obtenir, recherchez, synchroniser ou mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="10de6-149">Represents a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="10de6-150">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="10de6-150">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="10de6-151">Représente un dossier de recherche qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="10de6-151">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="10de6-152">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="10de6-152">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="10de6-153">Représente un dossier de tâches qui se trouve dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="10de6-153">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="10de6-154">Remarques</span><span class="sxs-lookup"><span data-stu-id="10de6-154">Remarks</span></span>

<span data-ttu-id="10de6-155">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="10de6-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10de6-156">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="10de6-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10de6-157">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="10de6-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="10de6-158">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="10de6-158">Schema Name</span></span>  <br/> |<span data-ttu-id="10de6-159">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="10de6-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="10de6-160">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="10de6-160">Validation File</span></span>  <br/> |<span data-ttu-id="10de6-161">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="10de6-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="10de6-162">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="10de6-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="10de6-163">False</span><span class="sxs-lookup"><span data-stu-id="10de6-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10de6-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="10de6-164">See also</span></span>



- [<span data-ttu-id="10de6-165">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="10de6-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

