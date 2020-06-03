---
title: Accéder aux contacts en tant que délégué à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3cd34c14-18b0-4fe2-a4c2-d884318c88fc
description: Découvrez comment accéder aux contacts en tant que délégué à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 06faf7dd7459b14792abbea21761e909c8eb9fb6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455344"
---
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a>Accéder aux contacts en tant que délégué à l’aide d’EWS dans Exchange

Découvrez comment accéder aux contacts en tant que délégué à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
Vous pouvez utiliser l’API managée EWS ou EWS pour donner à un utilisateur l’accès au dossier contacts d’un propriétaire de boîte aux lettres. Le délégué peut ensuite créer des contacts pour le compte du propriétaire de la boîte aux lettres et récupérer, mettre à jour et supprimer des contacts du dossier contacts du propriétaire de la boîte aux lettres, en fonction de leurs autorisations.
  
En tant que délégué, vous utilisez les mêmes méthodes et opérations pour accéder au dossier contacts d’un propriétaire de boîte aux lettres que vous utilisez pour accéder à votre propre dossier de contacts. La principale différence réside dans le fait que vous devez utiliser un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicit) pour rechercher ou créer un élément de contact, puis après avoir identifié l’ID de l’élément, vous pouvez utiliser l' [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) pour obtenir, mettre à jour ou supprimer l’élément. 
  
**Tableau 1. Méthodes de l’API managée EWS et opérations EWS pour accéder à un contact en tant que délégué**

|**Si vous souhaitez...**|**Utilisez cette méthode d’API managée EWS...**|**Utilisez cette opération EWS...**|
|:-----|:-----|:-----|
|Créer un contact en tant que délégué  <br/> |[Item. Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) où le paramètre [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier contacts du propriétaire de la boîte aux lettres  <br/> |[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) où l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie le [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres  <br/> |
|Créer plusieurs contacts en tant que délégué  <br/> |[ExchangeService. CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier contacts du propriétaire de la boîte aux lettres  <br/> |[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) où l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie le [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres  <br/> |
|Résoudre un contact en tant que délégué  <br/> |[ExchangeService. ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) où le paramètre [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier contacts du propriétaire de la boîte aux lettres  <br/> |[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) où l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie le [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres  <br/> |
|Rechercher ou Rechercher un contact en tant que délégué  <br/> |[ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier contacts du propriétaire de la boîte aux lettres  <br/> |[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) où l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie le [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres  <br/> |
|Obtenir un contact en tant que délégué  <br/> |[Contact. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Mettre à jour un contact en tant que délégué  <br/> |[Contact. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) suivi de [contact. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi de [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Supprimer un contact en tant que délégué  <br/> |[Contact. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) suivi de [contact. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , suivi de [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
> [!NOTE]
> Dans les exemples de code de cet article, primary@contoso.com est le propriétaire de la boîte aux lettres. 

<a name="bk_prereq"> </a>

## <a name="prerequisite-tasks"></a>Tâches préalables

Pour qu’un utilisateur puisse accéder au dossier contacts du propriétaire de la boîte aux lettres en tant que délégué, il doit être [ajouté en tant que délégué avec des autorisations](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) sur le dossier contacts du propriétaire de la boîte aux lettres. 

<a name="bk_createewsma"> </a>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a>Créer un contact en tant que délégué à l’aide de l’API managée EWS

L’API managée EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué afin de créer des contacts pour le propriétaire de la boîte aux lettres. Cet exemple montre comment utiliser la méthode [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) pour créer une réunion et envoyer des demandes de réunion aux participants. 
  
Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le délégué et que le délégué bénéficie des autorisations appropriées pour le dossier contacts du propriétaire de la boîte aux lettres. 
  
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

Notez que lorsque vous enregistrez l’élément, l’appel de la méthode [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) doit identifier le dossier contacts du propriétaire de la boîte aux lettres. Si le dossier contacts du propriétaire de la boîte aux lettres n’est pas spécifié, la demande de réunion est enregistrée dans le dossier contacts du délégué et non dans le dossier contacts du propriétaire de la boîte aux lettres. Vous pouvez inclure le dossier contacts du propriétaire de la boîte aux lettres dans l’appel de la méthode **Save** de manière bidirectionnelle. Nous vous recommandons d’instancier une nouvelle instance de l’objet [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) à l’aide de l' [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et de l’adresse SMTP du propriétaire de la boîte aux lettres. 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

Toutefois, vous pouvez également [établir une liaison](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) avec le dossier contacts, puis utiliser l’ID du dossier dans l’appel de la méthode **Save** . Toutefois, sachez que cela crée un appel EWS supplémentaire. 
  
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

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a>Créer un contact en tant que délégué à l’aide d’EWS

EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué afin de créer des éléments de contact pour le propriétaire de la boîte aux lettres. Cet exemple montre comment utiliser l’opération [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour créer un contact. 
  
Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez la méthode **Save** pour [créer un contact](#bk_createewsma).
  
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

Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui inclut la valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NOERROR**, ce qui indique que le contact a été créé avec succès. La réponse contient également l’ID de l’élément du contact qui vient d’être créé.

<a name="bk_resolveewsma"> </a>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a>Résoudre un contact en tant que délégué à l’aide de l’API managée EWS

Pour rechercher un contact en fonction d’un nom ou d’un terme éventuellement ambigu, vous devez utiliser l’une des méthodes [ExchangeService. ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) qui inclut un paramètre [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , afin que vous puissiez spécifier le dossier contacts du propriétaire de la boîte aux lettres. 
  
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

Une fois que l’appel de la méthode **ResolveNames** renvoie une réponse avec un ID, vous pouvez [obtenir, mettre à jour ou supprimer le contact](#bk_getewsma) à l’aide de l’ID et de l' [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit), &mdash; et vous n’avez pas besoin de spécifier l’adresse SMTP du propriétaire de la boîte aux lettres. 

<a name="bk_resolveews"> </a>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a>Résoudre un contact en tant que délégué à l’aide d’EWS

EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué afin de résoudre des noms partiels dans le dossier contacts du propriétaire de la boîte aux lettres. Cet exemple montre comment utiliser l’opération [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) pour rechercher des réunions dans le dossier contacts du propriétaire de la boîte aux lettres qui contient le mot « Johnson ». 
  
Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez la méthode **ResolveName** pour [résoudre un contact](#bk_resolveewsma).
  
```xml
 <?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Le serveur répond à la **demande ResolveNames** avec un message [ResolveNamesResponse](https://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que l’opération s’est terminée avec succès et qu’un seul résultat a été trouvé, ou **ErrorNameResolutionMultipleResults** si plusieurs résultats ont été trouvés, ce qui est indiqué dans le troisième exemple de code basé sur le contact [créer un contact en tant que délégué en utilisant l’API managée EWS](#bk_createewsma) La réponse contient également l' [ID ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de chaque résultat. 
  
La valeur de l’élément **ItemId** a été raccourcie pour des raisons de lisibilité. 
  
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
    <m:ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Maintenant que vous avez l' **ItemId** pour les contacts qui correspondent au nom ambigu, vous pouvez [obtenir, mettre à jour ou supprimer des éléments de contact en tant que délégué à l’aide d’EWS](#bk_getews) à l’aide de l' **ItemId** et de l' [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit), &mdash; et vous n’avez pas besoin de spécifier l’adresse SMTP du propriétaire de la boîte aux lettres. 

<a name="bk_getewsma"> </a>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a>Obtenir, mettre à jour ou supprimer des éléments de contact en tant que délégué à l’aide de l’API managée EWS

Vous pouvez utiliser l’API managée EWS pour obtenir, mettre à jour ou supprimer un contact de la même façon que vous effectuez ces actions lorsque vous n’utilisez pas l’accès délégué. La seule différence réside dans le fait que l’objet de service est destiné à l’utilisateur délégué. L’ID d’élément inclus dans l’appel de méthode de **liaison** identifie de manière unique l’élément dans la Banque de boîtes aux lettres, dans le dossier de contacts du propriétaire de la boîte aux lettres. 
  
**Tableau 2. Méthodes de l’API managée EWS utilisation d’un contact en tant que délégué**

|**Tâche**|**Méthode d'API managée EWS**|**Exemple de code**|
|:-----|:-----|:-----|
|Obtenir une ressource contact  <br/> |[Rattach](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[Obtention d’un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Mise à jour d'un contact  <br/> |[Liaison](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) suivie par la [mise à jour](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[Mise à jour d’un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|Supprimer un contact  <br/> |[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) suivi de [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[Suppression d’un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<a name="bk_getews"> </a>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a>Obtenir, mettre à jour ou supprimer des éléments de contact en tant que délégué à l’aide d’EWS

Vous pouvez utiliser EWS pour obtenir, mettre à jour ou supprimer un contact de réunion ou de rendez-vous de la même façon que vous effectuez ces actions lorsque vous n’utilisez pas l’accès délégué. La seule différence réside dans le fait que l’objet de service est destiné à l’utilisateur délégué. L’ID d’élément inclus dans la demande [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) identifie de manière unique l’élément dans la Banque de boîtes aux lettres, dans le dossier contacts du propriétaire de la boîte aux lettres. 
  
**Tableau 3. Opérations EWS pour travailler avec un contact en tant que délégué**

|**Task**|**Opération EWS**|**Exemple**|
|:-----|:-----|:-----|
|Obtenir une ressource contact  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Obtention d’un élément à l’aide d’EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Mise à jour d'un contact  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi de [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Mise à jour d’un élément à l’aide d’EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|Supprimer un contact  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , suivi de [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |[Suppression d’un élément à l’aide d’EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Accès délégué et EWS dans Exchange](delegate-access-and-ews-in-exchange.md)
- [Ajouter et supprimer des délégués à l’aide d’EWS dans Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [Définir les autorisations de dossier pour un autre utilisateur à l’aide d’EWS dans Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [Personnes et contacts dans EWS dans Exchange](people-and-contacts-in-ews-in-exchange.md)
- [Résoudre des noms ambigus à l’aide d’EWS dans Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

