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
ms.openlocfilehash: 1f82e6ade60fb70db4a9f026fd72d9f11cc63821
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755640"
---
# <a name="conversationid"></a><span data-ttu-id="5cde8-103">ConversationId</span><span class="sxs-lookup"><span data-stu-id="5cde8-103">ConversationId</span></span>

<span data-ttu-id="5cde8-104">L’élément **ConversationId** contient l’identificateur d’un élément ou d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="5cde8-104">The **ConversationId** element contains the identifier of an item or conversation.</span></span> 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 <span data-ttu-id="5cde8-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="5cde8-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cde8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5cde8-106">Attributes and elements</span></span>

<span data-ttu-id="5cde8-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5cde8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cde8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5cde8-108">Attributes</span></span>

|<span data-ttu-id="5cde8-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="5cde8-109">**Attribute**</span></span>|<span data-ttu-id="5cde8-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="5cde8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5cde8-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="5cde8-111">**Id**</span></span> <br/> |<span data-ttu-id="5cde8-112">Identifie un élément spécifique dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="5cde8-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="5cde8-113">**ChangeKey**</span></span> <br/> | <span data-ttu-id="5cde8-114">Identifie une version spécifique d’un élément.</span><span class="sxs-lookup"><span data-stu-id="5cde8-114">Identifies a specific version of an item.</span></span> <span data-ttu-id="5cde8-115">Un **ChangeKey** est requis pour les scénarios suivants :</span><span class="sxs-lookup"><span data-stu-id="5cde8-115">A **ChangeKey** is required for the following scenarios:</span></span>  <br/><br/><span data-ttu-id="5cde8-116">-L’élément [UpdateItem](updateitem.md) requiert un **ChangeKey** si l’attribut **ConflictResolution** est défini sur résoudre automatiquement.</span><span class="sxs-lookup"><span data-stu-id="5cde8-116">- The [UpdateItem](updateitem.md) element requires a **ChangeKey** if the **ConflictResolution** attribute is set to AutoResolve.</span></span> <span data-ttu-id="5cde8-117">Résolution automatique est une valeur par défaut.</span><span class="sxs-lookup"><span data-stu-id="5cde8-117">AutoResolve is a default value.</span></span> <span data-ttu-id="5cde8-118">Si l’attribut **ChangeKey** n’est pas inclus, la réponse renvoie une valeur [ResponseCode](responsecode.md) égale à **ErrorChangeKeyRequired**.</span><span class="sxs-lookup"><span data-stu-id="5cde8-118">If the **ChangeKey** attribute is not included, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorChangeKeyRequired**.</span></span><br/><br/><span data-ttu-id="5cde8-119">- Éléments [SendItem](senditem.md), [DeleteItem](deleteitem.md)et [DeleteFolder](deletefolder.md) nécessitent un **ChangeKey** vérifier si l’opération s’agir de la version la plus récente d’un élément.</span><span class="sxs-lookup"><span data-stu-id="5cde8-119">- [SendItem](senditem.md), [DeleteItem](deleteitem.md), and [DeleteFolder](deletefolder.md) elements require a **ChangeKey** to test whether the attempted operation will act upon the most recent version of an item.</span></span> <span data-ttu-id="5cde8-120">Si l’attribut **ChangeKey** n’est pas inclus dans l' **ID d’élément** , ou si la **ChangeKey** est vide, la réponse renvoie une valeur [ResponseCode](responsecode.md) égale à **ErrorStaleObject**.</span><span class="sxs-lookup"><span data-stu-id="5cde8-120">If the **ChangeKey** attribute is not included in the **ItemId** or if the **ChangeKey** is empty, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorStaleObject**.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5cde8-121">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5cde8-121">Child elements</span></span>

<span data-ttu-id="5cde8-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5cde8-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5cde8-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5cde8-123">Parent elements</span></span>

|<span data-ttu-id="5cde8-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5cde8-124">**Element**</span></span>|<span data-ttu-id="5cde8-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="5cde8-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cde8-126">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="5cde8-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5cde8-127">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-128">Contact</span><span class="sxs-lookup"><span data-stu-id="5cde8-128">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="5cde8-129">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-129">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-130">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="5cde8-130">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="5cde8-131">Représente une seule action à appliquer à une même conversation.</span><span class="sxs-lookup"><span data-stu-id="5cde8-131">Represents a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="5cde8-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="5cde8-133">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="5cde8-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-134">Élément</span><span class="sxs-lookup"><span data-stu-id="5cde8-134">Item</span></span>](item.md) <br/> |<span data-ttu-id="5cde8-135">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-135">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-136">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="5cde8-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="5cde8-137">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-138">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="5cde8-138">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="5cde8-139">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-139">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-140">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5cde8-140">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5cde8-141">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-141">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-142">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="5cde8-142">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="5cde8-143">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-143">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-144">Message</span><span class="sxs-lookup"><span data-stu-id="5cde8-144">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5cde8-145">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-145">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-146">Objet postItem</span><span class="sxs-lookup"><span data-stu-id="5cde8-146">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="5cde8-147">Représente un élément de publication dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-147">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-148">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="5cde8-148">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="5cde8-149">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-149">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-150">Tâche</span><span class="sxs-lookup"><span data-stu-id="5cde8-150">Task</span></span>](task.md) <br/> |<span data-ttu-id="5cde8-151">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-151">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5cde8-152">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="5cde8-152">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="5cde8-153">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="5cde8-153">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5cde8-154">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5cde8-154">Text value</span></span>

<span data-ttu-id="5cde8-155">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5cde8-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5cde8-156">Remarques</span><span class="sxs-lookup"><span data-stu-id="5cde8-156">Remarks</span></span>

<span data-ttu-id="5cde8-157">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cde8-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cde8-158">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5cde8-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cde8-159">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5cde8-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5cde8-160">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5cde8-160">Schema Name</span></span>  <br/> |<span data-ttu-id="5cde8-161">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5cde8-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="5cde8-162">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5cde8-162">Validation File</span></span>  <br/> |<span data-ttu-id="5cde8-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5cde8-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5cde8-164">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5cde8-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="5cde8-165">False</span><span class="sxs-lookup"><span data-stu-id="5cde8-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5cde8-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5cde8-166">See also</span></span>

- [<span data-ttu-id="5cde8-167">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="5cde8-167">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="5cde8-168">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5cde8-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
