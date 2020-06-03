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
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a>Traiter les messages électroniques par lots à l’aide d’EWS dans Exchange

Découvrez comment créer, obtenir, mettre à jour et supprimer des lots de messages électroniques dans un seul appel à l’aide de l’API managée EWS ou d’EWS dans Exchange.

Vous pouvez utiliser l’API managée EWS ou EWS pour utiliser des lots de messages électroniques afin de réduire le nombre d’appels effectués par un client sur un serveur Exchange. Lorsque vous utilisez l’API managée EWS pour créer, obtenir, mettre à jour, supprimer et envoyer des messages par lots, vous utilisez des méthodes d’objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , tandis que lorsque vous travaillez avec des messages électroniques uniques, vous utilisez des méthodes d’objet [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) . Si vous utilisez EWS, vous utilisez les mêmes opérations pour travailler avec un seul et même lot de messages électroniques.

**Tableau 1. Méthodes de l’API managée EWS et opérations EWS pour l’utilisation de lots de messages électroniques**

|**Afin de...**|**Utiliser cette méthode d’API managée EWS**|**Utiliser cette opération EWS**|
|:-----|:-----|:-----|
|Créer des messages électroniques par lots  <br/> |[ExchangeService. CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Obtenir des messages électroniques par lots  <br/> |[ExchangeService. BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|Mettre à jour les messages électroniques par lots  <br/> |[ExchangeService. UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) <br/> |[UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Supprimer les messages électroniques par lots  <br/> |[ExchangeService. DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |

Dans cet article, vous allez apprendre à effectuer des tâches de base pour les lots de messages électroniques à l’aide de l’API managée EWS ou d’EWS.

## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a>Créer des messages électroniques par lots à l’aide de l’API managée EWS
<a name="bk_createewsma"> </a>

Vous pouvez créer des messages par lots à l’aide de la méthode **CreateItems** de l’API managée EWS, comme le montre l’exemple suivant. Cet exemple crée trois objets [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) localement, ajoute chaque message à une collection, puis appelle la méthode **CreateItems** sur la collection de messages.

Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.

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

Notez que l’exemple enregistre uniquement les messages dans le dossier Brouillons ; Il n’envoie pas les messages. Pour plus d’informations sur l’envoi des messages, consultez [la rubrique envoyer des messages électroniques par lots à l’aide de l’API managée EWS](#bk_sendewsma).

## <a name="create-email-messages-in-batches-by-using-ews"></a>Créer des messages électroniques par lots à l’aide d’EWS
<a name="bk_createews"> </a>

Vous pouvez créer des messages électroniques par lots à l’aide de l’opération EWS de [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , comme illustré dans l’exemple de code suivant. Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [créer des messages électroniques par lots](#bk_createewsma).

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

Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de la propriété **NOERROR** pour chacun des nouveaux messages, ce qui indique que chaque message électronique a été créé et enregistré.

Notez que l’exemple enregistre uniquement les messages dans le dossier Brouillons ; Il n’envoie pas les messages. Pour plus d’informations sur l’envoi des messages, consultez la rubrique [Envoyer des messages électroniques par lots à l’aide d’EWS](#bk_sendews).

## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a>Envoyer des messages électroniques par lots à l’aide de l’API managée EWS
<a name="bk_sendewsma"> </a>

Vous utilisez le même code pour envoyer des messages électroniques par lots que vous utilisez pour créer des messages électroniques par lots, à l’exception des paramètres de la méthode [CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) modifiés. Par conséquent, pour envoyer des messages électroniques à l’aide de l’API managée EWS, utilisez le code que vous utilisez pour [créer des messages électroniques par lots](#bk_createewsma)et remplacez l’appel à la méthode **CreateItems** par l’appel dans l’exemple suivant. Dans cet exemple, les messages sont créés dans le dossier éléments envoyés, et la disposition du message est remplacée par [MessageDisposition. méthodesendandsavecopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), de sorte que le message est envoyé et pas simplement enregistré localement.

```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a>Envoyer des messages électroniques par lots à l’aide d’EWS
<a name="bk_sendews"> </a>

Vous utilisez le même code pour envoyer des messages électroniques par lots que vous utilisez pour créer des messages électroniques par lots, à l’exception des valeurs d’attribut modifiées pour l’opération **CreateItem** . Par conséquent, pour envoyer des messages électroniques à l’aide d’EWS, utilisez le code que vous utilisez pour [créer un message électronique par lots](#bk_createews)et modifiez la valeur **MessageDisposition** en « méthodesendandsavecopy », puis changez [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) en « éléments envoyés », comme illustré dans l’exemple de code suivant.

```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de la propriété **NOERROR** pour chacun des nouveaux messages, ce qui indique que chaque message électronique a été créé et envoyé avec succès.

## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a>Obtenir des messages électroniques par lots à l’aide de l’API managée EWS
<a name="bk_getewsma"> </a>

Vous pouvez obtenir des messages électroniques par lots à l’aide de la méthode [BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) de l’API managée EWS, comme illustré dans l’exemple suivant.

Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.

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

## <a name="get-email-messages-in-batches-by-using-ews"></a>Obtenir des messages électroniques par lots à l’aide d’EWS
<a name="bk_getews"> </a>

Vous pouvez obtenir des messages électroniques par lots à l’aide de l’opération EWS de [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) et du code de l’exemple suivant. Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [récupérer des messages électroniques par lots](#bk_getewsma).

[!REMARQUE] Les attributs **ItemId** et **ChangeKey** ont été réduits pour une meilleure lisibilité.

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

Le serveur répond à la demande **GetItem** avec un message [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) qui inclut les [Propriétés de première classe](email-properties-and-elements-in-ews-in-exchange.md) de chacun des messages demandés.

## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a>Mettre à jour les messages électroniques par lots à l’aide de l’API managée EWS
<a name="bk_updateewsma"> </a>

Vous pouvez obtenir des messages électroniques par lots à l’aide de la méthode [UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) de l’API managée EWS, comme illustré dans l’exemple suivant.

Pour obtenir la liste des propriétés d’un message électronique accessible en écriture, consultez la rubrique [Propriétés et éléments de messagerie dans EWS dans Exchange](email-properties-and-elements-in-ews-in-exchange.md).

Pour plus d’informations sur l’envoi d’un brouillon de message après sa mise à jour, consultez [la rubrique envoi de messages électroniques à l’aide de l’API managée EWS](#bk_sendewsma).

Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.

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

## <a name="update-email-messages-in-batches-by-using-ews"></a>Mettre à jour les messages électroniques par lots à l’aide d’EWS
<a name="bk_updateews"> </a>

Vous pouvez mettre à jour les messages électroniques par lots à l’aide de l’opération EWS de [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) , comme illustré dans l’exemple de code suivant. Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [mettre à jour les messages électroniques par lots](#bk_updateewsma).

Pour obtenir la liste des éléments de message électronique accessibles en écriture, consultez la rubrique [Propriétés et éléments de messagerie dans EWS dans Exchange](email-properties-and-elements-in-ews-in-exchange.md).

Pour plus d’informations sur l’envoi d’un brouillon de message après sa mise à jour, consultez la rubrique [Envoyer un brouillon de message électronique à l’aide d’EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).

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

Le serveur répond à la demande **UpdateItem** avec un message [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que chaque mise à jour a été enregistrée avec succès sur le serveur. Tous les conflits sont signalés dans l’élément [ConflictResult](https://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) .

## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a>Supprimer des messages électroniques par lots à l’aide de l’API managée EWS
<a name="bk_deleteewsma"> </a>

Vous pouvez supprimer des messages par lots à l’aide de la méthode [DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) de l’API managée EWS, comme le montre l’exemple suivant.

Cet exemple suppose que le **service** est un objet[ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a bien été authentifié pour un serveur Exchange.

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

## <a name="delete-email-messages-in-batches-by-using-ews"></a>Supprimer des messages électroniques par lots à l’aide d’EWS
<a name="bk_deleteews"> </a>

Vous pouvez supprimer des messages électroniques par lots à l’aide [de l’opération EWS EWS](../web-service-reference/deleteitem-operation.md) , comme illustré dans l’exemple de code suivant. Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [Supprimer les messages électroniques par lots](#bk_deleteewsma).

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

Le serveur répond à la demande **DeleteItem** avec un message [updateitemresponse](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) pour **chaque** élément supprimé. Notez que l’opération renvoie également Success si l’ID d’élément est introuvable.

## <a name="verifying-that-a-batch-process-completed-successfully"></a>Vérification de l’exécution réussie d’un processus de traitement par lots
<a name="bk_successful"> </a>

Lorsqu’un ou plusieurs messages électroniques dans une demande groupée ne peuvent pas être traités comme demandés, une erreur est renvoyée pour chaque message électronique ayant échoué et le reste des courriers électroniques dans le lot est traité comme prévu. Des défaillances dans le traitement par lots peuvent se produire si l’élément a été supprimé et, par conséquent, ne peut pas être envoyé, récupéré ou mis à jour, ou si l’élément a été déplacé vers un autre dossier, et par conséquent a un nouvel ID d’élément, et qu’il ne peut pas être modifié avec l’ID d’élément envoyé. Les informations contenues dans cette section indiquent comment obtenir des détails sur les échecs de traitement par lots de messages électroniques.

Pour vérifier la réussite d’un processus de traitement par lots à l’aide de l’API managée EWS, vous pouvez vérifier que la propriété [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) de l' [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) est égale à [ServiceResult. Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx). Si c’est le cas, tous les messages électroniques ont été traités avec succès. Si **OverallResult** n’est pas égal à **ServiceResult. Success**, un ou plusieurs messages électroniques n’ont pas été traités. Chacun des objets renvoyés dans l' **ServiceResponseCollection** contient les propriétés suivantes :

- [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)

- [ErrorDetails](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)

- [ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)

- [ErrorProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)

- [Résultat](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)

Ces propriétés contiennent des informations sur la raison pour laquelle les messages électroniques n’ont pas pu être traités comme demandé. Les exemples de cet article impriment les **résultats**, **ErrorCode**et **ErrorMessage** pour chaque message ayant échoué. Vous pouvez utiliser ces résultats pour examiner le problème.

Pour EWS, pour vérifier la réussite d’un processus par lot, vérifiez l’attribut [ResponseClass](https://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) pour chaque élément en cours de traitement. Voici la structure de base du **ResponseMessageType**, le type de base à partir duquel sont dérivés tous les messages de réponse.

```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

L’attribut **ResponseClass** est défini sur **Success** si le message électronique a été traité avec succès ou une **erreur** si le message n’a pas été traité correctement. Pour les messages électroniques, vous ne rencontrerez aucun **Avertissement** pendant le traitement par lots. Si **ResponseClass** **réussit**, l’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) qui suit est également toujours défini sur **NOERROR**. Si **ResponseClass** est une **erreur**, vous devez vérifier les valeurs des éléments [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**et [messagexml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) pour déterminer la cause du problème. [DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) n’est actuellement pas utilisé.

## <a name="see-also"></a>Voir aussi


- [Courrier électronique et les services EWS d'Exchange](email-and-ews-in-exchange.md)

- [Envoyer des messages électroniques à l’aide d’EWS dans Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)

- [Répondre à des messages électroniques à l’aide d’EWS dans Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)

- [Déplacer et copier des messages électroniques à l’aide d’EWS dans Exchange](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)

- [Implications de limitation pour les demandes de lots EWS](ews-throttling-in-exchange.md#throttling-implications-for-ews-batch-requests)
