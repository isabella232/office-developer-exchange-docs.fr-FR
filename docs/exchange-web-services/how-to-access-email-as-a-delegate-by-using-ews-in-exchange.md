---
title: Accéder à la messagerie électronique en tant que délégué à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a8123604-c7c0-405d-a0ed-7a9b4a431bfd
description: Découvrez comment accéder à la messagerie électronique en tant que délégué à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 0c26f69042c568fe7d877778c7d8f1e689e5b372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528285"
---
# <a name="access-email-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="ed0ce-103">Accéder à la messagerie électronique en tant que délégué à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ed0ce-103">Access email as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="ed0ce-104">Découvrez comment accéder à la messagerie électronique en tant que délégué à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-104">Learn how to access email as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="ed0ce-105">Vous pouvez utiliser l’API managée EWS ou EWS pour accorder à un utilisateur un accès délégué au dossier boîte de réception d’un propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-105">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Inbox folder.</span></span> <span data-ttu-id="ed0ce-106">Le délégué peut ensuite créer des demandes de réunion de la part du propriétaire de la boîte aux lettres, Rechercher des courriers électroniques et récupérer, mettre à jour et supprimer des messages électroniques du dossier boîte de réception du propriétaire de la boîte aux lettres, en fonction de leurs autorisations.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-106">The delegate can then create meeting requests on behalf of the mailbox owner, search for email, and retrieve, update, and delete email from the mailbox owner's Inbox folder, depending on their permissions.</span></span>
  
<span data-ttu-id="ed0ce-107">En tant que délégué, vous utilisez les mêmes méthodes et opérations pour accéder au dossier boîte de réception d’un propriétaire de boîte aux lettres que vous utilisez pour accéder à un dossier boîte de réception sans accès délégué.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-107">As a delegate, you use the same methods and operations to access a mailbox owner's Inbox folder that you use to access an Inbox folder without delegate access.</span></span> <span data-ttu-id="ed0ce-108">La principale différence réside dans le fait que vous devez utiliser un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicit) pour rechercher ou créer un élément de courrier, puis après avoir identifié l’ID d’élément, vous pouvez utiliser l' [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) pour obtenir, mettre à jour ou supprimer l’élément.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create an email item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="ed0ce-109">**Tableau 1. Méthodes d’API managée EWS et opérations EWS pour l’accès à la messagerie électronique en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-109">**Table 1. EWS Managed API methods and EWS operations for accessing email as a delegate**</span></span>

|<span data-ttu-id="ed0ce-110">**Si vous souhaitez...**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-110">**If you want to…**</span></span>|<span data-ttu-id="ed0ce-111">**Utilisez cette méthode d’API managée EWS...**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="ed0ce-112">**Utilisez cette opération EWS...**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ed0ce-113">Créer et envoyer un message électronique en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="ed0ce-113">Create and send an email as a delegate</span></span>  <br/> |<span data-ttu-id="ed0ce-114">[EmailMessage. Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) où le paramètre [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier Brouillons du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ed0ce-114">[EmailMessage.Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Drafts folder</span></span>  <br/> <span data-ttu-id="ed0ce-115">[EmailMessage. méthodesendandsavecopy](https://msdn.microsoft.com/library/dd634248%28v=exchg.80%29.aspx) où le paramètre [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier éléments envoyés du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ed0ce-115">[EmailMessage.SendAndSaveCopy](https://msdn.microsoft.com/library/dd634248%28v=exchg.80%29.aspx) where the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Sent Items folder</span></span>  <br/> |<span data-ttu-id="ed0ce-116">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) où l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie le [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ed0ce-116">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> <span data-ttu-id="ed0ce-117">[SendItem](https://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) où l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie le [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ed0ce-117">[SendItem](https://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="ed0ce-118">Créer plusieurs messages électroniques en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="ed0ce-118">Create multiple email messages as a delegate</span></span>  <br/> |<span data-ttu-id="ed0ce-119">[ExchangeService. CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier boîte de réception du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ed0ce-119">[ExchangeService.CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="ed0ce-120">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) où l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie le [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ed0ce-120">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="ed0ce-121">Rechercher ou Rechercher un message électronique en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="ed0ce-121">Search for or find an email as a delegate</span></span>  <br/> |<span data-ttu-id="ed0ce-122">[ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier boîte de réception du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ed0ce-122">[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="ed0ce-123">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) où l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie le [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ed0ce-123">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="ed0ce-124">Obtenir un message électronique en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="ed0ce-124">Get an email as a delegate</span></span>  <br/> |[<span data-ttu-id="ed0ce-125">EmailMessage. bind</span><span class="sxs-lookup"><span data-stu-id="ed0ce-125">EmailMessage.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="ed0ce-126">GetItem</span><span class="sxs-lookup"><span data-stu-id="ed0ce-126">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="ed0ce-127">Mettre à jour un message électronique en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="ed0ce-127">Update an email as a delegate</span></span>  <br/> |<span data-ttu-id="ed0ce-128">[EmailMessage. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) suivi de [EmailMessage. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ed0ce-128">[EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="ed0ce-129">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi de [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ed0ce-129">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="ed0ce-130">Supprimer un message électronique en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="ed0ce-130">Delete an email as a delegate</span></span>  <br/> |<span data-ttu-id="ed0ce-131">[EmailMessage. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) suivi de [EmailMessage. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ed0ce-131">[EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="ed0ce-132">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , suivi de [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="ed0ce-132">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
<span data-ttu-id="ed0ce-133">Gardez les points suivants à l’esprit lorsque vous utilisez des courriers électroniques en tant que délégué :</span><span class="sxs-lookup"><span data-stu-id="ed0ce-133">Keep the following things in mind when working with emails as a delegate:</span></span>
  
- <span data-ttu-id="ed0ce-134">Si un délégué ne doit travailler qu’avec des demandes de réunion et des réponses, il n’a pas besoin d’accéder au dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-134">If a delegate only needs to work with meeting requests and responses, the delegate does not need access to the Inbox folder.</span></span> <span data-ttu-id="ed0ce-135">Pour plus d’informations, reportez-vous à [tâches préalables pour l’accès aux calendriers en tant que délégué](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).</span><span class="sxs-lookup"><span data-stu-id="ed0ce-135">For more information, see [prerequisite tasks for accessing calendars as a delegate](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).</span></span>
    
- <span data-ttu-id="ed0ce-136">Lorsqu’un destinataire reçoit un message qui a été envoyé de la part d’un propriétaire de la boîte aux lettres, l’expéditeur apparaît sous la forme « *délégué* de la part du propriétaire de la *boîte aux lettres* ».</span><span class="sxs-lookup"><span data-stu-id="ed0ce-136">When a recipient receives a message that was sent on behalf of a mailbox owner, the sender appears as " *Delegate*  on behalf of  *mailbox owner*  ."</span></span> 
    
> [!NOTE]
> <span data-ttu-id="ed0ce-137">Dans les exemples de code de cet article, primary@contoso.com est le propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-137">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="ed0ce-138">Tâches préalables</span><span class="sxs-lookup"><span data-stu-id="ed0ce-138">Prerequisite tasks</span></span>
<span data-ttu-id="ed0ce-139"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="ed0ce-139"><a name="bk_prereq"> </a></span></span>

<span data-ttu-id="ed0ce-140">Pour qu’un utilisateur puisse accéder au dossier boîte de réception du propriétaire de la boîte aux lettres en tant que délégué, il doit être [ajouté en tant que délégué avec des autorisations](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) sur le dossier boîte de réception du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-140">Before a user can access the mailbox owner's Inbox folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-and-send-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="ed0ce-141">Créer et envoyer un message électronique en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-141">Create and send an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="ed0ce-142"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ed0ce-142"><a name="bk_createewsma"> </a></span></span>

<span data-ttu-id="ed0ce-143">L’API managée EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué afin de créer et d’envoyer des courriers électroniques au nom du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-143">The EWS Managed API enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner.</span></span> <span data-ttu-id="ed0ce-144">Cet exemple montre comment utiliser la méthode [Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) pour enregistrer le message dans le dossier Brouillons du propriétaire de la boîte aux lettres, puis la méthode [méthodesendandsavecopy](https://msdn.microsoft.com/library/dd634248%28v=exchg.80%29.aspx) pour envoyer le message et enregistrer le message dans le dossier éléments envoyés du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-144">This example shows how to use the [Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) method to save the message in the mailbox owner's Drafts folder, and then the [SendAndSaveCopy](https://msdn.microsoft.com/library/dd634248%28v=exchg.80%29.aspx) method to send the mail and save the message in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="ed0ce-145">Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le délégué et que le délégué dispose des [autorisations appropriées pour le dossier boîte de réception, brouillons et éléments envoyés du propriétaire de la boîte aux lettres](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="ed0ce-145">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the [appropriate permissions for the mailbox owner's Inbox, Drafts, and Sent Items folder](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
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

## <a name="create-and-send-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="ed0ce-146">Créer et envoyer un courrier électronique en tant que délégué à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-146">Create and send an email as a delegate by using EWS</span></span>
<span data-ttu-id="ed0ce-147"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="ed0ce-147"><a name="bk_createews"> </a></span></span>

<span data-ttu-id="ed0ce-148">EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué afin de créer et d’envoyer des courriers électroniques au nom du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-148">EWS enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner.</span></span> <span data-ttu-id="ed0ce-149">Cet exemple montre comment utiliser l’opération [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour créer un message électronique et l’opération [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) pour envoyer l’heure et l’enregistrer dans le dossier éléments envoyés du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-149">This example shows how to use the [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create an email and the [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation to send the time and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="ed0ce-150">Il s’agit également de la première demande XML que l’API managée EWS envoie lorsque vous utilisez la méthode **Save** pour [créer et envoyer un message électronique](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="ed0ce-150">This is also the first XML request that the EWS Managed API sends when you use the **Save** method to [create and send an email](#bk_createewsma).</span></span>
  
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

<span data-ttu-id="ed0ce-151">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui inclut la valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NOERROR**, ce qui indique que le message électronique a été créé et enregistré avec succès.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-151">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was created and saved successfully.</span></span> <span data-ttu-id="ed0ce-152">La réponse contient également l’ID de l’élément du message nouvellement créé.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-152">The response also contains the item ID of the newly created email.</span></span>
  
<span data-ttu-id="ed0ce-153">La valeur **ItemId** a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-153">The **ItemId** value has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="ed0ce-154">Ensuite, utilisez l’opération **SendItem** pour envoyer le message au nom du propriétaire de la boîte aux lettres et enregistrez-le dans le dossier éléments envoyés du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-154">Next, use the **SendItem** operation to send the message on behalf of the mailbox owner and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="ed0ce-155">La valeur **ItemId** a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-155">The **ItemId** value has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="ed0ce-156">Le serveur répond à la demande **SendItem** avec un message [SendItemResponse](https://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que le message électronique a été envoyé et enregistré avec succès dans le dossier éléments envoyés du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-156">The server responds to the **SendItem** request with a [SendItemResponse](https://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was sent and saved to the mailbox owner's Sent Items folder successfully.</span></span>
  
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

## <a name="search-for-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="ed0ce-157">Rechercher un message électronique en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-157">Search for an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="ed0ce-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ed0ce-158"><a name="bk_searchewsma"> </a></span></span>

<span data-ttu-id="ed0ce-159">Pour rechercher un message électronique, vous devez utiliser l’une des méthodes [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) qui inclut un paramètre [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , afin que vous puissiez spécifier le dossier boîte de réception du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-159">To search for an email, you must use one of the [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Inbox folder.</span></span> 
  
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

<span data-ttu-id="ed0ce-160">Une fois que l’appel **FindItems** renvoie une réponse avec un ID, vous pouvez obtenir, mettre à jour ou supprimer ce courrier électronique à l’aide de l’ID et de l' [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) -et vous n’avez pas besoin de spécifier l’adresse SMTP du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that email by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) - and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="ed0ce-161">Rechercher un message électronique en tant que délégué à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-161">Search for an email as a delegate by using EWS</span></span>
<span data-ttu-id="ed0ce-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="ed0ce-162"><a name="bk_searchews"> </a></span></span>

<span data-ttu-id="ed0ce-163">EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué afin de rechercher des courriers électroniques qui répondent à un ensemble de critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-163">EWS enables you to use the service object for the delegate user to search for emails that meet a set of search criteria.</span></span> <span data-ttu-id="ed0ce-164">Cet exemple montre comment utiliser l’opération [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour rechercher des messages dans le dossier boîte de réception du propriétaire qui contiennent le mot « football » dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-164">This example shows how to use the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find messages in the owner's Inbox folder that contain the word "soccer" in the subject.</span></span> 
  
<span data-ttu-id="ed0ce-165">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous [recherchez un message électronique](#bk_searchewsma).</span><span class="sxs-lookup"><span data-stu-id="ed0ce-165">This is also the XML request that the EWS Managed API sends when you [search for an email](#bk_searchewsma).</span></span>
  
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

<span data-ttu-id="ed0ce-166">Le serveur répond à la demande **FindItem** avec un message [FindItemResponse](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que la recherche s’est terminée avec succès.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-166">The server responds to the **FindItem** request with a [FindItemResponse](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully.</span></span> <span data-ttu-id="ed0ce-167">La réponse contient un élément [message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) pour tous les messages électroniques qui répondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-167">The response contains a [Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) element for any emails that met the search criteria.</span></span> <span data-ttu-id="ed0ce-168">Dans ce cas, un seul courrier électronique est trouvé.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-168">In this case, only one email is found.</span></span> 
  
<span data-ttu-id="ed0ce-169">La valeur de l’élément [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-169">The value of the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="ed0ce-170">Maintenant que vous disposez de l' **ID ItemId** pour le courrier électronique qui répond à vos critères, vous pouvez obtenir, mettre à jour ou supprimer ce courrier électronique à l’aide de l' **ItemId** et de l' [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) -et vous n’avez pas besoin de spécifier l’adresse SMTP du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-170">Now that you have the **ItemId** for the email that meets your criteria, you can get, update, or delete that email by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) - and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="ed0ce-171">Obtenir, mettre à jour ou supprimer des éléments de courrier électronique en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-171">Get, update, or delete email items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="ed0ce-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="ed0ce-172"><a name="bk_geteswma"> </a></span></span>

<span data-ttu-id="ed0ce-173">Vous pouvez utiliser l’API managée EWS pour obtenir, mettre à jour ou supprimer un message électronique de la même façon que vous effectuez ces actions lorsque vous n’utilisez pas l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-173">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="ed0ce-174">La seule différence réside dans le fait que l’objet **ExchangeService** est destiné à l’utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-174">The only difference is that the **ExchangeService** object is for the delegate user.</span></span> <span data-ttu-id="ed0ce-175">L’ID d’élément inclus dans l’appel de méthode de **liaison** identifie de manière unique l’élément dans la Banque de boîtes aux lettres, dans le dossier boîte de réception du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-175">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="ed0ce-176">**Tableau 2. Méthodes de l’API managée EWS utilisant le courrier électronique en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-176">**Table 2. EWS Managed API methods working with email as a delegate**</span></span>

|<span data-ttu-id="ed0ce-177">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-177">**Task**</span></span>|<span data-ttu-id="ed0ce-178">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-178">**EWS Managed API method**</span></span>|<span data-ttu-id="ed0ce-179">**Exemple de code**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ed0ce-180">Obtenir un message électronique</span><span class="sxs-lookup"><span data-stu-id="ed0ce-180">Get an email</span></span>  <br/> |[<span data-ttu-id="ed0ce-181">Rattach</span><span class="sxs-lookup"><span data-stu-id="ed0ce-181">Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="ed0ce-182">Obtention d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="ed0ce-183">Mettre à jour un message électronique</span><span class="sxs-lookup"><span data-stu-id="ed0ce-183">Update an email</span></span>  <br/> |<span data-ttu-id="ed0ce-184">[Liaison](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) suivie par la [mise à jour](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ed0ce-184">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="ed0ce-185">Mise à jour d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-185">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="ed0ce-186">Supprimer un message électronique</span><span class="sxs-lookup"><span data-stu-id="ed0ce-186">Delete an email</span></span>  <br/> |<span data-ttu-id="ed0ce-187">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) suivi de [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ed0ce-187">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="ed0ce-188">Suppression d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-188">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |
   
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="ed0ce-189">Obtenir, mettre à jour ou supprimer des éléments de courrier électronique en tant que délégué à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-189">Get, update, or delete email items as a delegate by using EWS</span></span>
<span data-ttu-id="ed0ce-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="ed0ce-190"><a name="bk_getews"> </a></span></span>

<span data-ttu-id="ed0ce-191">Vous pouvez utiliser l’API managée EWS pour obtenir, mettre à jour ou supprimer un message électronique de la même façon que vous effectuez ces actions lorsque vous n’utilisez pas l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-191">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="ed0ce-192">La seule différence réside dans le fait que l’objet de service est destiné à l’utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-192">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="ed0ce-193">L’ID d’élément inclus dans la demande **GetItem** identifie de façon unique l’élément dans la Banque de boîtes aux lettres, dans le dossier boîte de réception du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed0ce-193">The item ID included in the **GetItem** request uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="ed0ce-194">**Tableau 3. Opérations EWS pour l’utilisation d’un message électronique en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-194">**Table 3. EWS operations for working with email as a delegate**</span></span>

|<span data-ttu-id="ed0ce-195">**Task**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-195">**Task**</span></span>|<span data-ttu-id="ed0ce-196">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-196">**EWS operation**</span></span>|<span data-ttu-id="ed0ce-197">**Exemple de code**</span><span class="sxs-lookup"><span data-stu-id="ed0ce-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ed0ce-198">Obtenir un message électronique</span><span class="sxs-lookup"><span data-stu-id="ed0ce-198">Get an email</span></span>  <br/> |[<span data-ttu-id="ed0ce-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="ed0ce-199">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="ed0ce-200">Obtention d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="ed0ce-201">Mettre à jour un message électronique</span><span class="sxs-lookup"><span data-stu-id="ed0ce-201">Update an email</span></span>  <br/> |<span data-ttu-id="ed0ce-202">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi de [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ed0ce-202">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="ed0ce-203">Mise à jour d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-203">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="ed0ce-204">Supprimer un message électronique</span><span class="sxs-lookup"><span data-stu-id="ed0ce-204">Delete an email</span></span>  <br/> |<span data-ttu-id="ed0ce-205">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , suivi de [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="ed0ce-205">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[<span data-ttu-id="ed0ce-206">Suppression d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ed0ce-206">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed0ce-207">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ed0ce-207">See also</span></span>

- [<span data-ttu-id="ed0ce-208">Accès délégué et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ed0ce-208">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)    
- [<span data-ttu-id="ed0ce-209">Ajouter et supprimer des délégués à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ed0ce-209">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="ed0ce-210">Définir les autorisations de dossier pour un autre utilisateur à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ed0ce-210">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="ed0ce-211">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ed0ce-211">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

