---
title: Utilisation de conversations à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7750528c-acb2-43e5-a1e1-ee201c0e1730
description: Découvrez comment rechercher des conversations, appliquer des actions à des conversations et obtenir des éléments dans des conversations à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 71ef7674086607e1544111071928f3dd74073a77
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754969"
---
# <a name="work-with-conversations-by-using-ews-in-exchange"></a><span data-ttu-id="c294a-103">Utilisation de conversations à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c294a-103">Work with conversations by using EWS in Exchange</span></span>

<span data-ttu-id="c294a-104">Découvrez comment rechercher des conversations, appliquer des actions à des conversations et obtenir des éléments dans des conversations à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="c294a-104">Learn about how to find conversations, apply actions to conversations, and get items in conversations by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="c294a-105">Dans le contexte d’Exchange, les conversations sont un moyen de groupe et de gérer un ensemble de messages électroniques associé.</span><span class="sxs-lookup"><span data-stu-id="c294a-105">In the context of Exchange, conversations are a way to group and manage a related set of email messages.</span></span> <span data-ttu-id="c294a-106">Ils peuvent également fournir un moyen pour afficher les messages associés.</span><span class="sxs-lookup"><span data-stu-id="c294a-106">They can also provide a way to view related messages.</span></span> <span data-ttu-id="c294a-107">Exchange définit en fonction de la valeur de **L’ID de Message** du premier message électronique dans un thread de conversations.</span><span class="sxs-lookup"><span data-stu-id="c294a-107">Exchange defines conversations based on the **Message-ID** value of the first email message in a thread.</span></span> <span data-ttu-id="c294a-108">En-tête de **Message-ID** du message d’origine dans leurs **références de** faire référence à toutes les réponses et les messages et **In-Reply-To** en-têtes.</span><span class="sxs-lookup"><span data-stu-id="c294a-108">All replies and related messages reference the original message's **Message-ID** header in their **References** and **In-Reply-To** headers.</span></span> 
  
<span data-ttu-id="c294a-109">En outre, à l’intérieur de l’enveloppe SOAP, pour chaque message reçu dans une boîte aux lettres, Exchange définit les propriétés spécifiques et les éléments.</span><span class="sxs-lookup"><span data-stu-id="c294a-109">Additionally, inside the SOAP envelope, for each message received in a mailbox, Exchange sets specific properties and elements.</span></span>
  
<span data-ttu-id="c294a-110">**Le tableau 1. Propriétés de conversation et les éléments définie sur tous les messages électroniques**</span><span class="sxs-lookup"><span data-stu-id="c294a-110">**Table 1. Conversation properties and elements set on all email messages**</span></span>

|<span data-ttu-id="c294a-111">**Propriété API managées**</span><span class="sxs-lookup"><span data-stu-id="c294a-111">**EWS Managed API property**</span></span>|<span data-ttu-id="c294a-112">**Élément EWS**</span><span class="sxs-lookup"><span data-stu-id="c294a-112">**EWS element**</span></span>|<span data-ttu-id="c294a-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="c294a-113">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="c294a-114">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="c294a-114">ConversationTopic</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.conversationtopic%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c294a-115">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="c294a-115">ConversationTopic</span></span>](http://msdn.microsoft.com/library/46cacf42-4039-4c8a-9b20-c42cdd9f2760%28Office.15%29.aspx) <br/> |<span data-ttu-id="c294a-116">Contient un formulaire normalisé de la valeur de l’objet qui a été définie sur le message d’origine.</span><span class="sxs-lookup"><span data-stu-id="c294a-116">Contains a normalized form of the subject value that was set on the original message.</span></span> <span data-ttu-id="c294a-117">Il s’agit de la même que l’en-tête de message **Au sujet du Thread** .</span><span class="sxs-lookup"><span data-stu-id="c294a-117">This is the same as the **Thread-Topic** message header.</span></span> <span data-ttu-id="c294a-118">Cette valeur est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="c294a-118">This value is read-only.</span></span>  <br/> |
|[<span data-ttu-id="c294a-119">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="c294a-119">ConversationIndex</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.emailmessage.conversationindex%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c294a-120">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="c294a-120">ConversationIndex</span></span>](http://msdn.microsoft.com/library/fdf47e22-8d93-4ae4-883b-0c9f07f48724%28Office.15%29.aspx) <br/> |<span data-ttu-id="c294a-121">Représente la position de l’élément dans la conversation.</span><span class="sxs-lookup"><span data-stu-id="c294a-121">Represents the position of the item in the conversation.</span></span> <span data-ttu-id="c294a-122">Il s’agit de la même que l’en-tête de message **Index de Thread** .</span><span class="sxs-lookup"><span data-stu-id="c294a-122">This is the same as the **Thread-Index** message header.</span></span> <span data-ttu-id="c294a-123">Cette valeur est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="c294a-123">This value is read-only.</span></span>  <br/> |
   
<span data-ttu-id="c294a-124">Exchange s’applique la même valeur **ConversationTopic** aux réponses sur le premier message et met à jour la valeur **ConversationIndex** pour représenter la position du message par rapport au message d’origine.</span><span class="sxs-lookup"><span data-stu-id="c294a-124">Exchange applies the same **ConversationTopic** value to replies to the first message and then updates the **ConversationIndex** value to represent the message's position relative to the original message.</span></span> <span data-ttu-id="c294a-125">Si le sujet du thread e-mail change, Exchange applique une nouvelle valeur **ConversationTopic** et les nouvelles valeurs **ConversationIndex** à la nouvelle conversation.</span><span class="sxs-lookup"><span data-stu-id="c294a-125">If the subject of the email thread changes, Exchange applies a new **ConversationTopic** value and new **ConversationIndex** values to the new conversation.</span></span> 
  
<span data-ttu-id="c294a-126">**Le tableau 2. Méthodes d’API managées et opérations EWS pour travailler avec des conversations**</span><span class="sxs-lookup"><span data-stu-id="c294a-126">**Table 2. EWS Managed API methods and EWS operations for working with conversations**</span></span>

|<span data-ttu-id="c294a-127">**Pour...**</span><span class="sxs-lookup"><span data-stu-id="c294a-127">**In order to…**</span></span>|<span data-ttu-id="c294a-128">**Utiliser cette méthode d’API managées ou**</span><span class="sxs-lookup"><span data-stu-id="c294a-128">**Use this EWS Managed API method or methods**</span></span>|<span data-ttu-id="c294a-129">**Utilisez cette opération EWS**</span><span class="sxs-lookup"><span data-stu-id="c294a-129">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c294a-130">Rechercher des conversations</span><span class="sxs-lookup"><span data-stu-id="c294a-130">Find conversations</span></span>  <br/> |[<span data-ttu-id="c294a-131">ExchangeService.FindConversation</span><span class="sxs-lookup"><span data-stu-id="c294a-131">ExchangeService.FindConversation</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c294a-132">FindConversation</span><span class="sxs-lookup"><span data-stu-id="c294a-132">FindConversation</span></span>](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="c294a-133">Appliquer des actions de conversation</span><span class="sxs-lookup"><span data-stu-id="c294a-133">Apply conversation actions</span></span>  <br/> |[<span data-ttu-id="c294a-134">Conversation.EnableAlwaysCategorizeItems</span><span class="sxs-lookup"><span data-stu-id="c294a-134">Conversation.EnableAlwaysCategorizeItems</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.conversation.enablealwayscategorizeitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-135">Conversation.EnableAlwaysDeleteItems</span><span class="sxs-lookup"><span data-stu-id="c294a-135">Conversation.EnableAlwaysDeleteItems</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-136">Conversation.EnableAlwaysMoveItems</span><span class="sxs-lookup"><span data-stu-id="c294a-136">Conversation.EnableAlwaysMoveItems</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.conversation.enablealwaysmoveitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-137">ExchangeService.CopyItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-137">ExchangeService.CopyItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.copyitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-138">ExchangeService.DeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-138">ExchangeService.DeleteItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.deleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-139">ExchangeService.DisableAlwaysCategorizeItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-139">ExchangeService.DisableAlwaysCategorizeItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.disablealwayscategorizeitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-140">ExchangeService.DisableAlwaysDeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-140">ExchangeService.DisableAlwaysDeleteItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.disablealwaysdeleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-141">ExchangeService.DisableAlwaysMoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-141">ExchangeService.DisableAlwaysMoveItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.disablealwaysmoveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-142">ExchangeService.EnableAlwaysCategorizeItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-142">ExchangeService.EnableAlwaysCategorizeItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.enablealwayscategorizeitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-143">ExchangeService.EnableAlwaysDeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-143">ExchangeService.EnableAlwaysDeleteItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.enablealwaysdeleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-144">ExchangeService.EnableAlwaysMoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-144">ExchangeService.EnableAlwaysMoveItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.enablealwaysmoveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-145">ExchangeService.MoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-145">ExchangeService.MoveItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.moveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-146">ExchangeService.SetFlagStatusForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-146">ExchangeService.SetFlagStatusForItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.setflagstatusforitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-147">ExchangeService.SetReadStateForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-147">ExchangeService.SetReadStateForItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.setreadstateforitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="c294a-148">ExchangeService.SetRetentionPolicyForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="c294a-148">ExchangeService.SetRetentionPolicyForItemsInConversations</span></span>](http://msdn.microsoft.com/fr-fr/library/office/microsoft.exchange.webservices.data.exchangeservice.setretentionpolicyforitemsinconversations%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c294a-149">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="c294a-149">ApplyConversationAction</span></span>](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="c294a-150">Obtenir des éléments dans un ou plusieurs conversations</span><span class="sxs-lookup"><span data-stu-id="c294a-150">Get items in one or more conversations</span></span>  <br/> |[<span data-ttu-id="c294a-151">ExchangeService.GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="c294a-151">ExchangeService.GetConversationItems</span></span>](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c294a-152">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="c294a-152">GetConversationItems</span></span>](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |

<span data-ttu-id="c294a-153"><a name="bk_findewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="c294a-153"></span></span>

## <a name="find-a-conversation-by-using-the-ews-managed-api"></a><span data-ttu-id="c294a-154">Rechercher une conversation à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="c294a-154">Find a conversation by using the EWS Managed API</span></span>

<span data-ttu-id="c294a-155">Vous pouvez rechercher les conversations à l’aide de la méthode API managées [ExchangeService.FindConversation](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) , comme indiqué dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="c294a-155">You can find conversations by using the [ExchangeService.FindConversation](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="c294a-156">Cet exemple obtient les 10 premiers conversations dans le dossier boîte de réception dont l’objet qui contient le mot « news ».</span><span class="sxs-lookup"><span data-stu-id="c294a-156">This example gets the first 10 conversations in the Inbox folder that have a subject that contains the word "news".</span></span> <span data-ttu-id="c294a-157">L’exemple écrit ensuite le sujet de conversation, dernière heure de remise et liste des destinataires unique global dans la fenêtre de console.</span><span class="sxs-lookup"><span data-stu-id="c294a-157">The example then writes the conversation topic, last delivery time, and global unique recipient list to the console window.</span></span> 
  
<span data-ttu-id="c294a-158">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c294a-158">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void FindConversation(ExchangeService service)
{
    // Create the view of conversations returned in the response. This view will return at most 10 results.
    ConversationIndexedItemView view = new ConversationIndexedItemView(10);
    // Create the query string to search for.
    String queryString = "subject:news";
    // Search the Inbox for conversations and return a results set with the specified view.
    // This method call results in a FindConversation call to EWS. 
    ICollection<Conversation> conversations = service.FindConversation(view, WellKnownFolderName.Inbox, queryString);
    // Examine properties on each conversation returned in the response.
    foreach (Conversation conversation in conversations)
    {
        Console.WriteLine("Conversation Topic: " + conversation.Topic);
        Console.WriteLine("Last Delivered: " + conversation.LastDeliveryTime.ToString());
        ApplyConversationActions(service, conversation);
        foreach (string GlUniqRec in conversation.GlobalUniqueRecipients)
        {
            Console.WriteLine("Global Unique Recipient: " + GlUniqRec);
        }
        Console.WriteLine("");
    }
}
```

<span data-ttu-id="c294a-159"><a name="bk_findews"> </a></span><span class="sxs-lookup"><span data-stu-id="c294a-159"></span></span>

## <a name="find-a-conversation-by-using-ews"></a><span data-ttu-id="c294a-160">Rechercher une conversation à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="c294a-160">Find a conversation by using EWS</span></span>

<span data-ttu-id="c294a-161">Vous pouvez rechercher les conversations à l’aide de l’opération EWS [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="c294a-161">You can find conversations by using the [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) EWS operation, as shown in the following example.</span></span> <span data-ttu-id="c294a-162">Cet exemple obtient les dix premiers conversations dans le dossier boîte de réception dont l’objet qui contient le mot « news ».</span><span class="sxs-lookup"><span data-stu-id="c294a-162">This example gets the first ten conversations in the Inbox folder that have a subject that contains the word "news".</span></span> <span data-ttu-id="c294a-163">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [Rechercher une conversation](#bk_findewsma).</span><span class="sxs-lookup"><span data-stu-id="c294a-163">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [find a conversation](#bk_findewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindConversation>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:QueryString>subject:news</m:QueryString>
    </m:FindConversation>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="c294a-164">Le serveur répond à la demande **FindConversation** avec un message [FindConversationResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** pour indiquer que l’opération s’est terminée correctement.</span><span class="sxs-lookup"><span data-stu-id="c294a-164">The server responds to the **FindConversation** request with a [FindConversationResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** to indicate that the operation completed successfully.</span></span> <span data-ttu-id="c294a-165">La réponse inclut également la conversation uniquement dans la boîte aux lettres ayant un objet qui contient le mot « news ».</span><span class="sxs-lookup"><span data-stu-id="c294a-165">The response also includes the only conversation in the mailbox that has a subject that contains the word "news".</span></span> 
  
<span data-ttu-id="c294a-166">Les éléments **ItemId**, **ChangeKey**et **ConversationId** ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c294a-166">The **ItemId**, **ChangeKey**, and **ConversationId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="883"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindConversationResponse ResponseClass="Success"
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Conversations>
        <Conversation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <ConversationId Id="aO2NM+Q=" />
          <ConversationTopic>Today's top news headlines</ConversationTopic>
          <UniqueRecipients>
            <String>Sadie Daniels</String>
          </UniqueRecipients>
          <GlobalUniqueRecipients>
            <String>Sadie Daniels</String>
          </GlobalUniqueRecipients>
          <UniqueUnreadSenders>
            <String>Ronnie Sturgis</String>
          </UniqueUnreadSenders>
          <GlobalUniqueUnreadSenders>
            <String>Ronnie Sturgis</String>
          </GlobalUniqueUnreadSenders>
          <UniqueSenders>
            <String>Ronnie Sturgis</String>
          </UniqueSenders>
          <GlobalUniqueSenders>
            <String>Ronnie Sturgis</String>
          </GlobalUniqueSenders>
          <LastDeliveryTime>2014-02-18T20:42:26Z</LastDeliveryTime>
          <GlobalLastDeliveryTime>2014-02-18T20:42:26Z</GlobalLastDeliveryTime>
          <HasAttachments>false</HasAttachments>
          <GlobalHasAttachments>false</GlobalHasAttachments>
          <MessageCount>1</MessageCount>
          <GlobalMessageCount>1</GlobalMessageCount>
          <UnreadCount>1</UnreadCount>
          <GlobalUnreadCount>1</GlobalUnreadCount>
          <Size>9330</Size>
          <GlobalSize>9330</GlobalSize>
          <ItemClasses>
            <ItemClass>IPM.Note</ItemClass>
          </ItemClasses>
          <GlobalItemClasses>
            <ItemClass>IPM.Note</ItemClass>
          </GlobalItemClasses>
          <Importance>Normal</Importance>
          <GlobalImportance>Normal</GlobalImportance>
          <ItemIds>
            <ItemId Id="sVCyAAA="
                    ChangeKey="CQAAAA==" />
          </ItemIds>
          <GlobalItemIds>
            <ItemId Id="sVCyAAA="
                    ChangeKey="CQAAAA==" />
          </GlobalItemIds>
          <LastModifiedTime>2014-02-18T20:42:26Z</LastModifiedTime>
          <InstanceKey>AQAAAAAAAQABAAAACbFYggAAAAA=</InstanceKey>
          <HasIrm>false</HasIrm>
          <GlobalHasIrm>false</GlobalHasIrm>
        </Conversation>
      </Conversations>
      <TotalConversationsInView>1</TotalConversationsInView>
      <IndexedOffset>1</IndexedOffset>
    </FindConversationResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="c294a-167"><a name="bk_applyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="c294a-167"></span></span>

## <a name="apply-conversation-actions-by-using-the-ews-managed-api"></a><span data-ttu-id="c294a-168">Appliquer des actions de conversation à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="c294a-168">Apply conversation actions by using the EWS Managed API</span></span>

<span data-ttu-id="c294a-169">Vous pouvez appliquer des actions de conversation à une conversation à l’aide de plusieurs méthodes d’API managées, comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="c294a-169">You can apply conversation actions to a conversation by using a number of EWS Managed API methods, as shown in the following example.</span></span> <span data-ttu-id="c294a-170">Cet exemple montre comment ajoute des catégories aux éléments existants dans une conversation et applique les mêmes catégories à des éléments futurs de la conversation.</span><span class="sxs-lookup"><span data-stu-id="c294a-170">This example adds categories to existing items in a conversation and applies the same categories to future items in the conversation.</span></span> <span data-ttu-id="c294a-171">Il indique également comment activer le déplacement automatique des éléments de la conversation dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="c294a-171">It also shows how to enable the automatic moving of items in the conversation to a folder.</span></span> <span data-ttu-id="c294a-172">Dans cet exemple, les éléments sont déplacés vers le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="c294a-172">In this example, items are moved to the Drafts folder.</span></span>
  
<span data-ttu-id="c294a-173">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c294a-173">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
<span data-ttu-id="c294a-174">Pour obtenir une liste complète des méthodes qui s’appliquent les actions de conversation, voir le tableau 2.</span><span class="sxs-lookup"><span data-stu-id="c294a-174">For a complete list of methods that apply conversation actions, see Table 2.</span></span>
  
```cs
static void ApplyConversationActions(ExchangeService service, Conversation conversation)
{
   // Create a list of categories to apply to a conversation.
   List<string> categories = new List<string>();
   categories.Add("Customer");
   categories.Add("System Integrator");
   // Apply categorization to all items in the conversation and process the request
   // synchronously after enabling this rule and after all item categorization has been applied. 
   // This method call results in an ApplyConversationAction call to EWS.
   conversation.EnableAlwaysCategorizeItems(categories, true);
   // Apply an always move rule to all items in the conversation and move the items
   // to the Drafts folder. Process the request asynchronously and return the response. 
   // immediately. This method call results in an ApplyConversationAction call to EWS.
   conversation.EnableAlwaysMoveItems(WellKnownFolderName.Drafts, false);
}

```

<span data-ttu-id="c294a-175"><a name="bk_applyews"> </a></span><span class="sxs-lookup"><span data-stu-id="c294a-175"></span></span>

## <a name="apply-conversation-actions-by-using-ews"></a><span data-ttu-id="c294a-176">Appliquer des actions de conversation à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="c294a-176">Apply conversation actions by using EWS</span></span>

<span data-ttu-id="c294a-177">Vous pouvez appliquer des actions de conversation, tel que classer, supprimer et déplacer, à l’aide de l’opération [ApplyConversationAction](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="c294a-177">You can apply conversation actions, such as categorize, delete, and move, by using the [ApplyConversationAction](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) operation, as shown in the following example.</span></span> <span data-ttu-id="c294a-178">Cet exemple montre comment ajoute des catégories aux éléments existants dans une conversation et applique les mêmes catégories à des éléments futurs de la conversation.</span><span class="sxs-lookup"><span data-stu-id="c294a-178">This example adds categories to existing items in a conversation and applies the same categories to future items in the conversation.</span></span> <span data-ttu-id="c294a-179">Il indique également comment activer le déplacement automatique des éléments de la conversation dans un dossier ; Dans cet exemple, les éléments sont déplacés vers le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="c294a-179">It also shows how to enable the automatic moving of items in the conversation to a folder; in this example, items are moved to the Drafts folder.</span></span> <span data-ttu-id="c294a-180">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [appliquer des actions de conversation](#bk_applyewsma).</span><span class="sxs-lookup"><span data-stu-id="c294a-180">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [apply conversation actions](#bk_applyewsma).</span></span>
  
<span data-ttu-id="c294a-181">L’élément **ConversationId** a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c294a-181">The **ConversationId** element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:ApplyConversationAction>
      <m:ConversationActions>
        <t:ConversationAction>
          <t:Action>AlwaysMove</t:Action>
          <t:ConversationId Id="jG6WVpg=" />
          <t:ProcessRightAway>false</t:ProcessRightAway>
          <t:DestinationFolderId>
            <t:DistinguishedFolderId Id="drafts" />
          </t:DestinationFolderId>
        </t:ConversationAction>
      </m:ConversationActions>
    </m:ApplyConversationAction>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c294a-182">Le serveur répond à la demande **ApplyConversationAction** avec un message [ApplyConversationActionResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** pour indiquer que l’opération s’est terminée correctement.</span><span class="sxs-lookup"><span data-stu-id="c294a-182">The server responds to the **ApplyConversationAction** request with a [ApplyConversationActionResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** to indicate that the operation completed successfully.</span></span> 

<span data-ttu-id="c294a-183"><a name="bk_getitemssingleewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="c294a-183"></span></span>

## <a name="get-items-in-a-single-conversation-by-using-the-conversation-identifier-in-the-ews-managed-api"></a><span data-ttu-id="c294a-184">Obtenir des éléments dans une seule conversation à l’aide de l’identificateur de conversation dans l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="c294a-184">Get items in a single conversation by using the conversation identifier in the EWS Managed API</span></span>

<span data-ttu-id="c294a-185">Vous pouvez obtenir des éléments dans une conversation à l’aide de la méthode d’API managées [ExchangeService.GetConversationItems](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="c294a-185">You can get items in a conversation by using the [ExchangeService.GetConversationItems](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="c294a-186">Cet exemple fournit le jeu de nœuds de conversation pour la première conversation dans la boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="c294a-186">This example provides the set of conversation nodes for the first conversation in the Inbox.</span></span> <span data-ttu-id="c294a-187">L’identificateur d’élément, le sujet et l’heure de réception pour chaque élément sont retournés dans la réponse, ainsi que les propriétés d’index de conversation parent et les index de conversation.</span><span class="sxs-lookup"><span data-stu-id="c294a-187">The item identifier, subject, and received time for each item are returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="c294a-188">Vous pouvez utiliser les propriétés d’index de conversation pour reconstruire la hiérarchie de nœud.</span><span class="sxs-lookup"><span data-stu-id="c294a-188">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> 
  
<span data-ttu-id="c294a-189">Dans cet exemple, tous les éléments de conversation dans les dossiers d’éléments supprimés et les brouillons par défaut sont ignorés.</span><span class="sxs-lookup"><span data-stu-id="c294a-189">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="c294a-190">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c294a-190">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void GetConversationItemsSingleConversation(ExchangeService service)
{
   try
   {
      // Find the first item in the mailbox.
      // This method call results in an FindItem call to EWS.
      FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Inbox,
                                                         new ItemView(1));
      // Get the conversation identifier of the item. 
      ConversationId convId = results.Items[0].ConversationId;
      // Specify the properties that will be 
      // returned for the items in the conversation.
      PropertySet properties = new PropertySet(BasePropertySet.IdOnly,
                                                ItemSchema.Subject,
                                                ItemSchema.DateTimeReceived);
      // Identify the folders to ignore.
      Collection<FolderId> foldersToIgnore = new Collection<FolderId>() 
          { WellKnownFolderName.DeletedItems, WellKnownFolderName.Drafts };
      // Request the conversation items.
      // This method call results in an GetConversationItems call to EWS.
      ConversationResponse response = service.GetConversationItems(convId,
                                                   properties,
                                                  null,
                                                  foldersToIgnore,
                                                  ConversationSortOrder.TreeOrderDescending);
      // Get the synchronization state of the conversation.
      Console.WriteLine("SyncState: " + response.SyncState);
      Collection<Item> items = new Collection<Item>();
      // Process each node of conversation items.
      foreach (ConversationNode node in response.ConversationNodes)
      {
         Console.WriteLine("Parent conversation index: " + node.ParentConversationIndex);
         Console.WriteLine("Conversation index: " + node.ConversationIndex);
         Console.WriteLine("Conversation node items:");
         // Process each item in the conversation node.
         foreach (Item item in node.Items)
         {
            Console.WriteLine("   Item ID: " + item.Id.UniqueId);
            Console.WriteLine("   Subject: " + item.Subject);
            Console.WriteLine("   Received: " + item.DateTimeReceived);
            items.Add(item);
         }
      }
   }
   // This exception occurs if there is an error with the service.
   catch (ServiceResponseException srException)
   {
      Console.WriteLine(srException);
   }
}

```

<span data-ttu-id="c294a-191">Nous vous recommandons de mettre en cache la propriété **SyncState** pour les requêtes suivantes obtenir des éléments de la conversation.</span><span class="sxs-lookup"><span data-stu-id="c294a-191">We recommend that you cache the **SyncState** property for subsequent requests to get items in the conversation.</span></span> 

<span data-ttu-id="c294a-192"><a name="bk_getitemsmanyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="c294a-192"></span></span>

## <a name="get-items-in-many-conversations-by-using-the-conversationrequest-object-in-the-ews-managed-api"></a><span data-ttu-id="c294a-193">Obtenir des éléments de nombreuses conversations à l’aide de l’objet ConversationRequest dans l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="c294a-193">Get items in many conversations by using the ConversationRequest object in the EWS Managed API</span></span>

<span data-ttu-id="c294a-194">Vous pouvez utiliser l’objet [ConversationRequest](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.conversationrequest%28v=exchg.80%29.aspx) et la méthode d’API managées [ExchangeService.GetConversationItems](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) pour obtenir des éléments de deux ou plusieurs conversations.</span><span class="sxs-lookup"><span data-stu-id="c294a-194">You can use the [ConversationRequest](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.conversationrequest%28v=exchg.80%29.aspx) object and the [ExchangeService.GetConversationItems](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method to get items from two or more conversations.</span></span> <span data-ttu-id="c294a-195">Cet exemple fournit un jeu de nœuds de conversation pour les deux premières conversations dans la boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="c294a-195">This example provides a set of conversation nodes for the first two conversations in the Inbox.</span></span> <span data-ttu-id="c294a-196">L’identificateur d’élément, le sujet et l’heure de réception pour chaque élément seront renvoyés dans la réponse, ainsi que les propriétés d’index de conversation parent et les index de conversation.</span><span class="sxs-lookup"><span data-stu-id="c294a-196">The item identifier, subject, and the received time for each item will be returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="c294a-197">Vous pouvez utiliser les propriétés d’index de conversation pour reconstruire la hiérarchie de nœud.</span><span class="sxs-lookup"><span data-stu-id="c294a-197">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> <span data-ttu-id="c294a-198">Cet exemple suppose que les deux premiers éléments dans la boîte de réception des conversations différents.</span><span class="sxs-lookup"><span data-stu-id="c294a-198">This example assumes that the first two items in the Inbox are from different conversations.</span></span> 
  
<span data-ttu-id="c294a-199">Dans cet exemple, tous les éléments de conversation dans les dossiers d’éléments supprimés et les brouillons par défaut sont ignorés.</span><span class="sxs-lookup"><span data-stu-id="c294a-199">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="c294a-200">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c294a-200">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void GetConversationItemsManyConversations(ExchangeService service)
{
   try
   {
      // Find the first two items in the Inbox. This item will be used to call the GetConversationItems operation.
      // This method call results in an FindItem call to EWS.
      FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Inbox, new ItemView(2));
      // Get the conversation identifier of the first two items in the Inbox. 
      ConversationId convId1 = results.Items[0].ConversationId;
      ConversationId convId2 = results.Items[1].ConversationId;
      
      // Identify two conversation requests. 
      ConversationRequest convR1 = new ConversationRequest();
      convR1.ConversationId = convId1;
      ConversationRequest convR2 = new ConversationRequest();
      convR2.ConversationId = convId2;
      // Create a collection of conversations to fetch. 
      Collection<ConversationRequest> conversations = new Collection<ConversationRequest>();
      conversations.Add(convR1);
      conversations.Add(convR2);
      // Specify the properties that will be returned for the items in the conversation.
      PropertySet properties = new PropertySet(BasePropertySet.IdOnly,
                                                ItemSchema.Subject,
                                                ItemSchema.DateTimeReceived);
      // Identify the folders to ignore.
      Collection<FolderId> foldersToIgnore = new Collection<FolderId>() 
          { WellKnownFolderName.DeletedItems, WellKnownFolderName.Drafts };
      // Request the conversation items.
      // This method call results in an GetConversationItems call to EWS.
      ServiceResponseCollection<GetConversationItemsResponse> responses = 
          service.GetConversationItems(conversations, properties, foldersToIgnore, 
          ConversationSortOrder.TreeOrderDescending);
      // Process each conversation.
      foreach (GetConversationItemsResponse resp in responses)
      {
         // Identify the synchronization state of the conversation.
         Console.WriteLine("Sync State: " + resp.Conversation.SyncState);
         // Process each node in the conversation.
         foreach (ConversationNode node in resp.Conversation.ConversationNodes)
         {
            Console.WriteLine("Parent conversation index: " + node.ParentConversationIndex);
            Console.WriteLine("Conversation index: " + node.ConversationIndex);
            Console.WriteLine("Conversation node items:");
            // Process each item in the conversation node.
            foreach (Item item in node.Items)
            {
               Console.WriteLine("   Item ID: " + item.Id.UniqueId);
               Console.WriteLine("   Subject: " + item.Subject);
               Console.WriteLine("   Received: " + item.DateTimeReceived);
            }
         }
      }
   }
   // This exception occurs if there is an error with the service.
   catch (ServiceResponseException srException)
   { 
      Console.WriteLine(srException);
   }
}

```

<span data-ttu-id="c294a-201">Meilleure pratique, nous vous recommandons de vous renvoyer uniquement les propriétés qui nécessite l’application cliente, au lieu d’utiliser l’option **FirstClassProperties** pour la classe **BasePropertySet** .</span><span class="sxs-lookup"><span data-stu-id="c294a-201">As a best practice, we recommend that you return only the properties that the client application requires, rather than using the **FirstClassProperties** option for the **BasePropertySet** class.</span></span> <span data-ttu-id="c294a-202">Nous vous recommandons de mettre en cache la propriété **SyncState** pour les requêtes suivantes obtenir des éléments de la conversation.</span><span class="sxs-lookup"><span data-stu-id="c294a-202">We recommend that you cache the **SyncState** property for subsequent requests to get items in the conversation.</span></span> 

<span data-ttu-id="c294a-203"><a name="bk_getitemsews"> </a></span><span class="sxs-lookup"><span data-stu-id="c294a-203"></span></span>

## <a name="get-items-in-conversations-by-using-the-conversation-identifier-in-ews"></a><span data-ttu-id="c294a-204">Obtenir des éléments dans des conversations à l’aide de l’identificateur de conversation dans EWS</span><span class="sxs-lookup"><span data-stu-id="c294a-204">Get items in conversations by using the conversation identifier in EWS</span></span>

<span data-ttu-id="c294a-205">Vous pouvez obtenir des éléments dans une conversation à l’aide de l’opération EWS [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="c294a-205">You can get items in a conversation by using the [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="c294a-206">Cet exemple fournit un jeu de nœuds de conversation pour la première conversation dans la boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="c294a-206">This example provides a set of conversation nodes for the first conversation in the Inbox.</span></span> <span data-ttu-id="c294a-207">L’identificateur d’élément, le sujet et l’heure de réception pour chaque élément sont retournés dans la réponse, ainsi que les propriétés d’index de conversation parent et les index de conversation.</span><span class="sxs-lookup"><span data-stu-id="c294a-207">The item identifier, subject, and received time for each item are returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="c294a-208">Vous pouvez utiliser les propriétés d’index de conversation pour reconstruire la hiérarchie de nœud.</span><span class="sxs-lookup"><span data-stu-id="c294a-208">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> 
  
<span data-ttu-id="c294a-209">Dans cet exemple, tous les éléments de conversation dans les dossiers d’éléments supprimés et les brouillons par défaut sont ignorés.</span><span class="sxs-lookup"><span data-stu-id="c294a-209">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="c294a-210">L’élément **ConversationId** a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c294a-210">The **ConversationId** element has been shortened for readability.</span></span> 
  
<span data-ttu-id="c294a-211">Pour obtenir des éléments dans plusieurs conversations, incluent les éléments de **Conversation** supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="c294a-211">To get items from more than one conversation, include additional **Conversation** elements.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m=http://schemas.microsoft.com/exchange/services/2006/messages
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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
          <t:ConversationId Id="LUQFH6Q=" />
        </t:Conversation>
      </m:Conversations>
    </m:GetConversationItems>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **GetConversationItems** avec un message [GetConversationItemsResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** pour indiquer que l’opération s’est terminée correctement. <span data-ttu-id="c294a-213">La réponse inclut également les [ConversationNodes](http://msdn.microsoft.com/library/5c8a35b8-a940-4b3e-8768-9ba95766fd79%28Office.15%29.aspx) dans la conversation.</span><span class="sxs-lookup"><span data-stu-id="c294a-213">The response also includes the [ConversationNodes](http://msdn.microsoft.com/library/5c8a35b8-a940-4b3e-8768-9ba95766fd79%28Office.15%29.aspx) in the conversation.</span></span> 
  
<span data-ttu-id="c294a-214">Les éléments **ItemId**, **SyncState**et **ConversationId** ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c294a-214">The **ItemId**, **SyncState**, and **ConversationId** elements have been shortened for readability.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="873"
                         MinorBuildNumber="9"
                         Version="V2_9"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetConversationItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetConversationItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Conversation>
            <t:ConversationId Id="LUQFH6Q=" />
            <t:SyncState>AAAAYAm1</t:SyncState>
            <t:ConversationNodes>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;994051d7c1a346efbfce8dec2cbad509
                    @SN2SR01MB006.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AYB1NAAA="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYCHq" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T13:15:00Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;6a8e7658524b41cda7cdc3f23c1074a5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="lQAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAu8" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T10:02:08Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;bcdb185495834370a874a1e7ebedbb96
                    @SN2SR01MB005.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;e52a4de6b98d484887e141da094a2ce6
                    @SN2SR01MB006.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="igAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAuj" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T16:20:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;e52a4de6b98d484887e141da094a2ce6
                    @SN2SR01MB006.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;f0db3ead01db4fe087d98022149aa16f
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="iwAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAul" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T15:30:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;f0db3ead01db4fe087d98022149aa16f
                    @SN2SR01MB001.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;88b1884ecaaa4f68b081c009d827e8c6
                    @SN2SR01MB003.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="jQAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAuq" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T14:20:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;88b1884ecaaa4f68b081c009d827e8c6
                    @SN2SR01MB003.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="kAAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAux" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T12:52:09Z</t:DateTimeReceived>
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

<span data-ttu-id="c294a-215"><a name="bk_versiondiffs"> </a></span><span class="sxs-lookup"><span data-stu-id="c294a-215"></span></span>

## <a name="version-differences"></a><span data-ttu-id="c294a-216">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="c294a-216">Version differences</span></span>

<span data-ttu-id="c294a-217">Lorsque vous utilisez Exchange Server 2010 Service Pack 1 (SP1), la méthode [FindConversation](http://msdn.microsoft.com/fr-fr/library/office/jj220668%28v=exchg.80%29.aspx) a moins d’options, et l’opération [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) a moins d’éléments dans la demande.</span><span class="sxs-lookup"><span data-stu-id="c294a-217">When you are using Exchange Server 2010 Service Pack 1 (SP1), the [FindConversation](http://msdn.microsoft.com/fr-fr/library/office/jj220668%28v=exchg.80%29.aspx) method has fewer options available, and the [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) operation has fewer elements in the request.</span></span> 
  
<span data-ttu-id="c294a-218">**Le tableau 3. Prise en charge de la version Exchange 2010 SP1 pour FindConversation**</span><span class="sxs-lookup"><span data-stu-id="c294a-218">**Table 3. Exchange 2010 SP1 version support for FindConversation**</span></span>

|<span data-ttu-id="c294a-219">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="c294a-219">**EWS Managed API method**</span></span>|<span data-ttu-id="c294a-220">**Éléments EWS**</span><span class="sxs-lookup"><span data-stu-id="c294a-220">**EWS elements**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c294a-221">FindConversation (ViewBase, FolderId)</span><span class="sxs-lookup"><span data-stu-id="c294a-221">FindConversation (ViewBase, FolderId)</span></span>](http://msdn.microsoft.com/fr-fr/library/office/jj220668%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="c294a-222">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="c294a-222">IndexedPageItemView</span></span>](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) <br/> [<span data-ttu-id="c294a-223">SortOrder</span><span class="sxs-lookup"><span data-stu-id="c294a-223">SortOrder</span></span>](http://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) <br/> [<span data-ttu-id="c294a-224">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="c294a-224">ParentFolderId</span></span>](http://msdn.microsoft.com/library/0e3e6e5f-06d0-499b-8ca4-d36036521658%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="c294a-225">La méthode d’API managées [GetConversationItems](http://msdn.microsoft.com/fr-fr/library/office/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) et l’opération EWS [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) ont été introduites dans Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c294a-225">The [GetConversationItems](http://msdn.microsoft.com/fr-fr/library/office/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method and the [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS operation were introduced in Exchange Server 2013.</span></span> <span data-ttu-id="c294a-226">Les applications qui ciblent les versions antérieures d’Exchange ne pouvant appliquer les actions de conversation à des conversations, comme indiqué dans le tableau 2.</span><span class="sxs-lookup"><span data-stu-id="c294a-226">Applications that target earlier versions of Exchange can only apply conversation actions to conversations, as listed in Table 2.</span></span> 
  
<span data-ttu-id="c294a-227">La méthode **FindConversation** API managées et la méthode EWS **FindConversation** ne sont pas disponibles dans la version initiale d’Exchange 2010 ou Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="c294a-227">The **FindConversation** EWS Managed API method and the **FindConversation** EWS method are not available in the initial release version of Exchange 2010 or in Exchange 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c294a-228">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c294a-228">See also</span></span>

- [<span data-ttu-id="c294a-229">Courrier électronique et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="c294a-229">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
- [<span data-ttu-id="c294a-230">Utiliser des filtres de recherche avec EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c294a-230">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)   
- [<span data-ttu-id="c294a-231">Exchange 2013 : Rechercher des conversations dans les boîtes aux lettres par programme</span><span class="sxs-lookup"><span data-stu-id="c294a-231">Exchange 2013: Find conversations in mailboxes programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Find-d4b6b3af)    
- [<span data-ttu-id="c294a-232">Exchange 2013 : Appliquer les actions pour gérer les conversations dans une boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="c294a-232">Exchange 2013: Apply actions to manage conversations in a mailbox</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Apply-accde0b5)
    

