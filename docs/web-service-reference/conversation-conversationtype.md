---
title: Conversation (ConversationType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversation
api_type:
- schema
ms.assetid: 59d014cd-5886-49ea-8d36-ba5de7e675de
description: L’élément conversation représente une seule conversation.
ms.openlocfilehash: 9969a6cfe1f977b1c24e03771f231f4eb03d1ac6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458935"
---
# <a name="conversation-conversationtype"></a><span data-ttu-id="2d2d4-103">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2d2d4-103">Conversation (ConversationType)</span></span>

<span data-ttu-id="2d2d4-104">L’élément **conversation** représente une seule conversation.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-104">The **Conversation** element represents a single conversation.</span></span> 
  
[<span data-ttu-id="2d2d4-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="2d2d4-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="2d2d4-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="2d2d4-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="2d2d4-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2d2d4-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
```XML
<Conversation>
   <ConversationId/>
   <ConversationTopic/>
   <UniqueRecipients/>
   <GlobalUniqueRecipients/>
   <UniqueUnreadSenders/>
   <GlobalUniqueUnreadSenders/>
   <UniqueSenders/>
   <GlobalUniqueSenders/>
   <LastDeliveryTime/>
   <GlobalLastDeliveryTime/>
   <Categories/>
   <GlobalCategories/>
   <FlagStatus/>
   <GlobalFlagStatus/>
   <HasAttachments/>
   <GlobalHasAttachments/>
   <MessageCount/>
   <GlobalMessageCount/>
   <UnreadCount/>
   <GlobalUnreadCount/>
   <Size/>   <GlobalSize/>
   <ItemClasses/>
   <GlobalItemClasses/>
   <Importance/>
   <GlobalImportance/>
   <ItemIds/>
   <GlobalItemIds/>
</Conversation>
```

 <span data-ttu-id="2d2d4-108">**ConversationType**</span><span class="sxs-lookup"><span data-stu-id="2d2d4-108">**ConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d2d4-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2d2d4-109">Attributes and elements</span></span>

<span data-ttu-id="2d2d4-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d2d4-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="2d2d4-111">Attributes</span></span>

<span data-ttu-id="2d2d4-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d2d4-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2d2d4-113">Child elements</span></span>

|<span data-ttu-id="2d2d4-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2d2d4-114">**Element**</span></span>|<span data-ttu-id="2d2d4-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="2d2d4-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d2d4-116">ConversationId</span><span class="sxs-lookup"><span data-stu-id="2d2d4-116">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="2d2d4-117">Représente l’identificateur d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-117">Represents the identifier of a conversation.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-118">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="2d2d4-118">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="2d2d4-119">Représente la rubrique de conversation.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-119">Represents the conversation topic.</span></span> <span data-ttu-id="2d2d4-120">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-120">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-121">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="2d2d4-121">UniqueRecipients</span></span>](uniquerecipients.md) <br/> |<span data-ttu-id="2d2d4-122">Contient la liste des destinataires d’une conversation qui a été regroupée à partir d’un dossier particulier.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-122">Contains the recipient list of a conversation aggregated from a particular folder.</span></span> <span data-ttu-id="2d2d4-123">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-123">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-124">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="2d2d4-124">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md) <br/> |<span data-ttu-id="2d2d4-125">Contient la liste des destinataires d’une conversation qui est agrégée dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-125">Contains the recipient list of a conversation aggregated across a mailbox.</span></span> <span data-ttu-id="2d2d4-126">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-126">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-127">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="2d2d4-127">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md) <br/> |<span data-ttu-id="2d2d4-128">Contient une liste de toutes les personnes qui ont envoyé des messages non lus dans cette conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-128">Contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="2d2d4-129">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-129">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-130">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="2d2d4-130">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md) <br/> |<span data-ttu-id="2d2d4-131">Contient une liste de toutes les personnes qui ont envoyé des messages non lus dans cette conversation sur tous les dossiers de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-131">Contains a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-132">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="2d2d4-132">UniqueSenders</span></span>](uniquesenders.md) <br/> |<span data-ttu-id="2d2d4-133">Contient une liste de tous les expéditeurs d’éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-133">Contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="2d2d4-134">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-134">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-135">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="2d2d4-135">GlobalUniqueSenders</span></span>](globaluniquesenders.md) <br/> |<span data-ttu-id="2d2d4-136">Contient une liste de tous les expéditeurs d’éléments de conversation dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-136">Contains a list of all the senders of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-137">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="2d2d4-137">LastDeliveryTime</span></span>](lastdeliverytime.md) <br/> |<span data-ttu-id="2d2d4-138">Contient le délai de remise du message qui a été reçu en dernier dans cette conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-138">Contains the delivery time of the message that was last received in this conversation in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-139">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="2d2d4-139">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md) <br/> |<span data-ttu-id="2d2d4-140">Contient le délai de remise du message qui a été reçu en dernier dans cette conversation sur tous les dossiers de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-140">Contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-141">Catégories</span><span class="sxs-lookup"><span data-stu-id="2d2d4-141">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2d2d4-142">Contient une collection de chaînes qui identifient les catégories qui sont appliquées à tous les éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-142">Contains a collection of strings that identify the categories that are applied to all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-143">GlobalCategories</span><span class="sxs-lookup"><span data-stu-id="2d2d4-143">GlobalCategories</span></span>](globalcategories.md) <br/> |<span data-ttu-id="2d2d4-144">Contient la liste des catégories pour tous les éléments de conversation d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-144">Contains the category list for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-145">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="2d2d4-145">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="2d2d4-146">Contient l’état de l’indicateur agrégé pour les éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-146">Contains the aggregated flag status for conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-147">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="2d2d4-147">GlobalFlagStatus</span></span>](globalflagstatus.md) <br/> |<span data-ttu-id="2d2d4-148">Contient l’état de l’indicateur agrégé pour tous les éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-148">Contains the aggregated flag status for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-149">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="2d2d4-149">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="2d2d4-150">Contient une valeur qui indique si au moins un élément de conversation dans le dossier actif a une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-150">Contains a value that indicates whether at least one conversation item in the current folder has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-151">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="2d2d4-151">GlobalHasAttachments</span></span>](globalhasattachments.md) <br/> |<span data-ttu-id="2d2d4-152">Contient une valeur qui indique si au moins un élément de conversation dans une boîte aux lettres a une pièce jointe.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-152">Contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-153">MessageCount</span><span class="sxs-lookup"><span data-stu-id="2d2d4-153">MessageCount</span></span>](messagecount.md) <br/> |<span data-ttu-id="2d2d4-154">Contient le nombre total d’éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-154">Contains the total number of conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-155">GlobalMessageCount</span><span class="sxs-lookup"><span data-stu-id="2d2d4-155">GlobalMessageCount</span></span>](globalmessagecount.md) <br/> |<span data-ttu-id="2d2d4-156">Contient le nombre total d’éléments de conversation dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-156">Contains the total number of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="2d2d4-157">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="2d2d4-158">Contient le nombre d’éléments de conversation non lus dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-158">Contains the count of unread conversation items within a folder.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-159">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="2d2d4-159">GlobalUnreadCount</span></span>](globalunreadcount.md) <br/> |<span data-ttu-id="2d2d4-160">Contient le décompte de tous les éléments de conversation non lus dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-160">Contains a count of all the unread conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-161">Taille</span><span class="sxs-lookup"><span data-stu-id="2d2d4-161">Size</span></span>](size.md) <br/> |<span data-ttu-id="2d2d4-162">Contient la taille de la conversation calculée à partir de la taille de tous les éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-162">Contains the conversation size calculated from the size of all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-163">GlobalSize</span><span class="sxs-lookup"><span data-stu-id="2d2d4-163">GlobalSize</span></span>](globalsize.md) <br/> |<span data-ttu-id="2d2d4-164">Contient la taille de la conversation calculée à partir de la taille de tous les éléments de conversation dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-164">Contains the size of the conversation calculated from the size of all conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-165">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="2d2d4-165">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md) <br/> |<span data-ttu-id="2d2d4-166">Contient une liste de classes d’éléments qui représente toutes les classes d’éléments des éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-166">Contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-167">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="2d2d4-167">GlobalItemClasses</span></span>](globalitemclasses.md) <br/> |<span data-ttu-id="2d2d4-168">Contient une liste de classes d’éléments qui représente toutes les classes d’éléments des éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-168">Contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-169">Importance</span><span class="sxs-lookup"><span data-stu-id="2d2d4-169">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="2d2d4-170">Contient l’importance regroupée pour tous les éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-170">Contains the aggregated importance for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-171">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="2d2d4-171">GlobalImportance</span></span>](globalimportance.md) <br/> |<span data-ttu-id="2d2d4-172">Contient l’importance regroupée pour tous les éléments de conversation d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-172">Contains the aggregated importance for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-173">ItemIds</span><span class="sxs-lookup"><span data-stu-id="2d2d4-173">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="2d2d4-174">Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-174">Contains the collection of item identifiers for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="2d2d4-175">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="2d2d4-175">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="2d2d4-176">Contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-176">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d2d4-177">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2d2d4-177">Parent elements</span></span>

|<span data-ttu-id="2d2d4-178">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2d2d4-178">**Element**</span></span>|<span data-ttu-id="2d2d4-179">**Description**</span><span class="sxs-lookup"><span data-stu-id="2d2d4-179">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d2d4-180">Conversations</span><span class="sxs-lookup"><span data-stu-id="2d2d4-180">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2d2d4-181">Contient un tableau des conversations qui sont renvoyées dans la réponse **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="2d2d4-181">Contains an array of conversations that are returned in the **FindConversation** response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2d2d4-182">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="2d2d4-182">Text value</span></span>

<span data-ttu-id="2d2d4-183">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2d2d4-183">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2d2d4-184">Remarques</span><span class="sxs-lookup"><span data-stu-id="2d2d4-184">Remarks</span></span>

<span data-ttu-id="2d2d4-185">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2d2d4-185">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d2d4-186">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2d2d4-186">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d2d4-187">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2d2d4-187">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d2d4-188">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2d2d4-188">Schema name</span></span>  <br/> |<span data-ttu-id="2d2d4-189">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2d2d4-189">Types schema</span></span>  <br/> |
|<span data-ttu-id="2d2d4-190">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2d2d4-190">Validation file</span></span>  <br/> |<span data-ttu-id="2d2d4-191">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2d2d4-191">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d2d4-192">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2d2d4-192">Can be empty</span></span>  <br/> |<span data-ttu-id="2d2d4-193">False</span><span class="sxs-lookup"><span data-stu-id="2d2d4-193">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d2d4-194">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2d2d4-194">See also</span></span>



[<span data-ttu-id="2d2d4-195">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="2d2d4-195">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="2d2d4-196">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="2d2d4-196">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="2d2d4-197">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="2d2d4-197">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

