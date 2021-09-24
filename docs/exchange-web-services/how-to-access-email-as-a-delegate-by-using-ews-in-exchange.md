---
title: Accéder à la messagerie en tant que délégué à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: a8123604-c7c0-405d-a0ed-7a9b4a431bfd
description: Découvrez comment accéder à la messagerie en tant que délégué à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: aa921bc36004b3a26caa514390e52249021b304f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521213"
---
# <a name="access-email-as-a-delegate-by-using-ews-in-exchange"></a>Accéder à la messagerie en tant que délégué à l’aide d’EWS dans Exchange

Découvrez comment accéder à la messagerie en tant que délégué à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
  
Vous pouvez utiliser l’API gérée EWS ou EWS pour accorder à un utilisateur un accès délégué au dossier boîte de réception d’un propriétaire de boîte aux lettres. Le délégué peut ensuite créer des demandes de réunion pour le compte du propriétaire de la boîte aux lettres, rechercher des courriers électroniques et récupérer, mettre à jour et supprimer des messages électroniques à partir du dossier boîte de réception du propriétaire de la boîte aux lettres, en fonction de leurs autorisations.
  
En tant que délégué, vous utilisez les mêmes méthodes et opérations pour accéder au dossier Boîte de réception d’un propriétaire de boîte aux lettres que pour accéder à un dossier boîte de réception sans accès délégué. La principale différence est que [](delegate-access-and-ews-in-exchange.md#bk_explicit) vous devez utiliser un accès explicite pour rechercher ou créer un [](delegate-access-and-ews-in-exchange.md#bk_implicit) élément de courrier, puis après avoir identifié l’ID de l’élément, vous pouvez utiliser l’accès implicite pour obtenir, mettre à jour ou supprimer l’élément. 
  
**Tableau 1. Méthodes d’API gérées EWS et opérations EWS pour accéder à la messagerie en tant que délégué**

|**Si vous souhaitez...**|**Utilisez cette méthode d’API gérée EWS...**|**Utilisez cette opération EWS...**|
|:-----|:-----|:-----|
|Créer et envoyer un e-mail en tant que délégué  <br/> |[EmailMessage.Save où](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) le paramètre [](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit un accès explicite au dossier Brouillons du propriétaire de la boîte aux lettres  <br/> [EmailMessage.SendAndSaveCopy](https://msdn.microsoft.com/library/dd634248%28v=exchg.80%29.aspx) où le paramètre [](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit un accès explicite au dossier Éléments envoyés du propriétaire de la boîte aux lettres  <br/> |[CreateItem où](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie la [propriété EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres  <br/> [SendItem où](https://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie la [propriété EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres  <br/> |
|Créer plusieurs messages électroniques en tant que délégué  <br/> |[ExchangeService.CreateItems où](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) le paramètre [](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) **FolderId** fournit un accès explicite au dossier boîte de réception du propriétaire de la boîte aux lettres  <br/> |[CreateItem où](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie la [propriété EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres  <br/> |
|Rechercher ou rechercher un e-mail en tant que délégué  <br/> |[ExchangeService.FindItems où](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) le paramètre [](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) **FolderId** fournit un accès explicite au dossier boîte de réception du propriétaire de la boîte aux lettres  <br/> |[FindItem où](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie la [propriété EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres  <br/> |
|Obtenir un e-mail en tant que délégué  <br/> |[EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Mettre à jour un e-mail en tant que délégué  <br/> |[EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) suivi de [EmailMessage.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[GetItem suivi](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) de [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Supprimer un e-mail en tant que délégué  <br/> |[EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) suivi de [EmailMessage.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi de [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
Gardez les points suivants à l’esprit lorsque vous travaillez avec des e-mails en tant que délégué :
  
- Si un délégué doit uniquement travailler avec les demandes de réunion et les réponses, il n’a pas besoin d’accéder au dossier Boîte de réception. Pour plus d’informations, voir [les tâches prérequises pour accéder aux calendriers en tant que délégué.](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq)
    
- Lorsqu’un destinataire reçoit un message qui a été envoyé au nom  d’un propriétaire de boîte aux lettres, l’expéditeur apparaît comme « Délégué de la part du propriétaire de la *boîte aux lettres* ». 
    
> [!NOTE]
> Dans les exemples de code de cet article, primary@contoso.com est le propriétaire de la boîte aux lettres. 
  
## <a name="prerequisite-tasks"></a>Tâches prérequises
<a name="bk_prereq"> </a>

Pour qu’un utilisateur puisse accéder au dossier Boîte de réception du propriétaire de la boîte aux lettres en tant que délégué, il doit être ajouté en tant que délégué avec les [autorisations](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) d’accès au dossier Boîte de réception du propriétaire de la boîte aux lettres. 
  
## <a name="create-and-send-an-email-as-a-delegate-by-using-the-ews-managed-api"></a>Créer et envoyer un courrier électronique en tant que délégué à l’aide de l’API gérée EWS
<a name="bk_createewsma"> </a>

L’API gérée EWS vous permet d’utiliser l’objet service pour que l’utilisateur délégué crée et envoie des messages au nom du propriétaire de la boîte aux lettres. Cet exemple montre comment utiliser la méthode [Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) pour enregistrer le message dans le dossier Brouillons du propriétaire de la boîte aux lettres, puis la méthode [SendAndSaveCopy](https://msdn.microsoft.com/library/dd634248%28v=exchg.80%29.aspx) pour envoyer le message et l’enregistrer dans le dossier Éléments envoyés du propriétaire de la boîte aux lettres. 
  
Cet exemple suppose que **le service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le délégué et que le délégué a reçu les autorisations appropriées pour la boîte de réception, les brouillons et le dossier Éléments envoyés du propriétaire de la boîte aux [lettres.](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
  
```cs
public static void DelegateAccessCreateEmail(ExchangeService service)
{
    // Create an email message and provide it with connection 
    // configuration information by using an ExchangeService 
    // object named service.
    EmailMessage message = new EmailMessage(service);
    // Set properties on the email message.
    message.Subject = "Company Soccer Team";
    message.Body = "Are you interested in joining?";
    message.ToRecipients.Add("sadie@contoso.com");
    // Save the email to the mailbox owner's Drafts folder.
    // This method call results in a CreateItem call to EWS.
    // The FolderId parameter contains the context for the 
    // mailbox owner's Inbox folder. Any additional actions 
    // taken on this message will be performed in the mailbox 
    // owner's mailbox. 
    message.Save(new FolderId(WellKnownFolderName.Drafts, new Mailbox("primary@contoso.com")));
    // Send the email and save the message in the mailbox owner's 
    // Sent Items folder.
    // This method call results in a SendItem call to EWS.
    message.SendAndSaveCopy(new FolderId(WellKnownFolderName.SentItems, new Mailbox("primary@contoso.com")));
    Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" 
    + message.ToRecipients[0] + "' and saved in the Sent Items folder of the mailbox owner.");
}
```

## <a name="create-and-send-an-email-as-a-delegate-by-using-ews"></a>Créer et envoyer un courrier électronique en tant que délégué à l’aide d’EWS
<a name="bk_createews"> </a>

EWS vous permet d’utiliser l’objet de service pour que l’utilisateur délégué crée et envoie des messages au nom du propriétaire de la boîte aux lettres. Cet exemple montre comment utiliser l’opération [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour créer un message électronique et l’opération [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) pour envoyer le temps et l’enregistrer dans le dossier Éléments envoyés du propriétaire de la boîte aux lettres. 
  
Il s’agit également de la première demande XML que l’API gérée EWS envoie lorsque vous utilisez la méthode **Save** pour créer et [envoyer un e-mail.](#bk_createewsma)
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, qui indique que le message a été créé et enregistré avec succès. La réponse contient également l’ID d’élément du message électronique nouvellement créé.
  
La **valeur ItemId** a été raccourcie pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="iNRaAAA="
                        ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
            </t:Message>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

Ensuite, utilisez **l’opération SendItem** pour envoyer le message au nom du propriétaire de la boîte aux lettres et l’enregistrer dans le dossier Éléments envoyés du propriétaire de la boîte aux lettres. 
  
La **valeur ItemId** a été raccourcie pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="iNRaAAA="
                  ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **SendItem** avec un message [SendItemResponse](https://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError,** qui indique que le message a été envoyé et enregistré dans le dossier Éléments envoyés du propriétaire de la boîte aux lettres.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </m:SendItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="search-for-an-email-as-a-delegate-by-using-the-ews-managed-api"></a>Rechercher un e-mail en tant que délégué à l’aide de l’API gérée EWS
<a name="bk_searchewsma"> </a>

Pour rechercher un e-mail, vous devez utiliser l’une des méthodes [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) qui inclut un paramètre [FolderId,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) afin de pouvoir spécifier le dossier boîte de réception du propriétaire de la boîte de réception. 
  
```cs
static void DelegateAccessSearchEmailWithFilter(ExchangeService service)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    // Define the search filter.
    SearchFilter.ContainsSubstring filter = new SearchFilter.ContainsSubstring(ItemSchema.Subject, 
        "soccer", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Call FindItems to find matching Inbox items. 
        // The parameters of FindItems must denote the mailbox owner,
        // mailbox, and Inbox folder.
        // This call results in a FindItem call to EWS.
        FindItemsResults<Item> results = service.FindItems(new 
            FolderId(WellKnownFolderName.Inbox, "primary@contoso.com"), 
            filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

Une fois que l’appel **FindItems** renvoie une réponse avec un ID, vous pouvez obtenir, mettre à jour ou supprimer ce courrier électronique à l’aide de l’ID et de l’accès [implicite,](delegate-access-and-ews-in-exchange.md#bk_implicit) et vous n’avez pas besoin de spécifier l’adresse SMTP du propriétaire de la boîte aux lettres. 
  
## <a name="search-for-an-email-as-a-delegate-by-using-ews"></a>Rechercher un e-mail en tant que délégué à l’aide d’EWS
<a name="bk_searchews"> </a>

EWS vous permet d’utiliser l’objet de service pour que l’utilisateur délégué recherche des courriers électroniques qui répondent à un ensemble de critères de recherche. Cet exemple montre comment utiliser l’opération [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour rechercher des messages dans le dossier boîte de réception du propriétaire qui contiennent le mot « domaine » dans l’objet. 
  
Il s’agit également de la demande XML que l’API gérée EWS envoie lorsque vous [recherchez un e-mail.](#bk_searchewsma)
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:Restriction>
        <t:Contains ContainmentMode="Substring"
                    ContainmentComparison="IgnoreCase">
          <t:FieldURI FieldURI="item:Subject" />
          <t:Constant Value="soccer" />
        </t:Contains>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **FindItem** avec un message [FindItemResponse](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError,** ce qui indique que la recherche s’est terminée correctement. La réponse contient un [élément Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) pour tous les messages électroniques qui répondaient aux critères de recherche. Dans ce cas, un seul e-mail est trouvé. 
  
La valeur de [l’élément ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) a été raccourcie pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1"
                        TotalItemsInView="1"
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="iNwoAAA="
                          ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQuu" />
                <t:Subject>Soccer team</t:Subject>
                <t:DateTimeReceived>2014-03-10T06:16:55Z</t:DateTimeReceived>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

Maintenant que vous avez **l’ItemId** pour le courrier électronique qui répond à vos critères, vous pouvez obtenir, mettre à jour ou supprimer ce courrier électronique à l’aide de **l’ItemId** et de l’accès [implicite,](delegate-access-and-ews-in-exchange.md#bk_implicit) et vous n’avez pas besoin de spécifier l’adresse SMTP du propriétaire de la boîte aux lettres. 
  
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-the-ews-managed-api"></a>Obtenir, mettre à jour ou supprimer des éléments de courrier en tant que délégué à l’aide de l’API gérée EWS
<a name="bk_geteswma"> </a>

Vous pouvez utiliser l’API gérée EWS pour obtenir, mettre à jour ou supprimer un e-mail de la même manière que lorsque vous n’utilisez pas l’accès délégué. La seule différence est que **l’objet ExchangeService** est pour l’utilisateur délégué. L’ID d’élément inclus dans l’appel de la méthode **Bind** identifie de manière unique l’élément dans la boîte aux lettres, dans le dossier boîte de réception du propriétaire de la boîte de réception. 
  
**Tableau 2. Méthodes d’API gérées EWS avec la messagerie en tant que délégué**

|**Tâche**|**Méthode d'API managée EWS**|**Exemple de code**|
|:-----|:-----|:-----|
|Obtenir un e-mail  <br/> |[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[Obtention d’un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Mettre à jour un e-mail  <br/> |[Liaison](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) suivie de la mise [à jour](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[Mise à jour d’un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|Supprimer un e-mail  <br/> |[Liaison](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) suivie de [la suppression](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx) <br/> |[Suppression d’un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |
   
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-ews"></a>Obtenir, mettre à jour ou supprimer des éléments de courrier en tant que délégué à l’aide d’EWS
<a name="bk_getews"> </a>

Vous pouvez utiliser l’API gérée EWS pour obtenir, mettre à jour ou supprimer un e-mail de la même manière que lorsque vous n’utilisez pas l’accès délégué. La seule différence est que l’objet service est pour l’utilisateur délégué. L’ID d’élément inclus dans la demande **GetItem** identifie de manière unique l’élément dans la boîte aux lettres, dans le dossier boîte de réception du propriétaire de la boîte de réception. 
  
**Tableau 3. Opérations EWS pour travailler avec le courrier électronique en tant que délégué**

|**Tâche**|**Opération EWS**|**Exemple de code**|
|:-----|:-----|:-----|
|Obtenir un e-mail  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Obtention d’un élément à l’aide d’EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Mettre à jour un e-mail  <br/> |[GetItem suivi](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) de [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Mise à jour d’un élément à l’aide d’EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|Supprimer un e-mail  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi de [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |[Suppression d’un élément à l’aide d’EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Accès délégué et EWS dans Exchange](delegate-access-and-ews-in-exchange.md)    
- [Ajouter et supprimer des délégués à l’aide d’EWS dans Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Définir des autorisations de dossier pour un autre utilisateur à l’aide d’EWS dans Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)    
- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
    

