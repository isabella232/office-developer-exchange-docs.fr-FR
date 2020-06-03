---
title: Opération GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ae00a99-b37b-4194-829c-fe300db6ab99
description: Recherchez des informations sur l’opération GetConversationItems.
ms.openlocfilehash: ddeb5386e56653a32ca2e6d212518704cd0f0c58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457780"
---
# <a name="getconversationitems-operation"></a><span data-ttu-id="38b4c-103">Opération GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="38b4c-103">GetConversationItems operation</span></span>

<span data-ttu-id="38b4c-104">Recherchez des informations sur l’opération **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="38b4c-104">Find information about the **GetConversationItems** operation.</span></span> 
  
<span data-ttu-id="38b4c-105">L’opération **GetConversationItems** obtient un ou plusieurs ensembles d’éléments organisés dans les nœuds d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="38b4c-105">The **GetConversationItems** operation gets one or more sets of items that are organized in to nodes in a conversation.</span></span> 
  
<span data-ttu-id="38b4c-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="38b4c-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getconversationitems-operation"></a><span data-ttu-id="38b4c-107">Utilisation de l’opération GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="38b4c-107">Using the GetConversationItems operation</span></span>

<span data-ttu-id="38b4c-108">Vous pouvez utiliser l’opération **GetConversationItems** pour obtenir des éléments dans les conversations pour les boîtes aux lettres principale et d’archivage.</span><span class="sxs-lookup"><span data-stu-id="38b4c-108">You can use the **GetConversationItems** operation to get items in conversations for both primary and archive mailboxes.</span></span> 
  
### <a name="getconversationitems-operation-soap-headers"></a><span data-ttu-id="38b4c-109">En-têtes SOAP d’opération GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="38b4c-109">GetConversationItems operation SOAP headers</span></span>

<span data-ttu-id="38b4c-110">L’opération **GetConversationItems** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="38b4c-110">The **GetConversationItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="38b4c-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="38b4c-111">**Header name**</span></span>|<span data-ttu-id="38b4c-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="38b4c-112">**Element**</span></span>|<span data-ttu-id="38b4c-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="38b4c-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="38b4c-114">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="38b4c-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="38b4c-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="38b4c-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="38b4c-116">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="38b4c-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="38b4c-117">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="38b4c-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="38b4c-118">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="38b4c-118">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="38b4c-119">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="38b4c-119">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="38b4c-120">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="38b4c-120">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="38b4c-121">La valeur minimale de cet élément est **Exchange2013**.</span><span class="sxs-lookup"><span data-stu-id="38b4c-121">The minimum value for this element is **Exchange2013**.</span></span> <span data-ttu-id="38b4c-122">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="38b4c-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="38b4c-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="38b4c-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="38b4c-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="38b4c-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="38b4c-125">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="38b4c-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="38b4c-126">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="38b4c-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getconversationitems-operation-request-example-get-items-in-a-single-conversation"></a><span data-ttu-id="38b4c-127">Exemple de requête d’opération GetConversationItems : obtenir des éléments dans une conversation unique</span><span class="sxs-lookup"><span data-stu-id="38b4c-127">GetConversationItems operation request example: Get items in a single conversation</span></span>

<span data-ttu-id="38b4c-128">L’exemple suivant de demande d’opération **GetConversationItems** montre comment obtenir tous les éléments de conversation en une seule conversation, à l’exception des éléments situés dans les dossiers éléments supprimés et brouillons.</span><span class="sxs-lookup"><span data-stu-id="38b4c-128">The following example of a **GetConversationItems** operation request shows how to get all conversation items in a single conversation, with the exception of items located in the Deleted Items and Drafts folders.</span></span> <span data-ttu-id="38b4c-129">Chaque élément renvoyé dans la réponse contient un identificateur d’élément, un objet et l’heure à laquelle l’élément a été reçu dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38b4c-129">Each item returned in the response will contain an item identifier, a subject, and the time that the item was received in the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="38b4c-130">Tous les identificateurs d’élément et clés de modification de cet article ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="38b4c-130">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:GetConversationItems>
         <m:ItemShape>
            <t:BaseShape>IdOnly</t:BaseShape>
            <t:AdditionalProperties>
               <t:FieldURI FieldURI="item:Subject" />
               <t:FieldURI FieldURI="item:DateTimeReceived" />
            </t:AdditionalProperties>
         </m:ItemShape>
         <m:FoldersToIgnore>
            <t:DistinguishedFolderId Id="deleteditems" />
            <t:DistinguishedFolderId Id="drafts" />
         </m:FoldersToIgnore>
         <m:SortOrder>TreeOrderDescending</m:SortOrder>
         <m:Conversations>
            <t:Conversation>
               <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
            </t:Conversation>
         </m:Conversations>
      </m:GetConversationItems>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="38b4c-131">Cet exemple de requête **GetConversationItems** n’inclut pas les options suivantes :</span><span class="sxs-lookup"><span data-stu-id="38b4c-131">This example of a **GetConversationItems** request does not include the following options:</span></span> 
  
- <span data-ttu-id="38b4c-132">L’élément [MaxItemsToReturn](maxitemstoreturn.md) , qui définit le nombre maximal d’éléments à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="38b4c-132">The [MaxItemsToReturn](maxitemstoreturn.md) element, which sets the maximum number of items to return in the response.</span></span> 
    
- <span data-ttu-id="38b4c-133">L’élément [MailboxScope](mailboxscope.md) , qui définit l’étendue des boîtes aux lettres en indiquant si l’opération **GetConversationItems** doit être effectuée sur la boîte aux lettres principale, la boîte aux lettres d’archivage ou les deux boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38b4c-133">The [MailboxScope](mailboxscope.md) element, which sets the mailbox scope by indicating whether the **GetConversationItems** operation is to be performed on the primary mailbox, the archive mailbox, or both mailboxes.</span></span> 
    
- <span data-ttu-id="38b4c-134">L’élément [SyncState (base64Binary)](syncstate-base64binary.md) , qui définit l’état de la synchronisation pour obtenir uniquement les éléments de conversation qui sont nouveaux ou mis à jour dans la conversation.</span><span class="sxs-lookup"><span data-stu-id="38b4c-134">The [SyncState (base64Binary)](syncstate-base64binary.md) element, which sets the synchronization state to only get conversation items that are new or updated in the conversation.</span></span> <span data-ttu-id="38b4c-135">Cet élément est défini pour chaque conversation.</span><span class="sxs-lookup"><span data-stu-id="38b4c-135">This element is set for each conversation.</span></span> 
    
<span data-ttu-id="38b4c-136">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="38b4c-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="38b4c-137">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="38b4c-137">GetConversationItems</span></span>](getconversationitems.md)
    
- [<span data-ttu-id="38b4c-138">ItemShape</span><span class="sxs-lookup"><span data-stu-id="38b4c-138">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="38b4c-139">BaseShape</span><span class="sxs-lookup"><span data-stu-id="38b4c-139">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="38b4c-140">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="38b4c-140">AdditionalProperties</span></span>](additionalproperties.md)
    
- [<span data-ttu-id="38b4c-141">FieldURI</span><span class="sxs-lookup"><span data-stu-id="38b4c-141">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="38b4c-142">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="38b4c-142">FoldersToIgnore</span></span>](folderstoignore.md)
    
- [<span data-ttu-id="38b4c-143">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="38b4c-143">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="38b4c-144">OrdreTri (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="38b4c-144">SortOrder (ConversationNodeSortOrder)</span></span>](sortorder-conversationnodesortorder.md)
    
- [<span data-ttu-id="38b4c-145">Conversations</span><span class="sxs-lookup"><span data-stu-id="38b4c-145">Conversations</span></span>](conversations-ex15websvcsotherref.md)
    
- [<span data-ttu-id="38b4c-146">Conversation (ConversationRequestType)</span><span class="sxs-lookup"><span data-stu-id="38b4c-146">Conversation (ConversationRequestType)</span></span>](conversation-conversationrequesttype.md)
    
- [<span data-ttu-id="38b4c-147">ConversationId</span><span class="sxs-lookup"><span data-stu-id="38b4c-147">ConversationId</span></span>](conversationid.md)
    
## <a name="successful-getconversationitems-operation-response"></a><span data-ttu-id="38b4c-148">Réponse de l’opération GetConversationItems réussie</span><span class="sxs-lookup"><span data-stu-id="38b4c-148">Successful GetConversationItems operation response</span></span>

<span data-ttu-id="38b4c-149">L’exemple suivant montre une réponse réussie à une demande d’opération **GetConversationItems** pour obtenir des éléments dans une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="38b4c-149">The following example shows a successful response to a **GetConversationItems** operation request to get items in a single conversation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="545"
                           MinorBuildNumber="11"
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetConversationItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetConversationItemsResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Conversation>
                  <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
                  <t:SyncState>AQIAAABNVkUwAgIAAABhHqHUAwIAAABNVkUxBAIAAABhHqHfBAIAAABhHqHV</t:SyncState>
                  <t:ConversationNodes>
                     <t:ConversationNode>
                        <t:InternetMessageId>6a4838fa804045e09d40c1a39b9ea916@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTQrAABhHqHfAAA=" ChangeKey="CQAAABYAAACYAABhPpaq" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T18:42:27Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>2695d2b837954d68846b0c30491f5af1@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTExYjJkLTYxZDAt" ChangeKey="CQAAABQrAABhPpaP" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:38:26Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTFNVkUxAAA=" ChangeKey="CQAAABY4QrAABhPvYK" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkm4QrAABhHqHUAAA=" ChangeKey="CQAAABQrAABhPpaN" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:05Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:InternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkArAABNVkUwAAA=" ChangeKey="CQAAABm4QrAABhPvYJ" />
                              <t:Subject>Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:36:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                  </t:ConversationNodes>
               </m:Conversation>
            </m:GetConversationItemsResponseMessage>
         </m:ResponseMessages>
      </m:GetConversationItemsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="38b4c-150">Nous vous recommandons d’enregistrer le SyncState pour les demandes d’opération **GetConversationItems** suivantes.</span><span class="sxs-lookup"><span data-stu-id="38b4c-150">We recommend that you save the SyncState for subsequent **GetConversationItems** operation requests.</span></span> 
  
<span data-ttu-id="38b4c-151">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="38b4c-151">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="38b4c-152">GetConversationItemsResponse</span><span class="sxs-lookup"><span data-stu-id="38b4c-152">GetConversationItemsResponse</span></span>](getconversationitemsresponse.md)
    
- [<span data-ttu-id="38b4c-153">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="38b4c-153">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="38b4c-154">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="38b4c-154">GetConversationItemsResponseMessage</span></span>](getconversationitemsresponsemessage.md)
    
- [<span data-ttu-id="38b4c-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="38b4c-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="38b4c-156">Conversation (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="38b4c-156">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md)
    
- [<span data-ttu-id="38b4c-157">ConversationId</span><span class="sxs-lookup"><span data-stu-id="38b4c-157">ConversationId</span></span>](conversationid.md)
    
- [<span data-ttu-id="38b4c-158">SyncState (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="38b4c-158">SyncState (base64Binary)</span></span>](syncstate-base64binary.md)
    
- [<span data-ttu-id="38b4c-159">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="38b4c-159">ConversationNodes</span></span>](conversationnodes.md)
    
- [<span data-ttu-id="38b4c-160">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="38b4c-160">ConversationNode</span></span>](conversationnode.md)
    
- [<span data-ttu-id="38b4c-161">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="38b4c-161">InternetMessageId</span></span>](internetmessageid.md)
    
- [<span data-ttu-id="38b4c-162">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="38b4c-162">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="38b4c-163">Message</span><span class="sxs-lookup"><span data-stu-id="38b4c-163">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="38b4c-164">ItemId</span><span class="sxs-lookup"><span data-stu-id="38b4c-164">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="38b4c-165">Subject</span><span class="sxs-lookup"><span data-stu-id="38b4c-165">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="38b4c-166">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="38b4c-166">DateTimeReceived</span></span>](datetimereceived.md)
    
## <a name="getconversationitems-operation-error-response"></a><span data-ttu-id="38b4c-167">Réponse d’erreur d’opération GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="38b4c-167">GetConversationItems operation error response</span></span>

<span data-ttu-id="38b4c-168">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetConversationItems** afin d’obtenir des éléments dans une conversation qui n’existe plus dans la boîte aux lettres ou pour lesquels tous les éléments de conversation sont situés dans des dossiers ignorés.</span><span class="sxs-lookup"><span data-stu-id="38b4c-168">The following example shows an error response to a **GetConversationItems** operation request to get items in a conversation that either no longer exists in the mailbox, or for which all the conversation items are located in folders that are ignored.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="8" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetConversationItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetConversationItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetConversationItemsResponseMessage>
      </m:ResponseMessages>
    </m:GetConversationItemsResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="38b4c-169">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="38b4c-169">See also</span></span>

- [<span data-ttu-id="38b4c-170">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38b4c-170">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="38b4c-171">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="38b4c-171">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
    
- [<span data-ttu-id="38b4c-172">Opération FindConversation</span><span class="sxs-lookup"><span data-stu-id="38b4c-172">FindConversation operation</span></span>](findconversation-operation.md)
    

