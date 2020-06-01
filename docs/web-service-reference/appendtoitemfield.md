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
description: L’élément AppendToItemField identifie les données à ajouter à une propriété unique d’un élément au cours d’une opération UpdateItem.
ms.openlocfilehash: 902239155bff45d6f81989de954c9459cf012288
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466044"
---
# <a name="appendtoitemfield"></a><span data-ttu-id="ba546-103">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ba546-103">AppendToItemField</span></span>

<span data-ttu-id="ba546-104">L’élément **AppendToItemField** identifie les données à ajouter à une propriété unique d’un élément au cours d’une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ba546-104">The **AppendToItemField** element identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>
  
- [<span data-ttu-id="ba546-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ba546-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="ba546-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="ba546-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="ba546-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ba546-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="ba546-108">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="ba546-108">Updates (Item)</span></span>](updates-item.md)
  
- [<span data-ttu-id="ba546-109">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ba546-109">AppendToItemField</span></span>](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 <span data-ttu-id="ba546-110">**AppendToItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="ba546-110">**AppendToItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba546-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ba546-111">Attributes and elements</span></span>

<span data-ttu-id="ba546-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ba546-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba546-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="ba546-113">Attributes</span></span>

<span data-ttu-id="ba546-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ba546-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba546-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ba546-115">Child elements</span></span>

|<span data-ttu-id="ba546-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ba546-116">**Element**</span></span>|<span data-ttu-id="ba546-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba546-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba546-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ba546-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="ba546-119">Identifie les propriétés référencées fréquemment par URI.</span><span class="sxs-lookup"><span data-stu-id="ba546-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="ba546-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ba546-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="ba546-121">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="ba546-121">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="ba546-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ba546-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="ba546-123">Identifie les propriétés MAPI étendues à ajouter.</span><span class="sxs-lookup"><span data-stu-id="ba546-123">Identifies extended MAPI properties to append.</span></span>  <br/> |
|[<span data-ttu-id="ba546-124">Élément</span><span class="sxs-lookup"><span data-stu-id="ba546-124">Item</span></span>](item.md) <br/> |<span data-ttu-id="ba546-125">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba546-125">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ba546-126">Message</span><span class="sxs-lookup"><span data-stu-id="ba546-126">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ba546-127">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba546-127">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="ba546-128">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ba546-128">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ba546-129">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba546-129">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ba546-130">Contact</span><span class="sxs-lookup"><span data-stu-id="ba546-130">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="ba546-131">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba546-131">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="ba546-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="ba546-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="ba546-133">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="ba546-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="ba546-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ba546-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="ba546-135">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba546-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ba546-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="ba546-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="ba546-137">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba546-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ba546-138">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="ba546-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ba546-139">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba546-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ba546-140">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="ba546-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="ba546-141">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba546-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ba546-142">Tâche</span><span class="sxs-lookup"><span data-stu-id="ba546-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="ba546-143">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ba546-143">Represents a task in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ba546-144">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ba546-144">Parent elements</span></span>

|<span data-ttu-id="ba546-145">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ba546-145">**Element**</span></span>|<span data-ttu-id="ba546-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba546-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba546-147">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="ba546-147">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="ba546-148">Contient un tableau qui définit les modifications d’ajout, de définition et de suppression des propriétés d’élément.</span><span class="sxs-lookup"><span data-stu-id="ba546-148">Contains an array that defines append, set, and delete changes to item properties.</span></span>  <br/> <span data-ttu-id="ba546-149">Voici l’expression XPath de cet élément :`/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="ba546-149">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ba546-150">Remarques</span><span class="sxs-lookup"><span data-stu-id="ba546-150">Remarks</span></span>

<span data-ttu-id="ba546-151">Seules certaines propriétés prennent en charge les opérations Append.</span><span class="sxs-lookup"><span data-stu-id="ba546-151">Only certain properties support append operations.</span></span> <span data-ttu-id="ba546-152">Une tentative d’ajout à une propriété qui ne prend pas en charge l’ajout entraînera une erreur.</span><span class="sxs-lookup"><span data-stu-id="ba546-152">An attempt to append to a property that does not support appending will result in an error.</span></span>
  
<span data-ttu-id="ba546-153">Pour les opérations de mise à jour, une seule propriété peut être modifiée dans une seule demande.</span><span class="sxs-lookup"><span data-stu-id="ba546-153">For update operations, only one property can be modified within a single request.</span></span> <span data-ttu-id="ba546-154">Cette propriété unique doit être référencée dans l’élément [path](path.md) .</span><span class="sxs-lookup"><span data-stu-id="ba546-154">That single property must be referenced in the [Path](path.md) element.</span></span> <span data-ttu-id="ba546-155">L’élément **Item** dans les classes dérivées ne peut ensuite contenir qu’une seule propriété qui est en accord avec l’élément **path** unique.</span><span class="sxs-lookup"><span data-stu-id="ba546-155">The **Item** element in the derived classes can then only hold a single property that is in agreement with the single **Path** element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ba546-156">L’élément [path](path.md) est abstrait.</span><span class="sxs-lookup"><span data-stu-id="ba546-156">The [Path](path.md) element is abstract.</span></span> <span data-ttu-id="ba546-157">Elle doit être remplacée par l’élément [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)ou [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="ba546-157">It must be substituted by the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="ba546-158">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ba546-158">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba546-159">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ba546-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba546-160">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ba546-160">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba546-161">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ba546-161">Schema Name</span></span>  <br/> |<span data-ttu-id="ba546-162">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ba546-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba546-163">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ba546-163">Validation File</span></span>  <br/> |<span data-ttu-id="ba546-164">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ba546-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba546-165">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ba546-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba546-166">False</span><span class="sxs-lookup"><span data-stu-id="ba546-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba546-167">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ba546-167">See also</span></span>

- [<span data-ttu-id="ba546-168">Opération UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ba546-168">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="ba546-169">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ba546-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

