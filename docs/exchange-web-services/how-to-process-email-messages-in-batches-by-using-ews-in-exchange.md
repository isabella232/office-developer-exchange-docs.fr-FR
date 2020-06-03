---
title: Traiter les messages électroniques par lots à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 96390f92-cab1-4de6-9ec2-a55678fc20af
description: Découvrez comment créer, obtenir, mettre à jour et supprimer des lots de messages électroniques dans un seul appel à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 2592076c9c5b57356d96872f006dd7b0abfc328a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527774"
---
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a><span data-ttu-id="f665b-103">Traiter les messages électroniques par lots à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f665b-103">Process email messages in batches by using EWS in Exchange</span></span>

<span data-ttu-id="f665b-104">Découvrez comment créer, obtenir, mettre à jour et supprimer des lots de messages électroniques dans un seul appel à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="f665b-104">Learn how to create, get, update, and delete batches of email messages in a single call by using the EWS Managed API or EWS in Exchange.</span></span>

<span data-ttu-id="f665b-105">Vous pouvez utiliser l’API managée EWS ou EWS pour utiliser des lots de messages électroniques afin de réduire le nombre d’appels effectués par un client sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="f665b-105">You can use the EWS Managed API or EWS to work with batches of email messages to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="f665b-106">Lorsque vous utilisez l’API managée EWS pour créer, obtenir, mettre à jour, supprimer et envoyer des messages par lots, vous utilisez des méthodes d’objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , tandis que lorsque vous travaillez avec des messages électroniques uniques, vous utilisez des méthodes d’objet [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f665b-106">When you use the EWS Managed API to create, get, update, delete, and send messages in batches, you use [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single email messages, you use [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="f665b-107">Si vous utilisez EWS, vous utilisez les mêmes opérations pour travailler avec un seul et même lot de messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="f665b-107">If you are using EWS, you use the same operations to work with both single and batches of email messages.</span></span>

<span data-ttu-id="f665b-108">**Tableau 1. Méthodes de l’API managée EWS et opérations EWS pour l’utilisation de lots de messages électroniques**</span><span class="sxs-lookup"><span data-stu-id="f665b-108">**Table 1. EWS Managed API methods and EWS operations for working with batches of email messages**</span></span>

|<span data-ttu-id="f665b-109">**Afin de...**</span><span class="sxs-lookup"><span data-stu-id="f665b-109">**In order to…**</span></span>|<span data-ttu-id="f665b-110">**Utiliser cette méthode d’API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="f665b-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="f665b-111">**Utiliser cette opération EWS**</span><span class="sxs-lookup"><span data-stu-id="f665b-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f665b-112">Créer des messages électroniques par lots</span><span class="sxs-lookup"><span data-stu-id="f665b-112">Create email messages in batches</span></span>  <br/> |[<span data-ttu-id="f665b-113">ExchangeService. CreateItems</span><span class="sxs-lookup"><span data-stu-id="f665b-113">ExchangeService.CreateItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f665b-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="f665b-114">CreateItem</span></span>](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="f665b-115">Obtenir des messages électroniques par lots</span><span class="sxs-lookup"><span data-stu-id="f665b-115">Get email messages in batches</span></span>  <br/> |[<span data-ttu-id="f665b-116">ExchangeService. BindToItems</span><span class="sxs-lookup"><span data-stu-id="f665b-116">ExchangeService.BindToItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f665b-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="f665b-117">GetItem</span></span>](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="f665b-118">Mettre à jour les messages électroniques par lots</span><span class="sxs-lookup"><span data-stu-id="f665b-118">Update email messages in batches</span></span>  <br/> |[<span data-ttu-id="f665b-119">ExchangeService. UpdateItems</span><span class="sxs-lookup"><span data-stu-id="f665b-119">ExchangeService.UpdateItems</span></span>](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f665b-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="f665b-120">UpdateItem</span></span>](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="f665b-121">Supprimer les messages électroniques par lots</span><span class="sxs-lookup"><span data-stu-id="f665b-121">Delete email messages in batches</span></span>  <br/> |[<span data-ttu-id="f665b-122">ExchangeService. DeleteItems</span><span class="sxs-lookup"><span data-stu-id="f665b-122">ExchangeService.DeleteItems</span></span>](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f665b-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="f665b-123">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |

<span data-ttu-id="f665b-124">Dans cet article, vous allez apprendre à effectuer des tâches de base pour les lots de messages électroniques à l’aide de l’API managée EWS ou d’EWS.</span><span class="sxs-lookup"><span data-stu-id="f665b-124">In this article, you'll learn how to complete basic tasks for batches of email messages by using the EWS Managed API or EWS.</span></span>

## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="f665b-125">Créer des messages électroniques par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="f665b-125">Create email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="f665b-126"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f665b-126"><a name="bk_createewsma"> </a></span></span>

<span data-ttu-id="f665b-127">Vous pouvez créer des messages par lots à l’aide de la méthode **CreateItems** de l’API managée EWS, comme le montre l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f665b-127">You can create messages in batches by using the EWS Managed API **CreateItems** method, as shown in the following example.</span></span> <span data-ttu-id="f665b-128">Cet exemple crée trois objets [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) localement, ajoute chaque message à une collection, puis appelle la méthode **CreateItems** sur la collection de messages.</span><span class="sxs-lookup"><span data-stu-id="f665b-128">This example creates three [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects locally, adds each message to a collection, then calls the **CreateItems** method on the collection of messages.</span></span>

<span data-ttu-id="f665b-129">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="f665b-129">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span>

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

<span data-ttu-id="f665b-130">Notez que l’exemple enregistre uniquement les messages dans le dossier Brouillons ; Il n’envoie pas les messages.</span><span class="sxs-lookup"><span data-stu-id="f665b-130">Note that the example only saves the messages in the Drafts folder; it does not send the messages.</span></span> <span data-ttu-id="f665b-131">Pour plus d’informations sur l’envoi des messages, consultez [la rubrique envoyer des messages électroniques par lots à l’aide de l’API managée EWS](#bk_sendewsma).</span><span class="sxs-lookup"><span data-stu-id="f665b-131">For more about how to send the messages, see [Send email messages in batches by using the EWS Managed API](#bk_sendewsma).</span></span>

## <a name="create-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="f665b-132">Créer des messages électroniques par lots à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="f665b-132">Create email messages in batches by using EWS</span></span>
<span data-ttu-id="f665b-133"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="f665b-133"><a name="bk_createews"> </a></span></span>

<span data-ttu-id="f665b-134">Vous pouvez créer des messages électroniques par lots à l’aide de l’opération EWS de [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="f665b-134">You can create email messages in batches by using the [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="f665b-135">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [créer des messages électroniques par lots](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="f665b-135">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create email messages in batches](#bk_createewsma).</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="f665b-136">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de la propriété **NOERROR** pour chacun des nouveaux messages, ce qui indique que chaque message électronique a été créé et enregistré.</span><span class="sxs-lookup"><span data-stu-id="f665b-136">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and saved successfully.</span></span>

<span data-ttu-id="f665b-137">Notez que l’exemple enregistre uniquement les messages dans le dossier Brouillons ; Il n’envoie pas les messages.</span><span class="sxs-lookup"><span data-stu-id="f665b-137">Note that the example only saves the messages in the Drafts folder; it does not send the messages.</span></span> <span data-ttu-id="f665b-138">Pour plus d’informations sur l’envoi des messages, consultez la rubrique [Envoyer des messages électroniques par lots à l’aide d’EWS](#bk_sendews).</span><span class="sxs-lookup"><span data-stu-id="f665b-138">For more about how to send the messages, see [Send email messages in batches by using EWS](#bk_sendews).</span></span>

## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="f665b-139">Envoyer des messages électroniques par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="f665b-139">Send email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="f665b-140"><a name="bk_sendewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f665b-140"><a name="bk_sendewsma"> </a></span></span>

<span data-ttu-id="f665b-141">Vous utilisez le même code pour envoyer des messages électroniques par lots que vous utilisez pour créer des messages électroniques par lots, à l’exception des paramètres de la méthode [CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) modifiés.</span><span class="sxs-lookup"><span data-stu-id="f665b-141">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the [CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) method parameters change.</span></span> <span data-ttu-id="f665b-142">Par conséquent, pour envoyer des messages électroniques à l’aide de l’API managée EWS, utilisez le code que vous utilisez pour [créer des messages électroniques par lots](#bk_createewsma)et remplacez l’appel à la méthode **CreateItems** par l’appel dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f665b-142">So, to send email messages by using the EWS Managed API, use the code you use to [create email messages in batches](#bk_createewsma), and replace the call to the **CreateItems** method with the call in the following example.</span></span> <span data-ttu-id="f665b-143">Dans cet exemple, les messages sont créés dans le dossier éléments envoyés, et la disposition du message est remplacée par [MessageDisposition. méthodesendandsavecopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), de sorte que le message est envoyé et pas simplement enregistré localement.</span><span class="sxs-lookup"><span data-stu-id="f665b-143">In this example, the messages are created in the Sent Items folder, and the message disposition is changed to [MessageDisposition.SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), so that the message is sent, and not just saved locally.</span></span>

```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="f665b-144">Envoyer des messages électroniques par lots à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="f665b-144">Send email messages in batches by using EWS</span></span>
<span data-ttu-id="f665b-145"><a name="bk_sendews"> </a></span><span class="sxs-lookup"><span data-stu-id="f665b-145"><a name="bk_sendews"> </a></span></span>

<span data-ttu-id="f665b-146">Vous utilisez le même code pour envoyer des messages électroniques par lots que vous utilisez pour créer des messages électroniques par lots, à l’exception des valeurs d’attribut modifiées pour l’opération **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="f665b-146">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the attribute values change for the **CreateItem** operation.</span></span> <span data-ttu-id="f665b-147">Par conséquent, pour envoyer des messages électroniques à l’aide d’EWS, utilisez le code que vous utilisez pour [créer un message électronique par lots](#bk_createews)et modifiez la valeur **MessageDisposition** en « méthodesendandsavecopy », puis changez [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) en « éléments envoyés », comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="f665b-147">So, to send email messages by using EWS, use the code you use to [create email message in batches](#bk_createews), and change the **MessageDisposition** value to "SendAndSaveCopy", and change the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) to "sentitems", as shown in the following code example.</span></span>

```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

<span data-ttu-id="f665b-148">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de la propriété **NOERROR** pour chacun des nouveaux messages, ce qui indique que chaque message électronique a été créé et envoyé avec succès.</span><span class="sxs-lookup"><span data-stu-id="f665b-148">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and sent successfully.</span></span>

## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="f665b-149">Obtenir des messages électroniques par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="f665b-149">Get email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="f665b-150"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f665b-150"><a name="bk_getewsma"> </a></span></span>

<span data-ttu-id="f665b-151">Vous pouvez obtenir des messages électroniques par lots à l’aide de la méthode [BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) de l’API managée EWS, comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f665b-151">You can get email messages in batches by using the EWS Managed API [BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span>

<span data-ttu-id="f665b-152">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="f665b-152">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span>

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

## <a name="get-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="f665b-153">Obtenir des messages électroniques par lots à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="f665b-153">Get email messages in batches by using EWS</span></span>
<span data-ttu-id="f665b-154"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="f665b-154"><a name="bk_getews"> </a></span></span>

<span data-ttu-id="f665b-155">Vous pouvez obtenir des messages électroniques par lots à l’aide de l’opération EWS de [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) et du code de l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f665b-155">You can get email messages in batches by using the [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation and the code in the following example.</span></span> <span data-ttu-id="f665b-156">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [récupérer des messages électroniques par lots](#bk_getewsma).</span><span class="sxs-lookup"><span data-stu-id="f665b-156">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get email messages in batches](#bk_getewsma).</span></span>

<span data-ttu-id="f665b-157">[!REMARQUE] Les attributs **ItemId** et **ChangeKey** ont été réduits pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="f665b-157">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="f665b-158">Le serveur répond à la demande **GetItem** avec un message [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) qui inclut les [Propriétés de première classe](email-properties-and-elements-in-ews-in-exchange.md) de chacun des messages demandés.</span><span class="sxs-lookup"><span data-stu-id="f665b-158">The server responds to the **GetItem** request with a [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes the [first class properties](email-properties-and-elements-in-ews-in-exchange.md) for each of the requested messages.</span></span>

## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="f665b-159">Mettre à jour les messages électroniques par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="f665b-159">Update email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="f665b-160"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f665b-160"><a name="bk_updateewsma"> </a></span></span>

<span data-ttu-id="f665b-161">Vous pouvez obtenir des messages électroniques par lots à l’aide de la méthode [UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) de l’API managée EWS, comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f665b-161">You can get email messages in batches by using the EWS Managed API [UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span>

<span data-ttu-id="f665b-162">Pour obtenir la liste des propriétés d’un message électronique accessible en écriture, consultez la rubrique [Propriétés et éléments de messagerie dans EWS dans Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="f665b-162">For a list of writable email message properties, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span></span>

<span data-ttu-id="f665b-163">Pour plus d’informations sur l’envoi d’un brouillon de message après sa mise à jour, consultez [la rubrique envoi de messages électroniques à l’aide de l’API managée EWS](#bk_sendewsma).</span><span class="sxs-lookup"><span data-stu-id="f665b-163">For details about how to send a draft message after it's been updated, see [Sending email messages by using the EWS Managed API](#bk_sendewsma).</span></span>

<span data-ttu-id="f665b-164">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="f665b-164">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span>

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

## <a name="update-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="f665b-165">Mettre à jour les messages électroniques par lots à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="f665b-165">Update email messages in batches by using EWS</span></span>
<span data-ttu-id="f665b-166"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="f665b-166"><a name="bk_updateews"> </a></span></span>

<span data-ttu-id="f665b-167">Vous pouvez mettre à jour les messages électroniques par lots à l’aide de l’opération EWS de [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) , comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="f665b-167">You can update email messages in batches by using the [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in following code example.</span></span> <span data-ttu-id="f665b-168">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [mettre à jour les messages électroniques par lots](#bk_updateewsma).</span><span class="sxs-lookup"><span data-stu-id="f665b-168">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update email messages in batches](#bk_updateewsma).</span></span>

<span data-ttu-id="f665b-169">Pour obtenir la liste des éléments de message électronique accessibles en écriture, consultez la rubrique [Propriétés et éléments de messagerie dans EWS dans Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="f665b-169">For a list of writable email message elements, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span></span>

<span data-ttu-id="f665b-170">Pour plus d’informations sur l’envoi d’un brouillon de message après sa mise à jour, consultez la rubrique [Envoyer un brouillon de message électronique à l’aide d’EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span><span class="sxs-lookup"><span data-stu-id="f665b-170">For details about how to send a draft message after it's been updated, see [Send a draft email message by using EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="f665b-171">Le serveur répond à la demande **UpdateItem** avec un message [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que chaque mise à jour a été enregistrée avec succès sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="f665b-171">The server responds to the **UpdateItem** request with an [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server.</span></span> <span data-ttu-id="f665b-172">Tous les conflits sont signalés dans l’élément [ConflictResult](https://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f665b-172">Any conflicts are reported in the [ConflictResult](https://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span>

## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="f665b-173">Supprimer des messages électroniques par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="f665b-173">Delete email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="f665b-174"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f665b-174"><a name="bk_deleteewsma"> </a></span></span>

<span data-ttu-id="f665b-175">Vous pouvez supprimer des messages par lots à l’aide de la méthode [DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) de l’API managée EWS, comme le montre l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f665b-175">You can delete messages in batches by using the EWS Managed API [DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span>

<span data-ttu-id="f665b-176">Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="f665b-176">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span>

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

## <a name="delete-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="f665b-177">Supprimer des messages électroniques par lots à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="f665b-177">Delete email messages in batches by using EWS</span></span>
<span data-ttu-id="f665b-178"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="f665b-178"><a name="bk_deleteews"> </a></span></span>

<span data-ttu-id="f665b-179">Vous pouvez supprimer des messages électroniques par lots à l’aide [de l’opération EWS EWS](../web-service-reference/deleteitem-operation.md) , comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="f665b-179">You can delete email messages in batches by using the [DeleteItem](../web-service-reference/deleteitem-operation.md) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="f665b-180">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [Supprimer les messages électroniques par lots](#bk_deleteewsma).</span><span class="sxs-lookup"><span data-stu-id="f665b-180">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete email messages in batches](#bk_deleteewsma).</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="f665b-181">Le serveur répond à la demande **DeleteItem** avec un message [updateitemresponse](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) pour **chaque** élément supprimé.</span><span class="sxs-lookup"><span data-stu-id="f665b-181">The server responds to the **DeleteItem** request with a [DeleteItemResponse](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed.</span></span> <span data-ttu-id="f665b-182">Notez que l’opération renvoie également Success si l’ID d’élément est introuvable.</span><span class="sxs-lookup"><span data-stu-id="f665b-182">Note that the operation also returns success if the item ID could not be found.</span></span>

## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="f665b-183">Vérification de l’exécution réussie d’un processus de traitement par lots</span><span class="sxs-lookup"><span data-stu-id="f665b-183">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="f665b-184"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="f665b-184"><a name="bk_successful"> </a></span></span>

<span data-ttu-id="f665b-185">Lorsqu’un ou plusieurs messages électroniques dans une demande groupée ne peuvent pas être traités comme demandés, une erreur est renvoyée pour chaque message électronique ayant échoué et le reste des courriers électroniques dans le lot est traité comme prévu.</span><span class="sxs-lookup"><span data-stu-id="f665b-185">When one or more email messages in a batched request can't be processed as requested, an error is returned for each email message that failed, and the rest of the emails in the batch are processed as expected.</span></span> <span data-ttu-id="f665b-186">Des défaillances dans le traitement par lots peuvent se produire si l’élément a été supprimé et, par conséquent, ne peut pas être envoyé, récupéré ou mis à jour, ou si l’élément a été déplacé vers un autre dossier, et par conséquent a un nouvel ID d’élément, et qu’il ne peut pas être modifié avec l’ID d’élément envoyé.</span><span class="sxs-lookup"><span data-stu-id="f665b-186">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent.</span></span> <span data-ttu-id="f665b-187">Les informations contenues dans cette section indiquent comment obtenir des détails sur les échecs de traitement par lots de messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="f665b-187">The information in this section shows how to get error details about failures in batch processing of email message.</span></span>

<span data-ttu-id="f665b-188">Pour vérifier la réussite d’un processus de traitement par lots à l’aide de l’API managée EWS, vous pouvez vérifier que la propriété [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) de l' [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) est égale à [ServiceResult. Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="f665b-188">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="f665b-189">Si c’est le cas, tous les messages électroniques ont été traités avec succès.</span><span class="sxs-lookup"><span data-stu-id="f665b-189">If so, all the emails were processed successfully.</span></span> <span data-ttu-id="f665b-190">Si **OverallResult** n’est pas égal à **ServiceResult. Success**, un ou plusieurs messages électroniques n’ont pas été traités.</span><span class="sxs-lookup"><span data-stu-id="f665b-190">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the emails were not processed successfully.</span></span> <span data-ttu-id="f665b-191">Chacun des objets renvoyés dans l' **ServiceResponseCollection** contient les propriétés suivantes :</span><span class="sxs-lookup"><span data-stu-id="f665b-191">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span>

- [<span data-ttu-id="f665b-192">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="f665b-192">ErrorCode</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)

- [<span data-ttu-id="f665b-193">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f665b-193">ErrorDetails</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)

- [<span data-ttu-id="f665b-194">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="f665b-194">ErrorMessage</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)

- [<span data-ttu-id="f665b-195">ErrorProperties</span><span class="sxs-lookup"><span data-stu-id="f665b-195">ErrorProperties</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)

- [<span data-ttu-id="f665b-196">Résultat</span><span class="sxs-lookup"><span data-stu-id="f665b-196">Result</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)

<span data-ttu-id="f665b-197">Ces propriétés contiennent des informations sur la raison pour laquelle les messages électroniques n’ont pas pu être traités comme demandé.</span><span class="sxs-lookup"><span data-stu-id="f665b-197">These properties contain information about why the email messages could not be processed as requested.</span></span> <span data-ttu-id="f665b-198">Les exemples de cet article impriment les **résultats**, **ErrorCode**et **ErrorMessage** pour chaque message ayant échoué.</span><span class="sxs-lookup"><span data-stu-id="f665b-198">The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed message.</span></span> <span data-ttu-id="f665b-199">Vous pouvez utiliser ces résultats pour examiner le problème.</span><span class="sxs-lookup"><span data-stu-id="f665b-199">You can use these results to investigate the issue.</span></span>

<span data-ttu-id="f665b-200">Pour EWS, pour vérifier la réussite d’un processus par lot, vérifiez l’attribut [ResponseClass](https://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) pour chaque élément en cours de traitement.</span><span class="sxs-lookup"><span data-stu-id="f665b-200">For EWS, to verify the success of a batched process, check the [ResponseClass](https://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed.</span></span> <span data-ttu-id="f665b-201">Voici la structure de base du **ResponseMessageType**, le type de base à partir duquel sont dérivés tous les messages de réponse.</span><span class="sxs-lookup"><span data-stu-id="f665b-201">The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span>

```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="f665b-202">L’attribut **ResponseClass** est défini sur **Success** si le message électronique a été traité avec succès ou une **erreur** si le message n’a pas été traité correctement.</span><span class="sxs-lookup"><span data-stu-id="f665b-202">The **ResponseClass** attribute is set to **Success** if the email was processed successfully, or **Error** if the email was not processed successfully.</span></span> <span data-ttu-id="f665b-203">Pour les messages électroniques, vous ne rencontrerez aucun **Avertissement** pendant le traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="f665b-203">For email messages, you will not encounter a **Warning** during batch processing.</span></span> <span data-ttu-id="f665b-204">Si **ResponseClass** **réussit**, l’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) qui suit est également toujours défini sur **NOERROR**.</span><span class="sxs-lookup"><span data-stu-id="f665b-204">If the **ResponseClass** is **Success**, the [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**.</span></span> <span data-ttu-id="f665b-205">Si **ResponseClass** est une **erreur**, vous devez vérifier les valeurs des éléments [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**et [messagexml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) pour déterminer la cause du problème.</span><span class="sxs-lookup"><span data-stu-id="f665b-205">If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem.</span></span> <span data-ttu-id="f665b-206">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) n’est actuellement pas utilisé.</span><span class="sxs-lookup"><span data-stu-id="f665b-206">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span>

## <a name="see-also"></a><span data-ttu-id="f665b-207">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f665b-207">See also</span></span>


- [<span data-ttu-id="f665b-208">Courrier électronique et les services EWS d'Exchange</span><span class="sxs-lookup"><span data-stu-id="f665b-208">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)

- [<span data-ttu-id="f665b-209">Envoyer des messages électroniques à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f665b-209">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)

- [<span data-ttu-id="f665b-210">Répondre à des messages électroniques à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f665b-210">Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)

- [<span data-ttu-id="f665b-211">Déplacer et copier des messages électroniques à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f665b-211">Move and copy email messages by using EWS in Exchange</span></span>](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)

- [<span data-ttu-id="f665b-212">Implications de limitation pour les demandes de lots EWS</span><span class="sxs-lookup"><span data-stu-id="f665b-212">Throttling implications for EWS batch requests</span></span>](ews-throttling-in-exchange.md#throttling-implications-for-ews-batch-requests)
