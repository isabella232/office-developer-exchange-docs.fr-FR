---
title: Contacts Access en tant que délégué à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3cd34c14-18b0-4fe2-a4c2-d884318c88fc
description: Découvrez comment accéder aux contacts en tant que délégué à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 47540082f7e60645cae60fe2347e50e17cd226dd
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353720"
---
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="45929-103">Contacts Access en tant que délégué à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="45929-103">Access contacts as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="45929-104">Découvrez comment accéder aux contacts en tant que délégué à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="45929-104">Learn how to access contacts as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="45929-105">Vous pouvez utiliser les API managées EWS pour donner à un utilisateur l’accès au dossier de Contacts d’un propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-105">You can use the EWS Managed API or EWS to give a user access to a mailbox owner's Contacts folder.</span></span> <span data-ttu-id="45929-106">Le délégué peut puis créer des contacts pour le compte du propriétaire de boîte aux lettres, extraire, mettre à jour et supprimer des contacts à partir du dossier de Contacts du propriétaire de la boîte aux lettres, en fonction de leurs autorisations.</span><span class="sxs-lookup"><span data-stu-id="45929-106">The delegate can then create contacts on behalf of the mailbox owner, and retrieve, update, and delete contacts from the mailbox owner's Contacts folder, depending on their permissions.</span></span>
  
<span data-ttu-id="45929-107">En tant que délégué, vous utilisez les mêmes méthodes et opérations pour accéder au dossier Contacts d’un propriétaire de boîte aux lettres que vous utilisez pour accéder à votre propre dossier Contacts.</span><span class="sxs-lookup"><span data-stu-id="45929-107">As a delegate, you use the same methods and operations to access a mailbox owner's Contacts folder that you use to access your own Contacts folder.</span></span> <span data-ttu-id="45929-108">La principale différence est que vous devez utiliser [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicit) pour trouver ou créer un élément de contact, puis après avoir identifié l’ID d’élément, vous pouvez utiliser [un accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) pour obtenir, de mettre à jour ou de supprimer l’élément.</span><span class="sxs-lookup"><span data-stu-id="45929-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a contact item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="45929-109">**Le tableau 1. Méthodes d’API managées et opérations EWS pour accéder à un contact en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="45929-109">**Table 1. EWS Managed API methods and EWS operations for accessing a contact as a delegate**</span></span>

|<span data-ttu-id="45929-110">**Si vous souhaitez...**</span><span class="sxs-lookup"><span data-stu-id="45929-110">**If you want to…**</span></span>|<span data-ttu-id="45929-111">**Utilisez cette méthode d’API managées...**</span><span class="sxs-lookup"><span data-stu-id="45929-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="45929-112">**Utilisez cette opération EWS...**</span><span class="sxs-lookup"><span data-stu-id="45929-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="45929-113">Créer un contact en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="45929-113">Create a contact as a delegate</span></span>  <br/> |<span data-ttu-id="45929-114">[Item.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) où le paramètre [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de Contacts du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="45929-114">[Item.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="45929-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="45929-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="45929-116">Créer plusieurs contacts en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="45929-116">Create multiple contacts as a delegate</span></span>  <br/> |<span data-ttu-id="45929-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de Contacts du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="45929-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="45929-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="45929-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="45929-119">Résoudre un contact en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="45929-119">Resolve a contact as a delegate</span></span>  <br/> |<span data-ttu-id="45929-120">[ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) où le paramètre [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de Contacts du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="45929-120">[ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="45929-121">[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="45929-121">[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="45929-122">Recherchez ou rechercher un contact en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="45929-122">Search for or find a contact as a delegate</span></span>  <br/> |<span data-ttu-id="45929-123">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de Contacts du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="45929-123">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="45929-124">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="45929-124">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="45929-125">Obtenir un contact en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="45929-125">Get a contact as a delegate</span></span>  <br/> |[<span data-ttu-id="45929-126">Contact.Bind</span><span class="sxs-lookup"><span data-stu-id="45929-126">Contact.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="45929-127">GetItem</span><span class="sxs-lookup"><span data-stu-id="45929-127">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="45929-128">Mise à jour d’un contact en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="45929-128">Update a contact as a delegate</span></span>  <br/> |<span data-ttu-id="45929-129">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) suivi [Contact.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="45929-129">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="45929-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="45929-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="45929-131">Supprimer un contact en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="45929-131">Delete a contact as a delegate</span></span>  <br/> |<span data-ttu-id="45929-132">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) suivi [Contact.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="45929-132">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="45929-133">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="45929-133">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="45929-134">Dans les exemples de code dans cet article, primary@contoso.com est le propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-134">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 

<span data-ttu-id="45929-135"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="45929-135"></span></span>

## <a name="prerequisite-tasks"></a><span data-ttu-id="45929-136">Les tâches préalables</span><span class="sxs-lookup"><span data-stu-id="45929-136">Prerequisite tasks</span></span>

<span data-ttu-id="45929-137">Qu’un utilisateur puisse accéder dossier de Contacts du propriétaire de la boîte aux lettres en tant que délégué, l’utilisateur doit être [ajouté en tant que délégué disposant des autorisations](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) au dossier de Contacts du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-137">Before a user can access the mailbox owner's Contacts folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Contacts folder.</span></span> 

<span data-ttu-id="45929-138"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="45929-138"></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="45929-139">Créer un contact en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="45929-139">Create a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="45929-140">L’API managée EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour créer des contacts pour le propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-140">The EWS Managed API enables you to use the service object for the delegate user to create contacts for the mailbox owner.</span></span> <span data-ttu-id="45929-141">Cet exemple montre comment utiliser la méthode [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) pour créer une réunion et envoyer les demandes de réunion aux participants.</span><span class="sxs-lookup"><span data-stu-id="45929-141">This example shows how to use the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="45929-142">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le délégué et le délégué a été accordé les autorisations appropriées pour le dossier de Contacts du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-142">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Contacts folder.</span></span> 
  
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

<span data-ttu-id="45929-143">Notez que lorsque vous enregistrez l’élément, l’appel de méthode [Enregistrer](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) doit identifier le dossier de Contacts du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-143">Note that when you save the item, the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="45929-144">Si le dossier de Contacts du propriétaire de la boîte aux lettres n’est pas spécifié, la demande de réunion est enregistrée pour le dossier du délégué Contacts et non le dossier de Contacts du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-144">If the mailbox owner's Contacts folder is not specified, the meeting request gets saved to the delegate's Contacts folder and not the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="45929-145">Vous pouvez inclure le dossier de Contacts du propriétaire de la boîte aux lettres dans l’appel de méthode **Enregistrer** de manière deux.</span><span class="sxs-lookup"><span data-stu-id="45929-145">You can include the mailbox owner's Contacts folder in the **Save** method call in two way.</span></span> <span data-ttu-id="45929-146">Il est recommandé que vous instanciez une nouvelle instance de l’objet [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) à l’aide de la [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et l’adresse SMTP du propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-146">We recommend that you instantiate a new instance of the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

<span data-ttu-id="45929-147">Toutefois, vous pouvez également [lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) au dossier Contacts tout d’abord, puis utilisez l’ID du dossier de l’appel de méthode **Enregistrer** .</span><span class="sxs-lookup"><span data-stu-id="45929-147">However, you can also [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Contacts folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="45929-148">Sachez, toutefois, que cette opération crée un appel EWS supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="45929-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
```cs
    // Identify the mailbox owner's SMTP address 
    // and bind to their Contacts folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryContacts = Folder.Bind(service, new FolderId(WellKnownFolderName.Contacts, primary)); 
…
    // Save the contact to the mailbox owner's Contacts folder.
    meeting.Save(primaryContacts.Id);
```

<span data-ttu-id="45929-149"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="45929-149"></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="45929-150">Créer un contact en tant que délégué à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="45929-150">Create a contact as a delegate by using EWS</span></span>

<span data-ttu-id="45929-151">EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour créer des éléments de contact pour le propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-151">EWS enables you to use the service object for the delegate user to create contact items for the mailbox owner.</span></span> <span data-ttu-id="45929-152">Cet exemple montre comment utiliser l’opération [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour créer un contact.</span><span class="sxs-lookup"><span data-stu-id="45929-152">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a contact.</span></span> 
  
<span data-ttu-id="45929-153">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **Save** pour [créer un contact](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="45929-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a contact](#bk_createewsma).</span></span>
  
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

<span data-ttu-id="45929-154">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le contact a été créé avec succès.</span><span class="sxs-lookup"><span data-stu-id="45929-154">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the contact was created successfully.</span></span> <span data-ttu-id="45929-155">La réponse contient également l’ID d’élément de contact nouvellement créé.</span><span class="sxs-lookup"><span data-stu-id="45929-155">The response also contains the item ID of the newly created contact.</span></span>

<span data-ttu-id="45929-156"><a name="bk_resolveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="45929-156"></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="45929-157">Résoudre un contact en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="45929-157">Resolve a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="45929-158">Pour rechercher un contact basé sur un nom ambigu éventuellement ou un terme, vous devez utiliser une des méthodes [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) qui comprend un paramètre [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , afin que vous pouvez spécifier le dossier de Contacts du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-158">To find a contact based on a possibly ambiguous name or term, you must use one of the [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Contacts folder.</span></span> 
  
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

<span data-ttu-id="45929-159">Une fois que l’appel de méthode **ResolveNames** retourne une réponse avec un ID, vous pouvez [obtenir, de mettre à jour ou de supprimer le contact](#bk_getewsma) à l’aide de l’ID et [l’accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;et vous n’avez pas besoin de spécifier l’adresse SMTP de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-159">After the **ResolveNames** method call returns a response with an ID, you can [get, update or delete the contact](#bk_getewsma) using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="45929-160"><a name="bk_resolveews"> </a></span><span class="sxs-lookup"><span data-stu-id="45929-160"></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="45929-161">Résoudre un contact en tant que délégué à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="45929-161">Resolve a contact as a delegate by using EWS</span></span>

<span data-ttu-id="45929-162">EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour résoudre les noms partiels dans le dossier de Contacts du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-162">EWS enables you to use the service object for the delegate user to resolve partial names in the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="45929-163">Cet exemple montre comment utiliser l’opération [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) pour rechercher des réunions dans le dossier Contacts du propriétaire de la boîte aux lettres qui contiennent le mot « johnson ».</span><span class="sxs-lookup"><span data-stu-id="45929-163">This example shows how to use the [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Contacts folder that contain the word "johnson".</span></span> 
  
<span data-ttu-id="45929-164">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **ResolveName** pour [résoudre un contact](#bk_resolveewsma).</span><span class="sxs-lookup"><span data-stu-id="45929-164">This is also the XML request that the EWS Managed API sends when you use the **ResolveName** method to [resolve a contact](#bk_resolveewsma).</span></span>
  
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

<span data-ttu-id="45929-165">Le serveur répond à la demande **ResolveNames** avec un message [ResolveNamesResponse](http://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, qui indique que l’opération terminée avec succès et trouvé une seule résultat, ou **ErrorNameResolutionMultipleResults** si plusieurs résultats trouvés - qui correspond à ce qui est affiché dans le troisième exemple de code basé sur le contact [créer un contact en tant que délégué à l’aide de l’API managée EWS](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="45929-165">The server responds to the **ResolveNames** request with a [ResolveNamesResponse](http://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the operation completed successfully and found only one result, or **ErrorNameResolutionMultipleResults** if multiple results were found - which is what's shown in third code example based on the contact [Create a contact as a delegate by using the EWS Managed API](#bk_createewsma).</span></span> <span data-ttu-id="45929-166">La réponse contient également l' [ID d’élément](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de chaque résultat.</span><span class="sxs-lookup"><span data-stu-id="45929-166">The response also contains the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of each result.</span></span> 
  
<span data-ttu-id="45929-167">La valeur de l’élément **ItemId** a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="45929-167">The value of the **ItemId** element has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="45929-168">Maintenant que vous disposez de l' **ID d’élément** pour les contacts qui correspondent au nom ambigu, vous pouvez [obtenir, mettre à jour ou supprimer des éléments de contact en tant que délégué à l’aide de EWS](#bk_getews) à l’aide de **l’ItemId** et [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;et vous n’avez pas besoin de spécifier adresse SMTP de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-168">Now that you have the **ItemId** for the contacts that match the ambiguous name, you can [Get, update, or delete contact items as a delegate by using EWS](#bk_getews) by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="45929-169"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="45929-169"></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="45929-170">Obtenir, mettre à jour ou supprimer des éléments de contact en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="45929-170">Get, update, or delete contact items as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="45929-171">Vous pouvez utiliser l’API managée EWS pour obtenir, mettre à jour ou supprimer un contact de la même manière que vous effectuez ces actions lorsque vous n’utilisez pas d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="45929-171">You can use the EWS Managed API to get, update, or delete a contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="45929-172">La seule différence est que l’objet de service pour l’utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="45929-172">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="45929-173">L’ID d’élément inclus dans l’appel de méthode **lier** unique identifie l’élément dans le magasin de boîte aux lettres, dans le dossier de Contacts du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-173">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="45929-174">**Le tableau 2. Méthodes d’API managées fonctionne avec un contact en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="45929-174">**Table 2. EWS Managed API methods working with a contact as a delegate**</span></span>

|<span data-ttu-id="45929-175">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="45929-175">**Task**</span></span>|<span data-ttu-id="45929-176">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="45929-176">**EWS Managed API method**</span></span>|<span data-ttu-id="45929-177">**Code example**</span><span class="sxs-lookup"><span data-stu-id="45929-177">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="45929-178">Obtenir une ressource contact</span><span class="sxs-lookup"><span data-stu-id="45929-178">Get a contact</span></span>  <br/> |[<span data-ttu-id="45929-179">Créer une liaison</span><span class="sxs-lookup"><span data-stu-id="45929-179">Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="45929-180">Obtention d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="45929-180">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="45929-181">Mise à jour d'un contact</span><span class="sxs-lookup"><span data-stu-id="45929-181">Update a contact</span></span>  <br/> |<span data-ttu-id="45929-182">[Lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) le suivi de [mise à jour](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="45929-182">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="45929-183">Mise à jour d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="45929-183">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="45929-184">Supprimer un contact</span><span class="sxs-lookup"><span data-stu-id="45929-184">Delete a contact</span></span>  <br/> |<span data-ttu-id="45929-185">[Lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) suivie à [Supprimer](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="45929-185">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="45929-186">Suppression d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="45929-186">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<span data-ttu-id="45929-187"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="45929-187"></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="45929-188">Obtenir, mettre à jour ou supprimer des éléments de contact en tant que délégué à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="45929-188">Get, update, or delete contact items as a delegate by using EWS</span></span>

<span data-ttu-id="45929-189">Vous pouvez utiliser EWS pour obtenir, mettre à jour ou supprimer un contact de réunion ou un rendez-vous de la même manière que vous effectuez ces actions lorsque vous n’utilisez pas d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="45929-189">You can use EWS to get, update, or delete a meeting or appointment contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="45929-190">La seule différence est que l’objet de service pour l’utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="45929-190">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="45929-191">L’ID d’élément inclus dans la demande de [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) unique identifie l’élément dans le magasin de boîte aux lettres, dans le dossier de Contacts du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="45929-191">The item ID included in the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) request uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="45929-192">**Le tableau 3. Opérations EWS pour travailler avec un contact en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="45929-192">**Table 3. EWS operations for working with a contact as a delegate**</span></span>

|<span data-ttu-id="45929-193">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="45929-193">**Task**</span></span>|<span data-ttu-id="45929-194">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="45929-194">**EWS operation**</span></span>|<span data-ttu-id="45929-195">**Aperçu**</span><span class="sxs-lookup"><span data-stu-id="45929-195">**Sample**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="45929-196">Obtenir une ressource contact</span><span class="sxs-lookup"><span data-stu-id="45929-196">Get a contact</span></span>  <br/> |[<span data-ttu-id="45929-197">GetItem</span><span class="sxs-lookup"><span data-stu-id="45929-197">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="45929-198">Obtention d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="45929-198">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="45929-199">Mise à jour d'un contact</span><span class="sxs-lookup"><span data-stu-id="45929-199">Update a contact</span></span>  <br/> |<span data-ttu-id="45929-200">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="45929-200">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="45929-201">Mise à jour d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="45929-201">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="45929-202">Supprimer un contact</span><span class="sxs-lookup"><span data-stu-id="45929-202">Delete a contact</span></span>  <br/> |<span data-ttu-id="45929-203">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="45929-203">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[<span data-ttu-id="45929-204">Suppression d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="45929-204">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45929-205">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="45929-205">See also</span></span>

- [<span data-ttu-id="45929-206">Accès délégué et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="45929-206">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="45929-207">Ajouter et supprimer des délégués à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="45929-207">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="45929-208">Définir des autorisations de dossier pour un autre utilisateur à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="45929-208">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [<span data-ttu-id="45929-209">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="45929-209">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
- [<span data-ttu-id="45929-210">Résoudre des noms ambigus en utilisant EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="45929-210">Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

