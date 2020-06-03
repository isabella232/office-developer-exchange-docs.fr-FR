---
title: ConversationId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationId
api_type:
- schema
ms.assetid: d5f1ddb3-9af3-4677-a6ba-111b304a951e
description: L’élément ConversationId contient l’identificateur d’un élément ou d’une conversation.
ms.openlocfilehash: 4f12d70ae6b72773760a731f5778cf6743ce699f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461470"
---
# <a name="conversationid"></a><span data-ttu-id="66e2b-103">ConversationId</span><span class="sxs-lookup"><span data-stu-id="66e2b-103">ConversationId</span></span>

<span data-ttu-id="66e2b-104">L’élément **ConversationId** contient l’identificateur d’un élément ou d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="66e2b-104">The **ConversationId** element contains the identifier of an item or conversation.</span></span> 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 <span data-ttu-id="66e2b-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="66e2b-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66e2b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="66e2b-106">Attributes and elements</span></span>

<span data-ttu-id="66e2b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="66e2b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66e2b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="66e2b-108">Attributes</span></span>

|<span data-ttu-id="66e2b-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="66e2b-109">**Attribute**</span></span>|<span data-ttu-id="66e2b-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="66e2b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="66e2b-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="66e2b-111">**Id**</span></span> <br/> |<span data-ttu-id="66e2b-112">Identifie un élément spécifique dans la Banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="66e2b-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="66e2b-113">**ChangeKey**</span></span> <br/> | <span data-ttu-id="66e2b-114">Identifie une version spécifique d’un élément.</span><span class="sxs-lookup"><span data-stu-id="66e2b-114">Identifies a specific version of an item.</span></span> <span data-ttu-id="66e2b-115">Un **ChangeKey** est requis pour les scénarios suivants :</span><span class="sxs-lookup"><span data-stu-id="66e2b-115">A **ChangeKey** is required for the following scenarios:</span></span>  <br/><br/><span data-ttu-id="66e2b-116">-L’élément [UpdateItem](updateitem.md) nécessite un **ChangeKey** si l’attribut **ConflictResolution** est défini sur autosolve.</span><span class="sxs-lookup"><span data-stu-id="66e2b-116">- The [UpdateItem](updateitem.md) element requires a **ChangeKey** if the **ConflictResolution** attribute is set to AutoResolve.</span></span> <span data-ttu-id="66e2b-117">Autosolve est une valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="66e2b-117">AutoResolve is a default value.</span></span> <span data-ttu-id="66e2b-118">Si l’attribut **ChangeKey** n’est pas inclus, la réponse renvoie une valeur [ResponseCode](responsecode.md) égale à **ErrorChangeKeyRequired**.</span><span class="sxs-lookup"><span data-stu-id="66e2b-118">If the **ChangeKey** attribute is not included, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorChangeKeyRequired**.</span></span><br/><br/><span data-ttu-id="66e2b-119">- Les éléments [SendItem](senditem.md), [DeleteItem](deleteitem.md)et [DeleteFolder](deletefolder.md) requièrent un **ChangeKey** pour tester si l’opération tentée agira sur la version la plus récente d’un élément.</span><span class="sxs-lookup"><span data-stu-id="66e2b-119">- [SendItem](senditem.md), [DeleteItem](deleteitem.md), and [DeleteFolder](deletefolder.md) elements require a **ChangeKey** to test whether the attempted operation will act upon the most recent version of an item.</span></span> <span data-ttu-id="66e2b-120">Si l’attribut **ChangeKey** n’est pas inclus dans l' **ItemId** ou si **ChangeKey** est vide, la réponse renvoie une valeur [ResponseCode](responsecode.md) égale à **ErrorStaleObject**.</span><span class="sxs-lookup"><span data-stu-id="66e2b-120">If the **ChangeKey** attribute is not included in the **ItemId** or if the **ChangeKey** is empty, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorStaleObject**.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="66e2b-121">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="66e2b-121">Child elements</span></span>

<span data-ttu-id="66e2b-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="66e2b-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="66e2b-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="66e2b-123">Parent elements</span></span>

|<span data-ttu-id="66e2b-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="66e2b-124">**Element**</span></span>|<span data-ttu-id="66e2b-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="66e2b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66e2b-126">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="66e2b-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="66e2b-127">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-128">Contact</span><span class="sxs-lookup"><span data-stu-id="66e2b-128">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="66e2b-129">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-129">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-130">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="66e2b-130">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="66e2b-131">Représente une action unique à appliquer à une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="66e2b-131">Represents a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="66e2b-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="66e2b-133">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="66e2b-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-134">Élément</span><span class="sxs-lookup"><span data-stu-id="66e2b-134">Item</span></span>](item.md) <br/> |<span data-ttu-id="66e2b-135">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-135">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-136">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="66e2b-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="66e2b-137">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-138">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="66e2b-138">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="66e2b-139">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-139">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-140">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="66e2b-140">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="66e2b-141">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-141">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-142">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="66e2b-142">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="66e2b-143">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-143">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-144">Message</span><span class="sxs-lookup"><span data-stu-id="66e2b-144">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="66e2b-145">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-145">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-146">PostItem</span><span class="sxs-lookup"><span data-stu-id="66e2b-146">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="66e2b-147">Représente un élément post dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-147">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-148">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="66e2b-148">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="66e2b-149">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-149">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-150">Tâche</span><span class="sxs-lookup"><span data-stu-id="66e2b-150">Task</span></span>](task.md) <br/> |<span data-ttu-id="66e2b-151">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-151">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="66e2b-152">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="66e2b-152">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="66e2b-153">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="66e2b-153">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="66e2b-154">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="66e2b-154">Text value</span></span>

<span data-ttu-id="66e2b-155">Aucun.</span><span class="sxs-lookup"><span data-stu-id="66e2b-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="66e2b-156">Remarques</span><span class="sxs-lookup"><span data-stu-id="66e2b-156">Remarks</span></span>

<span data-ttu-id="66e2b-157">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="66e2b-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66e2b-158">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="66e2b-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66e2b-159">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="66e2b-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="66e2b-160">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="66e2b-160">Schema Name</span></span>  <br/> |<span data-ttu-id="66e2b-161">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="66e2b-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="66e2b-162">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="66e2b-162">Validation File</span></span>  <br/> |<span data-ttu-id="66e2b-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="66e2b-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="66e2b-164">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="66e2b-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="66e2b-165">False</span><span class="sxs-lookup"><span data-stu-id="66e2b-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66e2b-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="66e2b-166">See also</span></span>

- [<span data-ttu-id="66e2b-167">Opération FindConversation</span><span class="sxs-lookup"><span data-stu-id="66e2b-167">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="66e2b-168">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="66e2b-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

