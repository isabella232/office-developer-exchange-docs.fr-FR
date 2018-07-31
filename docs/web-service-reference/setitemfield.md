---
title: SetItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetItemField
api_type:
- schema
ms.assetid: 85284fcb-bd1e-4fda-9dab-cb4cd637cd5b
description: L’élément SetItemField représente une mise à jour d’une propriété unique d’un élément dans une opération UpdateItem.
ms.openlocfilehash: bd3e5bca3d61325ef3f218c5ada535346247f391
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353797"
---
# <a name="setitemfield"></a><span data-ttu-id="24f0b-103">SetItemField</span><span class="sxs-lookup"><span data-stu-id="24f0b-103">SetItemField</span></span>

<span data-ttu-id="24f0b-104">L’élément **SetItemField** représente une mise à jour d’une propriété unique d’un élément dans une [opération UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="24f0b-104">The **SetItemField** element represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>
  
```xml
<SetItemField>
   <FieldURI/>
   <Item/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Item/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingRequest/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingResponse/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <Contact/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <DistributionList/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingResponse/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingResponse/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingRequest/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <Contact/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <Message/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <CalendarItem/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Task/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Message/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingCancellation/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <Task/> 
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingRequest/>  
</SetItemField>
```

```xml
<SetItemField>
    <FieldURI/> 
    <CalendarItem/>
</SetItemField>
```

```xml
<SetItemField>
    <IndexedFieldURI/> 
    <Item/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingCancellation/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <DistributionList/> 
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingCancellation/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingMessage/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <Task/> 
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <CalendarItem/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingMessage/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingMessage/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <Message/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <DistributionList/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Contact/> 
</SetItemField>
```


<span data-ttu-id="24f0b-105">**SetItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="24f0b-105">**SetItemFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="24f0b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="24f0b-106">Attributes and elements</span></span>

<span data-ttu-id="24f0b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="24f0b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24f0b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="24f0b-108">Attributes</span></span>

<span data-ttu-id="24f0b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="24f0b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24f0b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="24f0b-110">Child elements</span></span>

|<span data-ttu-id="24f0b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="24f0b-111">**Element**</span></span>|<span data-ttu-id="24f0b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="24f0b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24f0b-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="24f0b-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="24f0b-114">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="24f0b-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="24f0b-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="24f0b-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="24f0b-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="24f0b-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="24f0b-118">Identifie les propriétés MAPI étendues à définir.</span><span class="sxs-lookup"><span data-stu-id="24f0b-118">Identifies extended MAPI properties to set.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-119">Élément</span><span class="sxs-lookup"><span data-stu-id="24f0b-119">Item</span></span>](item.md) <br/> |<span data-ttu-id="24f0b-120">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="24f0b-120">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-121">Message</span><span class="sxs-lookup"><span data-stu-id="24f0b-121">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="24f0b-122">Représente un message électronique d’Exchange pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="24f0b-122">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-123">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="24f0b-123">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="24f0b-124">Représente un élément de calendrier Exchange pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="24f0b-124">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-125">Contact</span><span class="sxs-lookup"><span data-stu-id="24f0b-125">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="24f0b-126">Représente un élément de contact Exchange pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="24f0b-126">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-127">DistributionList</span><span class="sxs-lookup"><span data-stu-id="24f0b-127">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="24f0b-128">Représente une liste de distribution pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="24f0b-128">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-129">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="24f0b-129">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="24f0b-130">Représente un message de réunion pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="24f0b-130">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-131">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="24f0b-131">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="24f0b-132">Représente une demande de réunion pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="24f0b-132">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-133">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="24f0b-133">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="24f0b-134">Représente une réponse à une réunion à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="24f0b-134">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-135">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="24f0b-135">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="24f0b-136">Représente une annulation de réunion pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="24f0b-136">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="24f0b-137">Tâche</span><span class="sxs-lookup"><span data-stu-id="24f0b-137">Task</span></span>](task.md) <br/> |<span data-ttu-id="24f0b-138">Représente une tâche à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="24f0b-138">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24f0b-139">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="24f0b-139">Parent elements</span></span>

|<span data-ttu-id="24f0b-140">**Élément**</span><span class="sxs-lookup"><span data-stu-id="24f0b-140">**Element**</span></span>|<span data-ttu-id="24f0b-141">**Description**</span><span class="sxs-lookup"><span data-stu-id="24f0b-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24f0b-142">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="24f0b-142">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="24f0b-143">Contient un ensemble d’éléments qui définissent append, définir et supprimer les modifications apportées aux propriétés de l’élément.</span><span class="sxs-lookup"><span data-stu-id="24f0b-143">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="24f0b-144">Remarques</span><span class="sxs-lookup"><span data-stu-id="24f0b-144">Remarks</span></span>

<span data-ttu-id="24f0b-145">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="24f0b-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24f0b-146">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="24f0b-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24f0b-147">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="24f0b-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="24f0b-148">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="24f0b-148">Schema Name</span></span>  <br/> |<span data-ttu-id="24f0b-149">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="24f0b-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="24f0b-150">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="24f0b-150">Validation File</span></span>  <br/> |<span data-ttu-id="24f0b-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="24f0b-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="24f0b-152">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="24f0b-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="24f0b-153">False</span><span class="sxs-lookup"><span data-stu-id="24f0b-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24f0b-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="24f0b-154">See also</span></span>

- [<span data-ttu-id="24f0b-155">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="24f0b-155">UpdateItem operation</span></span>](updateitem-operation.md)

