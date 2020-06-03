---
title: Catégories
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Categories
api_type:
- schema
ms.assetid: d84d4927-b524-4e62-bf3d-1f12fec8c21a
description: L’élément categories contient une collection de chaînes qui identifient les catégories auxquelles un élément de la boîte aux lettres appartient.
ms.openlocfilehash: 0d9f7068aa81306a10436ed0ca0d45f6d3b2c3a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462212"
---
# <a name="categories"></a><span data-ttu-id="ad202-103">Catégories</span><span class="sxs-lookup"><span data-stu-id="ad202-103">Categories</span></span>

<span data-ttu-id="ad202-104">L’élément **categories** contient une collection de chaînes qui identifient les catégories auxquelles un élément de la boîte aux lettres appartient.</span><span class="sxs-lookup"><span data-stu-id="ad202-104">The **Categories** element contains a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span> 
  
```XML
<Categories>
   <String/>
</Categories>
```

 <span data-ttu-id="ad202-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="ad202-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad202-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad202-106">Attributes and elements</span></span>

<span data-ttu-id="ad202-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad202-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad202-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad202-108">Attributes</span></span>

<span data-ttu-id="ad202-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ad202-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad202-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad202-110">Child elements</span></span>

|<span data-ttu-id="ad202-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad202-111">**Element**</span></span>|<span data-ttu-id="ad202-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad202-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad202-113">String</span><span class="sxs-lookup"><span data-stu-id="ad202-113">String</span></span>](string.md) <br/> |<span data-ttu-id="ad202-114">Contient une chaîne qui identifie une seule catégorie.</span><span class="sxs-lookup"><span data-stu-id="ad202-114">Contains a string that identifies a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad202-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad202-115">Parent elements</span></span>

|<span data-ttu-id="ad202-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad202-116">**Element**</span></span>|<span data-ttu-id="ad202-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad202-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad202-118">Élément</span><span class="sxs-lookup"><span data-stu-id="ad202-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="ad202-119">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad202-119">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ad202-120">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="ad202-120">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="ad202-121">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad202-121">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ad202-122">Message</span><span class="sxs-lookup"><span data-stu-id="ad202-122">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ad202-123">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad202-123">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="ad202-124">Tâche</span><span class="sxs-lookup"><span data-stu-id="ad202-124">Task</span></span>](task.md) <br/> |<span data-ttu-id="ad202-125">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad202-125">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ad202-126">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ad202-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ad202-127">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad202-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ad202-128">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="ad202-128">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="ad202-129">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="ad202-129">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="ad202-130">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ad202-130">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="ad202-131">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad202-131">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ad202-132">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="ad202-132">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ad202-133">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad202-133">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ad202-134">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="ad202-134">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="ad202-135">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad202-135">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ad202-136">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="ad202-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="ad202-137">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad202-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ad202-138">Contact</span><span class="sxs-lookup"><span data-stu-id="ad202-138">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="ad202-139">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad202-139">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="ad202-140">DistributionList</span><span class="sxs-lookup"><span data-stu-id="ad202-140">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="ad202-141">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="ad202-141">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="ad202-142">Conditions</span><span class="sxs-lookup"><span data-stu-id="ad202-142">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="ad202-143">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="ad202-143">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="ad202-144">Exceptions</span><span class="sxs-lookup"><span data-stu-id="ad202-144">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="ad202-145">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="ad202-145">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="ad202-146">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="ad202-146">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="ad202-147">Contient une seule action à appliquer à une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="ad202-147">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad202-148">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ad202-148">Text value</span></span>

<span data-ttu-id="ad202-149">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ad202-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ad202-150">Remarques</span><span class="sxs-lookup"><span data-stu-id="ad202-150">Remarks</span></span>

<span data-ttu-id="ad202-151">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad202-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad202-152">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad202-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad202-153">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad202-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad202-154">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad202-154">Schema Name</span></span>  <br/> |<span data-ttu-id="ad202-155">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ad202-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad202-156">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ad202-156">Validation File</span></span>  <br/> |<span data-ttu-id="ad202-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ad202-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad202-158">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad202-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad202-159">False</span><span class="sxs-lookup"><span data-stu-id="ad202-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad202-160">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad202-160">See also</span></span>



- [<span data-ttu-id="ad202-161">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ad202-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

