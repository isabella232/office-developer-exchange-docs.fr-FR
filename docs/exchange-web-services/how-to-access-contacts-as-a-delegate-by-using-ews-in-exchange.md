---
title: Contacts Access en tant que délégué à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3cd34c14-18b0-4fe2-a4c2-d884318c88fc
description: Découvrez comment accéder aux contacts en tant que délégué à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: a7f695dcbe0693809817de84284294dff872aa9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754797"
---
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a>Contacts Access en tant que délégué à l’aide de EWS dans Exchange

Découvrez comment accéder aux contacts en tant que délégué à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Vous pouvez utiliser les API managées EWS pour donner à un utilisateur l’accès au dossier de Contacts d’un propriétaire de boîte aux lettres. Le délégué peut puis créer des contacts pour le compte du propriétaire de boîte aux lettres, extraire, mettre à jour et supprimer des contacts à partir du dossier de Contacts du propriétaire de la boîte aux lettres, en fonction de leurs autorisations.
  
En tant que délégué, vous utilisez les mêmes méthodes et opérations pour accéder au dossier Contacts d’un propriétaire de boîte aux lettres que vous utilisez pour accéder à votre propre dossier Contacts. La principale différence est que vous devez utiliser [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicit) pour trouver ou créer un élément de contact, puis après avoir identifié l’ID d’élément, vous pouvez utiliser [un accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) pour obtenir, de mettre à jour ou de supprimer l’élément. 
  
**Le tableau 1. Méthodes d’API managées et opérations EWS pour accéder à un contact en tant que délégué**

|**Si vous souhaitez...**|**Utilisez cette méthode d’API managées...**|**Utilisez cette opération EWS...**|
|:-----|:-----|:-----|
|Créer un contact en tant que délégué  <br/> |[Item.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) où le paramètre [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de Contacts du propriétaire de la boîte aux lettres  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres  <br/> |
|Créer plusieurs contacts en tant que délégué  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de Contacts du propriétaire de la boîte aux lettres  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres  <br/> |
|Résoudre un contact en tant que délégué  <br/> |[ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) où le paramètre [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de Contacts du propriétaire de la boîte aux lettres  <br/> |[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres  <br/> |
|Recherchez ou rechercher un contact en tant que délégué  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de Contacts du propriétaire de la boîte aux lettres  <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres  <br/> |
|Obtenir un contact en tant que délégué  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Mise à jour d’un contact en tant que délégué  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) suivi [Contact.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Supprimer un contact en tant que délégué  <br/> |[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) suivi [Contact.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
> [!NOTE]
> Dans les exemples de code dans cet article, primary@contoso.com est le propriétaire de boîte aux lettres. 

<a name="bk_prereq"> </a>

## <a name="prerequisite-tasks"></a>Les tâches préalables

Qu’un utilisateur puisse accéder dossier de Contacts du propriétaire de la boîte aux lettres en tant que délégué, l’utilisateur doit être [ajouté en tant que délégué disposant des autorisations](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) au dossier de Contacts du propriétaire de la boîte aux lettres. 

<a name="bk_createewsma"> </a>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a>Créer un contact en tant que délégué à l’aide de l’API managée EWS

L’API managée EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour créer des contacts pour le propriétaire de boîte aux lettres. Cet exemple montre comment utiliser la méthode [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) pour créer une réunion et envoyer les demandes de réunion aux participants. 
  
Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le délégué et le délégué a été accordé les autorisations appropriées pour le dossier de Contacts du propriétaire de la boîte aux lettres. 
  
```cs
 public static void DelegateAccessCreateContact(ExchangeService service)
{
    // Create the contact.
    Contact contact = new Contact(service);
    // Specify the name and how the contact should be filed.
    contact.GivenName = "Brian";
    contact.MiddleName = "David";
    contact.Surname = "Johnson";
    contact.FileAsMapping = FileAsMapping.SurnameCommaGivenName;
    // Specify the company name.
    contact.CompanyName = "Contoso";
    // Specify the business, home, and car phone numbers.
    contact.PhoneNumbers[PhoneNumberKey.BusinessPhone] = "425-555-0110";
    contact.PhoneNumbers[PhoneNumberKey.HomePhone] = "425-555-0120";
    contact.PhoneNumbers[PhoneNumberKey.CarPhone] = "425-555-0130";
    // Specify two email addresses.
    contact.EmailAddresses[EmailAddressKey.EmailAddress1] = 
        new EmailAddress("brian_1@contoso.com");
    contact.EmailAddresses[EmailAddressKey.EmailAddress2] = 
        new EmailAddress("brian_2@contoso.com");
    // Save the contact in the mailbox owner's Contacts folder.
    // This method call results in a CreateItem call to EWS. 
    // The contact identifier contains the context for the mailbox owner's 
    // Contact folder. Any additional actions take on this contact will 
    // be performed in the mailbox owner's mailbox. 
    contact.Save(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    // Verify that the contact was created.
    // This method call results in a GetItem call to EWS
    // to load the display name property on the contact. 
    contact.Load(new PropertySet (ContactSchema.DisplayName));
    Console.WriteLine("\nContact created: " + contact.DisplayName + "\n");
}
```

Notez que lorsque vous enregistrez l’élément, l’appel de méthode [Enregistrer](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) doit identifier le dossier de Contacts du propriétaire de la boîte aux lettres. Si le dossier de Contacts du propriétaire de la boîte aux lettres n’est pas spécifié, la demande de réunion est enregistrée pour le dossier du délégué Contacts et non le dossier de Contacts du propriétaire de la boîte aux lettres. Vous pouvez inclure le dossier de Contacts du propriétaire de la boîte aux lettres dans l’appel de méthode **Enregistrer** de manière deux. Il est recommandé que vous instanciez une nouvelle instance de l’objet [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) à l’aide de la [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et l’adresse SMTP du propriétaire de boîte aux lettres. 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

Toutefois, vous pouvez également [lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) au dossier Contacts tout d’abord, puis utilisez l’ID du dossier de l’appel de méthode **Enregistrer** . Sachez, toutefois, que cette opération crée un appel EWS supplémentaire. 
  
```cs
    // Identify the mailbox owner's SMTP address 
    // and bind to their Contacts folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryContacts = Folder.Bind(service, new FolderId(WellKnownFolderName.Contacts, primary)); 
…
    // Save the contact to the mailbox owner's Contacts folder.
    meeting.Save(primaryContacts.Id);
```

<a name="bk_createews"> </a>

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a>Créer un contact en tant que délégué à l’aide de EWS

EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour créer des éléments de contact pour le propriétaire de la boîte aux lettres. Cet exemple montre comment utiliser l’opération [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour créer un contact. 
  
C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **Save** pour [créer un contact](#bk_createewsma).
  
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
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Contact>
          <t:FileAsMapping>LastCommaFirst</t:FileAsMapping>
          <t:GivenName>Brian</t:GivenName>
          <t:MiddleName>David</t:MiddleName>
          <t:CompanyName>Contoso</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">brian_1@contoso.com</t:Entry>
            <t:Entry Key="EmailAddress2">brian_2@contoso.com</t:Entry>
          </t:EmailAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">425-555-0110</t:Entry>
            <t:Entry Key="HomePhone">425-555-0120</t:Entry>
            <t:Entry Key="CarPhone">425-555-0130</t:Entry>
          </t:PhoneNumbers>
          <t:Surname>Johnson</t:Surname>
        </t:Contact>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le contact a été créé avec succès. La réponse contient également l’ID d’élément de contact nouvellement créé.

<a name="bk_resolveewsma"> </a>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a>Résoudre un contact en tant que délégué à l’aide de l’API managée EWS

Pour rechercher un contact basé sur un nom ambigu éventuellement ou un terme, vous devez utiliser une des méthodes [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) qui comprend un paramètre [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , afin que vous pouvez spécifier le dossier de Contacts du propriétaire de la boîte aux lettres. 
  
```cs
private static void DelegateAccessResolveContacts(ExchangeService service)
{
    // Create a list to store folders to search.
    List<FolderId> folders = new List<FolderId>();
   
    // Add the mailbox owner's folder to the list.
    folders.Add(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    
    // Resolve the ambiguous name "Johnson".
    // This method call results in a ResolveNames call to EWS.
    NameResolutionCollection resolvedNames = service.ResolveName(
        "johnson", folders, ResolveNameSearchLocation.ContactsOnly, true);
    // Output the list of candidate email addresses and contact names.
    foreach (NameResolution nameRes in resolvedNames)
    {
        Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
        Console.WriteLine("Contact ID: " + nameRes.Mailbox.Id);
    }
}
```

Une fois que l’appel de méthode **ResolveNames** retourne une réponse avec un ID, vous pouvez [obtenir, de mettre à jour ou de supprimer le contact](#bk_getewsma) à l’aide de l’ID et [l’accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;et vous n’avez pas besoin de spécifier l’adresse SMTP de l’utilisateur de boîte aux lettres. 

<a name="bk_resolveews"> </a>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a>Résoudre un contact en tant que délégué à l’aide de EWS

EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour résoudre les noms partiels dans le dossier de Contacts du propriétaire de la boîte aux lettres. Cet exemple montre comment utiliser l’opération [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) pour rechercher des réunions dans le dossier Contacts du propriétaire de la boîte aux lettres qui contiennent le mot « johnson ». 
  
C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **ResolveName** pour [résoudre un contact](#bk_resolveewsma).
  
```xml
 <?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ResolveNames ReturnFullContactData="true"
                    SearchScope="Contacts">
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
      <m:UnresolvedEntry>johnson</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **ResolveNames** avec un message [ResolveNamesResponse](http://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, qui indique que l’opération terminée avec succès et trouvé une seule résultat, ou **ErrorNameResolutionMultipleResults** si plusieurs résultats trouvés - qui correspond à ce qui est affiché dans le troisième exemple de code basé sur le contact [créer un contact en tant que délégué à l’aide de l’API managée EWS](#bk_createewsma). La réponse contient également l' [ID d’élément](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de chaque résultat. 
  
La valeur de l’élément **ItemId** a été raccourcie pour des raisons de lisibilité. 
  
```XML
 <?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Warning">
          <m:MessageText>Multiple results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionMultipleResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:ResolutionSet TotalItemsInView="2"
                           IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_1@contoso.com</t:Name>
                <t:EmailAddress>brian_1@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_2@contoso.com</t:Name>
                <t:EmailAddress>brian_2@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>
```

Maintenant que vous disposez de l' **ID d’élément** pour les contacts qui correspondent au nom ambigu, vous pouvez [obtenir, mettre à jour ou supprimer des éléments de contact en tant que délégué à l’aide de EWS](#bk_getews) à l’aide de **l’ItemId** et [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;et vous n’avez pas besoin de spécifier adresse SMTP de l’utilisateur de boîte aux lettres. 

<a name="bk_getewsma"> </a>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a>Obtenir, mettre à jour ou supprimer des éléments de contact en tant que délégué à l’aide de l’API managée EWS

Vous pouvez utiliser l’API managée EWS pour obtenir, mettre à jour ou supprimer un contact de la même manière que vous effectuez ces actions lorsque vous n’utilisez pas d’accès délégué. La seule différence est que l’objet de service pour l’utilisateur délégué. L’ID d’élément inclus dans l’appel de méthode **lier** unique identifie l’élément dans le magasin de boîte aux lettres, dans le dossier de Contacts du propriétaire de la boîte aux lettres. 
  
**Le tableau 2. Méthodes d’API managées fonctionne avec un contact en tant que délégué**

|**Tâche**|**Méthode d'API managée EWS**|**Exemple de code**|
|:-----|:-----|:-----|
|Obtenir un contact  <br/> |[Créer une liaison](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[Obtenir un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Mettre à jour un contact  <br/> |[Lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) le suivi de [mise à jour](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[Mettre à jour un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|Supprimer un contact  <br/> |[Lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) suivie à [Supprimer](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[Supprimer un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<a name="bk_getews"> </a>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a>Obtenir, mettre à jour ou supprimer des éléments de contact en tant que délégué à l’aide de EWS

Vous pouvez utiliser EWS pour obtenir, mettre à jour ou supprimer un contact de réunion ou un rendez-vous de la même manière que vous effectuez ces actions lorsque vous n’utilisez pas d’accès délégué. La seule différence est que l’objet de service pour l’utilisateur délégué. L’ID d’élément inclus dans la demande de [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) unique identifie l’élément dans le magasin de boîte aux lettres, dans le dossier de Contacts du propriétaire de la boîte aux lettres. 
  
**Le tableau 3. Opérations EWS pour travailler avec un contact en tant que délégué**

|**Tâche**|**Opération EWS**|**Exemple**|
|:-----|:-----|:-----|
|Obtenir un contact  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Obtenir un élément à l’aide de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Mettre à jour un contact  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Mettre à jour un élément à l’aide de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|Supprimer un contact  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |[Supprimer un élément à l’aide de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Accès délégué et EWS dans Exchange](delegate-access-and-ews-in-exchange.md)
- [Ajouter et supprimer des délégués à l’aide de EWS dans Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [Définir des autorisations de dossier pour un autre utilisateur à l’aide de EWS dans Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [Personnes et contacts dans EWS dans Exchange](people-and-contacts-in-ews-in-exchange.md)
- [Résoudre des noms ambigus en utilisant EWS dans Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

