---
title: AppendToItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppendToItemField
api_type:
- schema
ms.assetid: 66dbcb4a-ae6d-4648-8610-67187bdb105c
description: L’élément AppendToItemField identifie les données à ajouter à une propriété d’un élément pendant une opération UpdateItem.
ms.openlocfilehash: b432399e84ee4a3fd7edc5d3f803079435c79143
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755222"
---
# <a name="appendtoitemfield"></a><span data-ttu-id="ce346-103">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ce346-103">AppendToItemField</span></span>

<span data-ttu-id="ce346-104">L’élément **AppendToItemField** identifie les données à ajouter à une propriété d’un élément pendant une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ce346-104">The **AppendToItemField** element identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>
  
- [<span data-ttu-id="ce346-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ce346-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="ce346-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="ce346-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="ce346-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ce346-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="ce346-108">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="ce346-108">Updates (Item)</span></span>](updates-item.md)
  
- [<span data-ttu-id="ce346-109">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ce346-109">AppendToItemField</span></span>](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 <span data-ttu-id="ce346-110">**AppendToItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="ce346-110">**AppendToItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce346-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ce346-111">Attributes and elements</span></span>

<span data-ttu-id="ce346-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ce346-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce346-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="ce346-113">Attributes</span></span>

<span data-ttu-id="ce346-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ce346-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce346-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ce346-115">Child elements</span></span>

|<span data-ttu-id="ce346-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ce346-116">**Element**</span></span>|<span data-ttu-id="ce346-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ce346-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce346-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ce346-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="ce346-119">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="ce346-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="ce346-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ce346-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="ce346-121">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="ce346-121">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="ce346-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ce346-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="ce346-123">Identifie les propriétés MAPI étendues à ajouter.</span><span class="sxs-lookup"><span data-stu-id="ce346-123">Identifies extended MAPI properties to append.</span></span>  <br/> |
|[<span data-ttu-id="ce346-124">Élément</span><span class="sxs-lookup"><span data-stu-id="ce346-124">Item</span></span>](item.md) <br/> |<span data-ttu-id="ce346-125">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce346-125">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce346-126">Message</span><span class="sxs-lookup"><span data-stu-id="ce346-126">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ce346-127">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce346-127">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="ce346-128">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ce346-128">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ce346-129">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce346-129">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ce346-130">Contact</span><span class="sxs-lookup"><span data-stu-id="ce346-130">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="ce346-131">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce346-131">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="ce346-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="ce346-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="ce346-133">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="ce346-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="ce346-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ce346-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="ce346-135">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce346-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce346-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="ce346-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="ce346-137">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce346-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce346-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ce346-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ce346-139">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce346-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce346-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="ce346-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="ce346-141">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce346-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ce346-142">Tâche</span><span class="sxs-lookup"><span data-stu-id="ce346-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="ce346-143">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce346-143">Represents a task in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce346-144">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ce346-144">Parent elements</span></span>

|<span data-ttu-id="ce346-145">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ce346-145">**Element**</span></span>|<span data-ttu-id="ce346-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="ce346-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce346-147">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="ce346-147">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="ce346-148">Contient un tableau qui définit append, définir et supprimer les modifications apportées aux propriétés de l’élément.</span><span class="sxs-lookup"><span data-stu-id="ce346-148">Contains an array that defines append, set, and delete changes to item properties.</span></span>  <br/> <span data-ttu-id="ce346-149">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="ce346-149">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ce346-150">Note</span><span class="sxs-lookup"><span data-stu-id="ce346-150">Remarks</span></span>

<span data-ttu-id="ce346-151">Opérations d’ajout sont uniquement certain prennent en charge les propriétés.</span><span class="sxs-lookup"><span data-stu-id="ce346-151">Only certain properties support append operations.</span></span> <span data-ttu-id="ce346-152">Une tentative d’ajouter à une propriété qui ne prend pas en charge l’ajout d’entraîne une erreur.</span><span class="sxs-lookup"><span data-stu-id="ce346-152">An attempt to append to a property that does not support appending will result in an error.</span></span>
  
<span data-ttu-id="ce346-153">Pour les opérations de mise à jour, une seule propriété peut être modifiée dans une demande unique.</span><span class="sxs-lookup"><span data-stu-id="ce346-153">For update operations, only one property can be modified within a single request.</span></span> <span data-ttu-id="ce346-154">Cette propriété doit être référencée dans l’élément de [chemin d’accès](path.md) .</span><span class="sxs-lookup"><span data-stu-id="ce346-154">That single property must be referenced in the [Path](path.md) element.</span></span> <span data-ttu-id="ce346-155">**L’élément dans les classes dérivées** peut contenir puis qu’une seule propriété qui est en accord avec l’élément de **chemin d’accès** unique.</span><span class="sxs-lookup"><span data-stu-id="ce346-155">The **Item** element in the derived classes can then only hold a single property that is in agreement with the single **Path** element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ce346-156">L’élément de [chemin d’accès](path.md) est abstraite.</span><span class="sxs-lookup"><span data-stu-id="ce346-156">The [Path](path.md) element is abstract.</span></span> <span data-ttu-id="ce346-157">Il doit être remplacé par l’élément [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="ce346-157">It must be substituted by the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="ce346-158">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ce346-158">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce346-159">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ce346-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce346-160">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ce346-160">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ce346-161">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ce346-161">Schema Name</span></span>  <br/> |<span data-ttu-id="ce346-162">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ce346-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="ce346-163">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ce346-163">Validation File</span></span>  <br/> |<span data-ttu-id="ce346-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ce346-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ce346-165">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ce346-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce346-166">False</span><span class="sxs-lookup"><span data-stu-id="ce346-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce346-167">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ce346-167">See also</span></span>

- [<span data-ttu-id="ce346-168">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="ce346-168">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="ce346-169">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ce346-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

