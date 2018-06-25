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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755222"
---
# <a name="appendtoitemfield"></a><span data-ttu-id="bcf55-103">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="bcf55-103">AppendToItemField</span></span>

<span data-ttu-id="bcf55-104">L’élément **AppendToItemField** identifie les données à ajouter à une propriété d’un élément pendant une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="bcf55-104">The **AppendToItemField** element identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>
  
- [<span data-ttu-id="bcf55-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="bcf55-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="bcf55-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="bcf55-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="bcf55-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="bcf55-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="bcf55-108">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="bcf55-108">Updates (Item)</span></span>](updates-item.md)
  
- [<span data-ttu-id="bcf55-109">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="bcf55-109">AppendToItemField</span></span>](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 <span data-ttu-id="bcf55-110">**AppendToItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="bcf55-110">**AppendToItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bcf55-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bcf55-111">Attributes and elements</span></span>

<span data-ttu-id="bcf55-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bcf55-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bcf55-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="bcf55-113">Attributes</span></span>

<span data-ttu-id="bcf55-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bcf55-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bcf55-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bcf55-115">Child elements</span></span>

|<span data-ttu-id="bcf55-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bcf55-116">**Element**</span></span>|<span data-ttu-id="bcf55-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="bcf55-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcf55-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="bcf55-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="bcf55-119">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="bcf55-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="bcf55-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="bcf55-121">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="bcf55-121">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="bcf55-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="bcf55-123">Identifie les propriétés MAPI étendues à ajouter.</span><span class="sxs-lookup"><span data-stu-id="bcf55-123">Identifies extended MAPI properties to append.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-124">Élément</span><span class="sxs-lookup"><span data-stu-id="bcf55-124">Item</span></span>](item.md) <br/> |<span data-ttu-id="bcf55-125">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcf55-125">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-126">Message</span><span class="sxs-lookup"><span data-stu-id="bcf55-126">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bcf55-127">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcf55-127">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-128">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="bcf55-128">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="bcf55-129">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcf55-129">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-130">Contact</span><span class="sxs-lookup"><span data-stu-id="bcf55-130">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="bcf55-131">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcf55-131">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="bcf55-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="bcf55-133">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="bcf55-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="bcf55-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="bcf55-135">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcf55-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="bcf55-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="bcf55-137">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcf55-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="bcf55-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="bcf55-139">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcf55-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="bcf55-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="bcf55-141">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcf55-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="bcf55-142">Tâche</span><span class="sxs-lookup"><span data-stu-id="bcf55-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="bcf55-143">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcf55-143">Represents a task in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bcf55-144">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bcf55-144">Parent elements</span></span>

|<span data-ttu-id="bcf55-145">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bcf55-145">**Element**</span></span>|<span data-ttu-id="bcf55-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="bcf55-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcf55-147">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="bcf55-147">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="bcf55-148">Contient un tableau qui définit append, définir et supprimer les modifications apportées aux propriétés de l’élément.</span><span class="sxs-lookup"><span data-stu-id="bcf55-148">Contains an array that defines append, set, and delete changes to item properties.</span></span>  <br/> <span data-ttu-id="bcf55-149">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="bcf55-149">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bcf55-150">Remarques</span><span class="sxs-lookup"><span data-stu-id="bcf55-150">Remarks</span></span>

<span data-ttu-id="bcf55-151">Opérations d’ajout sont uniquement certain prennent en charge les propriétés.</span><span class="sxs-lookup"><span data-stu-id="bcf55-151">Only certain properties support append operations.</span></span> <span data-ttu-id="bcf55-152">Une tentative d’ajouter à une propriété qui ne prend pas en charge l’ajout d’entraîne une erreur.</span><span class="sxs-lookup"><span data-stu-id="bcf55-152">An attempt to append to a property that does not support appending will result in an error.</span></span>
  
<span data-ttu-id="bcf55-153">Pour les opérations de mise à jour, une seule propriété peut être modifiée dans une demande unique.</span><span class="sxs-lookup"><span data-stu-id="bcf55-153">For update operations, only one property can be modified within a single request.</span></span> <span data-ttu-id="bcf55-154">Cette propriété doit être référencée dans l’élément de [chemin d’accès](path.md) .</span><span class="sxs-lookup"><span data-stu-id="bcf55-154">That single property must be referenced in the [Path](path.md) element.</span></span> <span data-ttu-id="bcf55-155">**L’élément dans les classes dérivées** peut contenir puis qu’une seule propriété qui est en accord avec l’élément de **chemin d’accès** unique.</span><span class="sxs-lookup"><span data-stu-id="bcf55-155">The **Item** element in the derived classes can then only hold a single property that is in agreement with the single **Path** element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bcf55-156">L’élément de [chemin d’accès](path.md) est abstraite.</span><span class="sxs-lookup"><span data-stu-id="bcf55-156">The [Path](path.md) element is abstract.</span></span> <span data-ttu-id="bcf55-157">Il doit être remplacé par l’élément [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="bcf55-157">It must be substituted by the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="bcf55-158">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="bcf55-158">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bcf55-159">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bcf55-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bcf55-160">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bcf55-160">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bcf55-161">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bcf55-161">Schema Name</span></span>  <br/> |<span data-ttu-id="bcf55-162">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bcf55-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="bcf55-163">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bcf55-163">Validation File</span></span>  <br/> |<span data-ttu-id="bcf55-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bcf55-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bcf55-165">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bcf55-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="bcf55-166">False</span><span class="sxs-lookup"><span data-stu-id="bcf55-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bcf55-167">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bcf55-167">See also</span></span>

- [<span data-ttu-id="bcf55-168">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="bcf55-168">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="bcf55-169">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bcf55-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

