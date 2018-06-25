---
title: Traiter les messages électroniques par lots à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 96390f92-cab1-4de6-9ec2-a55678fc20af
description: Découvrez comment créer, obtenir, mettre à jour et supprimer des lots de messages électroniques dans un seul appel à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 30ebbdf4c92111df629c7662987e301d167336e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754947"
---
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a><span data-ttu-id="07372-103">Traiter les messages électroniques par lots à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="07372-103">Process email messages in batches by using EWS in Exchange</span></span>

<span data-ttu-id="07372-104">Découvrez comment créer, obtenir, mettre à jour et supprimer des lots de messages électroniques dans un seul appel à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="07372-104">Learn how to create, get, update, and delete batches of email messages in a single call by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="07372-105">Vous pouvez utiliser l’API managée EWS ou EWS pour travailler avec des lots de messages électroniques pour réduire le nombre d’appels un client permet à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="07372-105">You can use the EWS Managed API or EWS to work with batches of email messages to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="07372-106">Lorsque vous utilisez l’API managée EWS pour créer, obtenir, mettre à jour, supprimer et envoyer des messages par lots, vous utilisez les méthodes de l’objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , tandis que lorsque vous travaillez avec des messages de messagerie unique, vous utilisez les méthodes de l’objet [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="07372-106">When you use the EWS Managed API to create, get, update, delete, and send messages in batches, you use [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single email messages, you use [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="07372-107">Si vous utilisez EWS, vous utilisez les mêmes opérations avec unique et de lots de messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="07372-107">If you are using EWS, you use the same operations to work with both single and batches of email messages.</span></span> 
  
<span data-ttu-id="07372-108">**Le tableau 1. Méthodes d’API managées et opérations EWS pour travailler avec des lots de messages électroniques**</span><span class="sxs-lookup"><span data-stu-id="07372-108">**Table 1. EWS Managed API methods and EWS operations for working with batches of email messages**</span></span>

|<span data-ttu-id="07372-109">**Pour...**</span><span class="sxs-lookup"><span data-stu-id="07372-109">**In order to…**</span></span>|<span data-ttu-id="07372-110">**Utilisez cette méthode de l’API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="07372-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="07372-111">**Utilisez cette opération EWS**</span><span class="sxs-lookup"><span data-stu-id="07372-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="07372-112">Créer des messages électroniques par lots</span><span class="sxs-lookup"><span data-stu-id="07372-112">Create email messages in batches</span></span>  <br/> |[<span data-ttu-id="07372-113">ExchangeService.CreateItems</span><span class="sxs-lookup"><span data-stu-id="07372-113">ExchangeService.CreateItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="07372-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="07372-114">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="07372-115">Obtenir des messages électroniques par lots</span><span class="sxs-lookup"><span data-stu-id="07372-115">Get email messages in batches</span></span>  <br/> |[<span data-ttu-id="07372-116">ExchangeService.BindToItems</span><span class="sxs-lookup"><span data-stu-id="07372-116">ExchangeService.BindToItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="07372-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="07372-117">GetItem</span></span>](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="07372-118">Mettre à jour des messages électroniques par lots</span><span class="sxs-lookup"><span data-stu-id="07372-118">Update email messages in batches</span></span>  <br/> |[<span data-ttu-id="07372-119">ExchangeService.UpdateItems</span><span class="sxs-lookup"><span data-stu-id="07372-119">ExchangeService.UpdateItems</span></span>](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="07372-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="07372-120">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="07372-121">Supprimer des messages électroniques par lots</span><span class="sxs-lookup"><span data-stu-id="07372-121">Delete email messages in batches</span></span>  <br/> |[<span data-ttu-id="07372-122">ExchangeService.DeleteItems</span><span class="sxs-lookup"><span data-stu-id="07372-122">ExchangeService.DeleteItems</span></span>](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="07372-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="07372-123">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="07372-124">Dans cet article, vous allez apprendre à effectuer les tâches de base pour les lots de messages électroniques à l’aide de l’API managée EWS ou EWS.</span><span class="sxs-lookup"><span data-stu-id="07372-124">In this article, you'll learn how to complete basic tasks for batches of email messages by using the EWS Managed API or EWS.</span></span>
  
## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="07372-125">Créer des messages électroniques par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="07372-125">Create email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="07372-126"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="07372-126"></span></span>

<span data-ttu-id="07372-127">Vous pouvez créer des messages par lots à l’aide de la méthode API managées **CreateItems** , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="07372-127">You can create messages in batches by using the EWS Managed API **CreateItems** method, as shown in the following example.</span></span> <span data-ttu-id="07372-128">Cet exemple crée trois objets [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) localement, ajoute chaque message à une collection, puis appelle la méthode **CreateItems** sur la collection de messages.</span><span class="sxs-lookup"><span data-stu-id="07372-128">This example creates three [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects locally, adds each message to a collection, then calls the **CreateItems** method on the collection of messages.</span></span> 
  
<span data-ttu-id="07372-129">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="07372-129">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<ItemId> CreateDraftEmailInBatch(ExchangeService service)
{
    // These are unsaved local instances of an EmailMessage object.
    // Despite the required parameter of an ExchangeService object (service), no call
    // to an Exchange server is made when the objects are instantiated.
    // A call to the Exchange server is made when the service.CreateItems() method is called.
    EmailMessage message1 = new EmailMessage(service);
    EmailMessage message2 = new EmailMessage(service);
    EmailMessage message3 = new EmailMessage(service);
    // Set the properties on the first message.
    message1.Subject = "Project priorities";
    message1.Body = "(1) Buy pizza, (2) Eat pizza";
    message1.ToRecipients.Add("sadie@contoso.com");
    // Set the properties on the second message.
    message2.Subject = "Company Soccer Team";
    message2.Body = "Are you interested in joining?";
    message2.ToRecipients.Add("magdalena@contoso.com");
    // Set the properties on the third message.
    message3.Subject = "Code Blast";
    message3.Body = "Are you interested in getting together to finish the methods for the ContosoLive project?";
    message3.ToRecipients.Add("mack@contoso.com");
    // Add the EmailMessage objects to a collection.
    Collection<EmailMessage> messageItems = new Collection<EmailMessage>() { message1, message2, message3 };
    // Create the batch of email messages on the server.
    // This method call results in an CreateItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.Drafts, MessageDisposition.SaveOnly, null);
    // Instantiate a collection of item IDs to populate from the values that are returned by the Exchange server.
    Collection<ItemId> itemIds = new Collection<ItemId>();
    // Collect the item IDs from the created email messages.
    foreach (EmailMessage message in messageItems)
    {
        try
        {
            itemIds.Add(message.Id);
            Console.WriteLine("Email message '{0}' created successfully.", message.Subject);
        }
        catch (Exception ex)
        {
            // Print out the exception and the last eight characters of the item ID.
            Console.WriteLine("Exception while creating message {0}: {1}", message.Id.ToString().Substring(144), ex.Message);
        }
    }
    // Check for success of the CreateItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
            Console.WriteLine("All locally created messages were successfully saved to the Drafts folder.");
            Console.WriteLine("\r\n");
    }
   
    // If the method did not return success, print the result message for each email.
    else
    {
        int counter = 1;
        foreach (ServiceResponse resp in response)
        {
            // Print out the result and the last eight characters of the item ID.
            Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(144), resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            Console.WriteLine("\r\n");
            counter++;
        }
    }
    return itemIds;
}
```

<span data-ttu-id="07372-130">Notez que l’exemple enregistre uniquement les messages dans le dossier Brouillons. Il n’envoie pas les messages.</span><span class="sxs-lookup"><span data-stu-id="07372-130">Note that the example only saves the messages in the Drafts folder; it does not send the messages.</span></span> <span data-ttu-id="07372-131">Pour plus d’informations sur la façon d’envoyer les messages, voir [Envoyer des messages électroniques par lots à l’aide de l’API managée EWS](#bk_sendewsma).</span><span class="sxs-lookup"><span data-stu-id="07372-131">For more about how to send the messages, see [Send email messages in batches by using the EWS Managed API](#bk_sendewsma).</span></span>
  
## <a name="create-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="07372-132">Créer des messages électroniques par lots à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="07372-132">Create email messages in batches by using EWS</span></span>
<span data-ttu-id="07372-133"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="07372-133"></span></span>

<span data-ttu-id="07372-134">Vous pouvez créer des messages électroniques par lots à l’aide de l’opération EWS [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="07372-134">You can create email messages in batches by using the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="07372-135">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [créer des messages électroniques par lots](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="07372-135">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create email messages in batches](#bk_createewsma).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Project priorities</t:Subject>
          <t:Body BodyType="HTML">(1) Buy pizza, (2) Eat pizza</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>magdalena@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
        <t:Message>
          <t:Subject>Code Blast</t:Subject>
          <t:Body BodyType="HTML">Are you interested in getting together to finish the methods for the ContosoLive project?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>mack@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="07372-136">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** pour chacun des nouveaux messages, ce qui indique que chaque e-mail a été créé et enregistré avec succès .</span><span class="sxs-lookup"><span data-stu-id="07372-136">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and saved successfully.</span></span> 
  
<span data-ttu-id="07372-137">Notez que l’exemple enregistre uniquement les messages dans le dossier Brouillons. Il n’envoie pas les messages.</span><span class="sxs-lookup"><span data-stu-id="07372-137">Note that the example only saves the messages in the Drafts folder; it does not send the messages.</span></span> <span data-ttu-id="07372-138">Pour plus d’informations sur la façon d’envoyer les messages, voir [Envoyer des messages électroniques par lots à l’aide de EWS](#bk_sendews).</span><span class="sxs-lookup"><span data-stu-id="07372-138">For more about how to send the messages, see [Send email messages in batches by using EWS](#bk_sendews).</span></span>
  
## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="07372-139">Envoyer des messages électroniques par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="07372-139">Send email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="07372-140"><a name="bk_sendewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="07372-140"></span></span>

<span data-ttu-id="07372-141">Vous utilisez le même code pour envoyer des messages électroniques par lots que vous utilisez pour créer des messages électroniques en lots, sauf que modifier quelques-uns des paramètres de la méthode [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="07372-141">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) method parameters change.</span></span> <span data-ttu-id="07372-142">Ainsi, pour envoyer des messages électroniques à l’aide de l’API managée EWS, utilisez le code qui que vous permet de [créer des messages électroniques par lots](#bk_createewsma)et remplacez l’appel à la méthode **CreateItems** par l’appel dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="07372-142">So, to send email messages by using the EWS Managed API, use the code you use to [create email messages in batches](#bk_createewsma), and replace the call to the **CreateItems** method with the call in the following example.</span></span> <span data-ttu-id="07372-143">Dans cet exemple, les messages sont créés dans le dossier éléments envoyés, et la destruction du message est remplacée par [MessageDisposition.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), afin que le message est envoyé et pas seulement enregistré localement.</span><span class="sxs-lookup"><span data-stu-id="07372-143">In this example, the messages are created in the Sent Items folder, and the message disposition is changed to [MessageDisposition.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), so that the message is sent, and not just saved locally.</span></span>
  
```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="07372-144">Envoyer des messages électroniques par lots à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="07372-144">Send email messages in batches by using EWS</span></span>
<span data-ttu-id="07372-145"><a name="bk_sendews"> </a></span><span class="sxs-lookup"><span data-stu-id="07372-145"></span></span>

<span data-ttu-id="07372-146">Vous utilisez le même code pour envoyer des messages électroniques par lots que vous permet de créer les messages électroniques en lots, sauf que quelques-unes des valeurs d’attribut Modifier pour l’opération **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="07372-146">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the attribute values change for the **CreateItem** operation.</span></span> <span data-ttu-id="07372-147">Ainsi, pour envoyer des messages électroniques à l’aide de EWS, utilisez le code que vous utilisez pour [créer le message électronique par lots](#bk_createews), remplacez la valeur **MessageDisposition** « SendAndSaveCopy » et modifiez le [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) à « éléments envoyés », comme indiqué dans le exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="07372-147">So, to send email messages by using EWS, use the code you use to [create email message in batches](#bk_createews), and change the **MessageDisposition** value to "SendAndSaveCopy", and change the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) to "sentitems", as shown in the following code example.</span></span> 
  
```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

<span data-ttu-id="07372-148">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** pour chacun des nouveaux messages, ce qui indique que chaque e-mail a été créé et envoyé correctement.</span><span class="sxs-lookup"><span data-stu-id="07372-148">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and sent successfully.</span></span> 
  
## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="07372-149">Obtenir des messages électroniques par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="07372-149">Get email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="07372-150"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="07372-150"></span></span>

<span data-ttu-id="07372-151">Vous pouvez obtenir des messages électroniques par lots à l’aide de la méthode API managées [BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="07372-151">You can get email messages in batches by using the EWS Managed API [BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> 
  
<span data-ttu-id="07372-152">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="07372-152">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<EmailMessage> BatchGetEmailItems(ExchangeService service, Collection<ItemId> itemIds)
{
    // Create a property set that limits the properties returned by the Bind method to only those that are required.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ToRecipients);
    // Get the items from the server.
    // This method call results in a GetItem call to EWS.
    ServiceResponseCollection<GetItemResponse> response = service.BindToItems(itemIds, propSet);
           
    // Instantiate a collection of EmailMessage objects to populate from the values that are returned by the Exchange server.
    Collection<EmailMessage> messageItems = new Collection<EmailMessage>();
    foreach (GetItemResponse getItemResponse in response)
    {
        try
        {
            Item item = getItemResponse.Item;
            EmailMessage message = (EmailMessage)item;
            messageItems.Add(message);
            // Print out confirmation and the last eight characters of the item ID.
            Console.WriteLine("Found item {0}.", message.Id.ToString().Substring(144));
        }
        catch (Exception ex)
        {
           Console.WriteLine("Exception while getting a message: {0}", ex.Message);
        }
    }
    // Check for success of the BindToItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All email messages retrieved successfully.");
        Console.WriteLine("\r\n");
    }
        return messageItems;
}
```

## <a name="get-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="07372-153">Obtenir des messages électroniques par lots à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="07372-153">Get email messages in batches by using EWS</span></span>
<span data-ttu-id="07372-154"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="07372-154"></span></span>

<span data-ttu-id="07372-155">Vous pouvez obtenir des messages électroniques par lots à l’aide de l’opération EWS [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) et le code dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="07372-155">You can get email messages in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation and the code in the following example.</span></span> <span data-ttu-id="07372-156">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [obtenir des messages électroniques par lots](#bk_getewsma).</span><span class="sxs-lookup"><span data-stu-id="07372-156">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get email messages in batches](#bk_getewsma).</span></span> 
  
<span data-ttu-id="07372-157">[!REMARQUE] Les attributs **ItemId** et **ChangeKey** ont été réduits pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="07372-157">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="message:ToRecipients" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="m4NxAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB0" />
        <t:ItemId Id="m4NyAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB1" />
        <t:ItemId Id="m4NzAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB2" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="07372-158">Le serveur répond à la demande de **GetItem** avec un message [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) qui contient les [Propriétés de première classe](email-properties-and-elements-in-ews-in-exchange.md) pour chacun des messages demandés.</span><span class="sxs-lookup"><span data-stu-id="07372-158">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes the [first class properties](email-properties-and-elements-in-ews-in-exchange.md) for each of the requested messages.</span></span> 
  
## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="07372-159">Mettre à jour des messages électroniques par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="07372-159">Update email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="07372-160"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="07372-160"></span></span>

<span data-ttu-id="07372-161">Vous pouvez obtenir des messages électroniques par lots à l’aide de la méthode API managées [UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="07372-161">You can get email messages in batches by using the EWS Managed API [UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> 
  
<span data-ttu-id="07372-162">Pour une liste des propriétés de message électronique accessible en écriture, voir [propriétés et éléments dans les services EWS de messagerie dans Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="07372-162">For a list of writable email message properties, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="07372-163">Pour plus d’informations sur la façon d’envoyer un message de brouillon après est été mis à jour, consultez [envoi de messages électroniques à l’aide de l’API managée EWS](#bk_sendewsma).</span><span class="sxs-lookup"><span data-stu-id="07372-163">For details about how to send a draft message after it's been updated, see [Sending email messages by using the EWS Managed API](#bk_sendewsma).</span></span>
  
<span data-ttu-id="07372-164">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="07372-164">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<EmailMessage> BatchUpdateEmailItems(ExchangeService service, Collection<EmailMessage> messageItems)
{
    // Update the subject of each message locally.
    foreach (EmailMessage message in messageItems)
    {
        // Update the Subject of the email.
        message.Subject = "Updated subject at " + DateTime.Now;
        // Print out confirmation with the last eight characters of the item ID and the email subject.
        Console.WriteLine("Updated local email message {0} with the subject '{1}'.", message.Id.ToString().Substring(144), message.Subject);
    }
    // Send the item updates to the server.
    // This method call results in an UpdateItem call to EWS.
    ServiceResponseCollection<UpdateItemResponse> response = service.UpdateItems(messageItems, WellKnownFolderName.Drafts, ConflictResolutionMode.AutoResolve, MessageDisposition.SaveOnly, null);
    // Check for success of the UpdateItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All email messages updated successfully.\r\n");
    }
    // If the method did not return success, print the result message for each email.
    else
    {
        Console.WriteLine("All emails were not successfully saved on the server.\r\n");
        int counter = 1;
        foreach (ServiceResponse resp in response)
        {
            Console.WriteLine("Result for (message {0}): {1}", counter, resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            counter++;
        }
    }
    return messageItems;
}    
```

## <a name="update-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="07372-165">Mettre à jour des messages électroniques par lots à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="07372-165">Update email messages in batches by using EWS</span></span>
<span data-ttu-id="07372-166"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="07372-166"></span></span>

<span data-ttu-id="07372-167">Vous pouvez mettre à jour les messages électroniques par lots à l’aide de l’opération EWS [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) , comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="07372-167">You can update email messages in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in following code example.</span></span> <span data-ttu-id="07372-168">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [mettre à jour des messages électroniques par lots](#bk_updateewsma).</span><span class="sxs-lookup"><span data-stu-id="07372-168">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update email messages in batches](#bk_updateewsma).</span></span>
  
<span data-ttu-id="07372-169">Pour obtenir la liste des éléments de message électronique accessible en écriture, voir [propriétés et éléments dans les services EWS de messagerie dans Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="07372-169">For a list of writable email message elements, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="07372-170">Pour plus d’informations sur la façon d’envoyer un message de brouillon après est été mis à jour, voir [Envoyer un message électronique de brouillon à l’aide de EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span><span class="sxs-lookup"><span data-stu-id="07372-170">For details about how to send a draft message after it's been updated, see [Send a draft email message by using EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly"
                  ConflictResolution="AutoResolve">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="m4OVAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKCy" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="m4OWAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKCz" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="m4OXAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKC0" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="07372-171">Le serveur répond à la demande **UpdateItem** avec un message [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que les mises à jour a été correctement enregistré sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="07372-171">The server responds to the **UpdateItem** request with an [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server.</span></span> <span data-ttu-id="07372-172">Les conflits sont déclarées dans l’élément [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="07372-172">Any conflicts are reported in the [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span> 
  
## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="07372-173">Supprimer des messages électroniques par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="07372-173">Delete email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="07372-174"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="07372-174"></span></span>

<span data-ttu-id="07372-175">Vous pouvez supprimer des messages par lots à l’aide de la méthode API managées [DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="07372-175">You can delete messages in batches by using the EWS Managed API [DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> 
  
<span data-ttu-id="07372-176">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="07372-176">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void BatchDeleteEmailItems(ExchangeService service, Collection<ItemId> itemIds)
{
    // Delete the batch of email message objects.
    // This method call results in an DeleteItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.DeleteItems(itemIds, DeleteMode.SoftDelete, null, AffectedTaskOccurrence.AllOccurrences);
    
    // Check for success of the DeleteItems method call.
    // DeleteItems returns success even if it does not find all the item IDs.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("Email messages deleted successfully.\r\n");
    }
    // If the method did not return success, print a message.
    else
    {
        Console.WriteLine("Not all email messages deleted successfully.\r\n");
    }
}
```

## <a name="delete-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="07372-177">Supprimer des messages électroniques par lots à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="07372-177">Delete email messages in batches by using EWS</span></span>
<span data-ttu-id="07372-178"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="07372-178"></span></span>

<span data-ttu-id="07372-179">Vous pouvez supprimer des messages électroniques par lots à l’aide de l’opération EWS [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) , comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="07372-179">You can delete email messages in batches by using the [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="07372-180">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [Supprimer des messages électroniques par lots](#bk_deleteewsma).</span><span class="sxs-lookup"><span data-stu-id="07372-180">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete email messages in batches](#bk_deleteewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="SoftDelete"
                  AffectedTaskOccurrences="AllOccurrences">
      <m:ItemIds>
        <t:ItemId Id="m4OkAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDE" />
        <t:ItemId Id="m4OlAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDF" />
        <t:ItemId Id="m4OmAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDG" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="07372-181">Le serveur répond à la demande **DeleteItem** avec un message [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** pour chaque élément qui a été supprimé.</span><span class="sxs-lookup"><span data-stu-id="07372-181">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed.</span></span> <span data-ttu-id="07372-182">Notez que l’opération renvoie également réussite si l’ID de l’élément est introuvable.</span><span class="sxs-lookup"><span data-stu-id="07372-182">Note that the operation also returns success if the item ID could not be found.</span></span> 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="07372-183">Vérification réussie un traitement par lots</span><span class="sxs-lookup"><span data-stu-id="07372-183">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="07372-184"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="07372-184"></span></span>

<span data-ttu-id="07372-185">Lorsqu’un ou plusieurs messages électroniques dans une requête par lot ne peut pas être traités, une erreur est renvoyée pour chaque message électronique qui a échoué, et le reste des e-mails dans le lot sont traitées comme prévu.</span><span class="sxs-lookup"><span data-stu-id="07372-185">When one or more email messages in a batched request can't be processed as requested, an error is returned for each email message that failed, and the rest of the emails in the batch are processed as expected.</span></span> <span data-ttu-id="07372-186">Échecs dans le traitement par lots peuvent se produire si l’élément a été supprimé et par conséquent ne peut pas être envoyé, récupéré ou mis à jour, ou si l’élément déplacé vers un autre dossier et par conséquent ne possède un nouvel ID d’élément et ne peut pas être modifié avec l’ID d’élément envoyé.</span><span class="sxs-lookup"><span data-stu-id="07372-186">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent.</span></span> <span data-ttu-id="07372-187">Les informations contenues dans cette section montre comment obtenir des détails sur les échecs de l’erreur dans le traitement du message électronique.</span><span class="sxs-lookup"><span data-stu-id="07372-187">The information in this section shows how to get error details about failures in batch processing of email message.</span></span>
  
<span data-ttu-id="07372-188">Pour vérifier la réussite d’un processus de traitement par lots à l’aide de l’API managée EWS, vous pouvez vérifier que la propriété [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) de la [ServiceResponseCollection](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx) est égale à [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="07372-188">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="07372-189">Dans ce cas, tous les messages électroniques les traitement a réussi.</span><span class="sxs-lookup"><span data-stu-id="07372-189">If so, all the emails were processed successfully.</span></span> <span data-ttu-id="07372-190">Si **OverallResult** n’est pas égale à **ServiceResult.Success**, un ou plusieurs des e-mails qui n’ont pas été traités avec succès.</span><span class="sxs-lookup"><span data-stu-id="07372-190">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the emails were not processed successfully.</span></span> <span data-ttu-id="07372-191">Chacun des objets retournés dans le **ServiceResponseCollection** contient les propriétés suivantes :</span><span class="sxs-lookup"><span data-stu-id="07372-191">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span> 
  
- [<span data-ttu-id="07372-192">Code d’erreur</span><span class="sxs-lookup"><span data-stu-id="07372-192">ErrorCode</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="07372-193">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="07372-193">ErrorDetails</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="07372-194">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="07372-194">ErrorMessage</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="07372-195">ErrorProperties</span><span class="sxs-lookup"><span data-stu-id="07372-195">ErrorProperties</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="07372-196">Résultat</span><span class="sxs-lookup"><span data-stu-id="07372-196">Result</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
<span data-ttu-id="07372-197">Ces propriétés contiennent des informations sur la raison pour laquelle les messages électroniques pas peuvent être traitées comme demandé.</span><span class="sxs-lookup"><span data-stu-id="07372-197">These properties contain information about why the email messages could not be processed as requested.</span></span> <span data-ttu-id="07372-198">Les exemples de cet article impriment les **résultats**, **code d’erreur**et **ErrorMessage** pour chaque message.</span><span class="sxs-lookup"><span data-stu-id="07372-198">The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed message.</span></span> <span data-ttu-id="07372-199">Vous pouvez utiliser ces résultats pour rechercher le problème.</span><span class="sxs-lookup"><span data-stu-id="07372-199">You can use these results to investigate the issue.</span></span> 
  
<span data-ttu-id="07372-200">Pour EWS, pour vérifier la réussite d’un processus par lot, consultez l’attribut [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) pour chaque élément en cours de traitement.</span><span class="sxs-lookup"><span data-stu-id="07372-200">For EWS, to verify the success of a batched process, check the [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed.</span></span> <span data-ttu-id="07372-201">Voici la structure de base de la **ResponseMessageType**, le type de base à partir de la réponse de tous les messages sont dérivés.</span><span class="sxs-lookup"><span data-stu-id="07372-201">The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span> 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="07372-202">L’attribut **ResponseClass** est défini sur **Réussite** si le message électronique a été correctement traité, ou **erreur** si le courrier électronique n’a pas réussi.</span><span class="sxs-lookup"><span data-stu-id="07372-202">The **ResponseClass** attribute is set to **Success** if the email was processed successfully, or **Error** if the email was not processed successfully.</span></span> <span data-ttu-id="07372-203">Pour les messages électroniques, vous ne rencontrerez pas un **Avertissement** au cours de traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="07372-203">For email messages, you will not encounter a **Warning** during batch processing.</span></span> <span data-ttu-id="07372-204">Si la **ResponseClass** est **opération réussie**, l’élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) qui suit est également définie sur **NoError**.</span><span class="sxs-lookup"><span data-stu-id="07372-204">If the **ResponseClass** is **Success**, the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**.</span></span> <span data-ttu-id="07372-205">Si la **ResponseClass** est **erreur**, vous devez vérifier les valeurs des éléments [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) **ResponseCode**et [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) pour déterminer la cause du problème.</span><span class="sxs-lookup"><span data-stu-id="07372-205">If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem.</span></span> <span data-ttu-id="07372-206">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) n’est actuellement pas utilisé.</span><span class="sxs-lookup"><span data-stu-id="07372-206">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="07372-207">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="07372-207">See also</span></span>


- [<span data-ttu-id="07372-208">Courrier électronique et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="07372-208">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="07372-209">Envoyer des messages électroniques à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="07372-209">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="07372-210">Répondre aux messages électroniques à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="07372-210">Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="07372-211">Déplacer et copier des messages électroniques à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="07372-211">Move and copy email messages by using EWS in Exchange</span></span>](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="07372-212">Limitation des implications en matière de requêtes de lots EWS</span><span class="sxs-lookup"><span data-stu-id="07372-212">Throttling implications for EWS batch requests</span></span>](ews-throttling-in-exchange.md#bk_ThrottlingBatch)
    

