---
title: Accéder à la messagerie en tant que délégué à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a8123604-c7c0-405d-a0ed-7a9b4a431bfd
description: Découvrez comment accéder à leur messagerie à l’aide de l’API managée EWS ou EWS dans Exchange en tant que délégué.
ms.openlocfilehash: 8331f337136426913347cf6941d64b4611922d74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754798"
---
# <a name="access-email-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="38c37-103">Accéder à la messagerie en tant que délégué à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38c37-103">Access email as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="38c37-104">Découvrez comment accéder à leur messagerie à l’aide de l’API managée EWS ou EWS dans Exchange en tant que délégué.</span><span class="sxs-lookup"><span data-stu-id="38c37-104">Learn how to access email as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="38c37-105">Vous pouvez utiliser l’API managée EWS ou EWS pour donner à un utilisateur délégué l’accès au dossier de boîte de réception du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-105">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Inbox folder.</span></span> <span data-ttu-id="38c37-106">Le délégué peut ensuite créer des demandes de réunion pour le compte du propriétaire de boîte aux lettres, de recherche pour le courrier électronique, récupérer et mettre à jour, supprimer le courrier électronique à partir du dossier boîte de réception du propriétaire de la boîte aux lettres, en fonction de leurs autorisations.</span><span class="sxs-lookup"><span data-stu-id="38c37-106">The delegate can then create meeting requests on behalf of the mailbox owner, search for email, and retrieve, update, and delete email from the mailbox owner's Inbox folder, depending on their permissions.</span></span>
  
<span data-ttu-id="38c37-107">En tant que délégué, vous utilisez les mêmes méthodes et opérations pour accéder au dossier boîte de réception du propriétaire de la boîte aux lettres que vous utilisez pour accéder à un dossier boîte de réception sans accès délégué.</span><span class="sxs-lookup"><span data-stu-id="38c37-107">As a delegate, you use the same methods and operations to access a mailbox owner's Inbox folder that you use to access an Inbox folder without delegate access.</span></span> <span data-ttu-id="38c37-108">La principale différence est que vous devez utiliser [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicit) pour trouver ou créer un élément de courrier électronique, puis après avoir identifié l’ID d’élément, vous pouvez utiliser [un accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) pour obtenir, de mettre à jour ou de supprimer l’élément.</span><span class="sxs-lookup"><span data-stu-id="38c37-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create an email item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="38c37-109">**Le tableau 1. Méthodes d’API managées et opérations EWS pour accéder au courrier électronique en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="38c37-109">**Table 1. EWS Managed API methods and EWS operations for accessing email as a delegate**</span></span>

|<span data-ttu-id="38c37-110">**Si vous souhaitez...**</span><span class="sxs-lookup"><span data-stu-id="38c37-110">**If you want to…**</span></span>|<span data-ttu-id="38c37-111">**Utilisez cette méthode d’API managées...**</span><span class="sxs-lookup"><span data-stu-id="38c37-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="38c37-112">**Utilisez cette opération EWS...**</span><span class="sxs-lookup"><span data-stu-id="38c37-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="38c37-113">Créer et envoyer un message électronique en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="38c37-113">Create and send an email as a delegate</span></span>  <br/> |<span data-ttu-id="38c37-114">[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) où le paramètre [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) dans le dossier Brouillons du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="38c37-114">[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Drafts folder</span></span>  <br/> <span data-ttu-id="38c37-115">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) où le paramètre [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) pour le dossier éléments envoyés du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="38c37-115">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Sent Items folder</span></span>  <br/> |<span data-ttu-id="38c37-116">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="38c37-116">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> <span data-ttu-id="38c37-117">[SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="38c37-117">[SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="38c37-118">Créer plusieurs messages électroniques en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="38c37-118">Create multiple email messages as a delegate</span></span>  <br/> |<span data-ttu-id="38c37-119">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de boîte de réception du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="38c37-119">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="38c37-120">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="38c37-120">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="38c37-121">Recherchez ou rechercher un message électronique en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="38c37-121">Search for or find an email as a delegate</span></span>  <br/> |<span data-ttu-id="38c37-122">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de boîte de réception du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="38c37-122">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="38c37-123">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="38c37-123">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="38c37-124">Obtenir un message électronique en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="38c37-124">Get an email as a delegate</span></span>  <br/> |[<span data-ttu-id="38c37-125">EmailMessage.Bind</span><span class="sxs-lookup"><span data-stu-id="38c37-125">EmailMessage.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="38c37-126">GetItem</span><span class="sxs-lookup"><span data-stu-id="38c37-126">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="38c37-127">Mettre à jour un message électronique en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="38c37-127">Update an email as a delegate</span></span>  <br/> |<span data-ttu-id="38c37-128">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) suivi [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38c37-128">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="38c37-129">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38c37-129">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="38c37-130">Supprimer un message électronique en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="38c37-130">Delete an email as a delegate</span></span>  <br/> |<span data-ttu-id="38c37-131">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) suivi [EmailMessage.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38c37-131">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="38c37-132">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38c37-132">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |
   
<span data-ttu-id="38c37-133">Gardez les éléments suivants à l’esprit lorsque vous travaillez avec les messages électroniques en tant que délégué :</span><span class="sxs-lookup"><span data-stu-id="38c37-133">Keep the following things in mind when working with emails as a delegate:</span></span>
  
- <span data-ttu-id="38c37-134">Si un délégué n’a besoin travailler avec des demandes de réunion et les réponses, le délégué ne doit pas accès au dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="38c37-134">If a delegate only needs to work with meeting requests and responses, the delegate does not need access to the Inbox folder.</span></span> <span data-ttu-id="38c37-135">Pour plus d’informations, voir [les tâches requises pour l’accès aux calendriers en tant que délégué](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).</span><span class="sxs-lookup"><span data-stu-id="38c37-135">For more information, see [prerequisite tasks for accessing calendars as a delegate](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).</span></span>
    
- <span data-ttu-id="38c37-136">Lorsqu’un destinataire reçoit un message qui a été envoyé au nom d’un propriétaire de boîte aux lettres, l’expéditeur s’affiche en tant que « *délégué* au nom du *propriétaire de boîte aux lettres* ».</span><span class="sxs-lookup"><span data-stu-id="38c37-136">When a recipient receives a message that was sent on behalf of a mailbox owner, the sender appears as " *Delegate*  on behalf of  *mailbox owner*  ."</span></span> 
    
> [!NOTE]
> <span data-ttu-id="38c37-137">Dans les exemples de code dans cet article, primary@contoso.com est le propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-137">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="38c37-138">Les tâches préalables</span><span class="sxs-lookup"><span data-stu-id="38c37-138">Prerequisite tasks</span></span>
<span data-ttu-id="38c37-139"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="38c37-139"></span></span>

<span data-ttu-id="38c37-140">Qu’un utilisateur puisse accéder dossier de boîte de réception du propriétaire de la boîte aux lettres en tant que délégué, l’utilisateur doit être [ajouté en tant que délégué disposant des autorisations](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) au dossier de boîte de réception du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-140">Before a user can access the mailbox owner's Inbox folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-and-send-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="38c37-141">Créer et envoyer un message électronique en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-141">Create and send an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="38c37-142"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="38c37-142"></span></span>

<span data-ttu-id="38c37-143">L’API managée EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour créer et envoyer un message électronique au nom du propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-143">The EWS Managed API enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner.</span></span> <span data-ttu-id="38c37-144">Cet exemple montre comment utiliser la méthode [Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) pour enregistrer le message dans le dossier Brouillons du propriétaire de la boîte aux lettres, puis la méthode [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) pour envoyer le message et enregistrez le message dans le dossier éléments envoyés du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-144">This example shows how to use the [Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) method to save the message in the mailbox owner's Drafts folder, and then the [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) method to send the mail and save the message in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="38c37-145">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le délégué et le délégué a reçu les [autorisations appropriées pour le dossier de boîte de réception, Brouillons et éléments envoyés du propriétaire de la boîte aux lettres](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="38c37-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the [appropriate permissions for the mailbox owner's Inbox, Drafts, and Sent Items folder](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
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

## <a name="create-and-send-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="38c37-146">Créer et envoyer un message électronique en tant que délégué à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-146">Create and send an email as a delegate by using EWS</span></span>
<span data-ttu-id="38c37-147"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="38c37-147"></span></span>

<span data-ttu-id="38c37-148">EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour créer et envoyer un message électronique au nom du propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-148">EWS enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner.</span></span> <span data-ttu-id="38c37-149">Cet exemple montre comment utiliser l’opération [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour créer un message électronique et l’opération [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) pour envoyer l’heure et enregistrez-le dans le dossier éléments envoyés du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-149">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create an email and the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation to send the time and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="38c37-150">C’est également la première requête XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **Save** pour [créer et envoyer un message électronique](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="38c37-150">This is also the first XML request that the EWS Managed API sends when you use the **Save** method to [create and send an email](#bk_createewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="38c37-151">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le courrier électronique a été créé et enregistré avec succès.</span><span class="sxs-lookup"><span data-stu-id="38c37-151">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was created and saved successfully.</span></span> <span data-ttu-id="38c37-152">La réponse contient également l’ID d’élément du courrier électronique nouvellement créé.</span><span class="sxs-lookup"><span data-stu-id="38c37-152">The response also contains the item ID of the newly created email.</span></span>
  
<span data-ttu-id="38c37-153">La valeur **ItemId** a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="38c37-153">The **ItemId** value has been shortened for readability.</span></span> 
  
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
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="38c37-154">Ensuite, utilisez l’opération **SendItem** pour envoyer le message au propriétaire de la boîte aux lettres et enregistrez-le dans le dossier éléments envoyés du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-154">Next, use the **SendItem** operation to send the message on behalf of the mailbox owner and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="38c37-155">La valeur **ItemId** a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="38c37-155">The **ItemId** value has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="38c37-156">Le serveur répond à la demande **SendItem** avec un message [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que le courrier électronique a été envoyé et enregistré dans le dossier éléments envoyés du propriétaire de la boîte aux lettres avec succès.</span><span class="sxs-lookup"><span data-stu-id="38c37-156">The server responds to the **SendItem** request with a [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was sent and saved to the mailbox owner's Sent Items folder successfully.</span></span>
  
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
    <m:SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </m:SendItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="search-for-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="38c37-157">Rechercher un message électronique en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-157">Search for an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="38c37-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="38c37-158"></span></span>

<span data-ttu-id="38c37-159">Pour rechercher un message électronique, vous devez utiliser une des méthodes [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) qui comprend un paramètre [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , afin que vous pouvez spécifier le dossier de boîte de réception du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-159">To search for an email, you must use one of the [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Inbox folder.</span></span> 
  
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

<span data-ttu-id="38c37-160">Une fois l’appel **FindItems** retourne une réponse avec un ID, vous pouvez obtenir, mise à jour ou suppression de messagerie à l’aide de l’ID et [un accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) - et vous est inutile spécifier l’adresse SMTP de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that email by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) - and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="38c37-161">Rechercher un message électronique en tant que délégué à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-161">Search for an email as a delegate by using EWS</span></span>
<span data-ttu-id="38c37-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="38c37-162"></span></span>

<span data-ttu-id="38c37-163">EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour rechercher des messages électroniques qui répondent à un ensemble de critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="38c37-163">EWS enables you to use the service object for the delegate user to search for emails that meet a set of search criteria.</span></span> <span data-ttu-id="38c37-164">Cet exemple montre comment utiliser l’opération [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour rechercher les messages dans le dossier du propriétaire de la boîte de réception qui contiennent le mot « football » dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="38c37-164">This example shows how to use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find messages in the owner's Inbox folder that contain the word "soccer" in the subject.</span></span> 
  
<span data-ttu-id="38c37-165">C’est également la demande XML que l’API managée EWS envoie lorsque vous [Recherchez un message électronique](#bk_searchewsma).</span><span class="sxs-lookup"><span data-stu-id="38c37-165">This is also the XML request that the EWS Managed API sends when you [search for an email](#bk_searchewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="38c37-166">Le serveur répond à la demande **FindItem** avec un message [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, qui indique que la recherche s’est terminée correctement.</span><span class="sxs-lookup"><span data-stu-id="38c37-166">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully.</span></span> <span data-ttu-id="38c37-167">La réponse contient un élément de [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) pour les messages électroniques qui répondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="38c37-167">The response contains a [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) element for any emails that met the search criteria.</span></span> <span data-ttu-id="38c37-168">Dans ce cas, qu’un e-mail est trouvée.</span><span class="sxs-lookup"><span data-stu-id="38c37-168">In this case, only one email is found.</span></span> 
  
<span data-ttu-id="38c37-169">La valeur de l’élément [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="38c37-169">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
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
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="38c37-170">Maintenant que vous avez l' **ItemId** pour le courrier électronique qui répond à vos critères, vous pouvez obtenir, mise à jour ou suppression de messagerie à l’aide de l' **ID d’élément** et [un accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) - et est inutile spécifier l’adresse SMTP de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-170">Now that you have the **ItemId** for the email that meets your criteria, you can get, update, or delete that email by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) - and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="38c37-171">Obtenir, mettre à jour ou supprimer des éléments de courrier électronique en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-171">Get, update, or delete email items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="38c37-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="38c37-172"></span></span>

<span data-ttu-id="38c37-173">Vous pouvez utiliser l’API managée EWS pour obtenir, mettre à jour ou supprimer un message électronique de la même manière que vous effectuez ces actions lorsque vous n’utilisez pas d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="38c37-173">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="38c37-174">La seule différence est que l’objet **ExchangeService** pour l’utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="38c37-174">The only difference is that the **ExchangeService** object is for the delegate user.</span></span> <span data-ttu-id="38c37-175">L’ID d’élément inclus dans l’appel de méthode **lier** unique identifie l’élément dans le magasin de boîte aux lettres, dans le dossier de boîte de réception du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-175">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="38c37-176">**Le tableau 2. Méthodes d’API managées utilisation de messagerie en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="38c37-176">**Table 2. EWS Managed API methods working with email as a delegate**</span></span>

|<span data-ttu-id="38c37-177">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="38c37-177">**Task**</span></span>|<span data-ttu-id="38c37-178">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="38c37-178">**EWS Managed API method**</span></span>|<span data-ttu-id="38c37-179">**Exemple de code**</span><span class="sxs-lookup"><span data-stu-id="38c37-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="38c37-180">Obtenir un message électronique</span><span class="sxs-lookup"><span data-stu-id="38c37-180">Get an email</span></span>  <br/> |[<span data-ttu-id="38c37-181">Créer une liaison</span><span class="sxs-lookup"><span data-stu-id="38c37-181">Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="38c37-182">Obtenir un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="38c37-183">Mettre à jour un message électronique</span><span class="sxs-lookup"><span data-stu-id="38c37-183">Update an email</span></span>  <br/> |<span data-ttu-id="38c37-184">[Lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) le suivi de [mise à jour](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38c37-184">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="38c37-185">Mettre à jour un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-185">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="38c37-186">Supprimer un message électronique</span><span class="sxs-lookup"><span data-stu-id="38c37-186">Delete an email</span></span>  <br/> |<span data-ttu-id="38c37-187">[Lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) suivie à [Supprimer](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38c37-187">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="38c37-188">Supprimer un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-188">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |
   
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="38c37-189">Obtenir, mettre à jour ou supprimer des éléments de courrier électronique en tant que délégué à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-189">Get, update, or delete email items as a delegate by using EWS</span></span>
<span data-ttu-id="38c37-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="38c37-190"></span></span>

<span data-ttu-id="38c37-191">Vous pouvez utiliser l’API managée EWS pour obtenir, mettre à jour ou supprimer un message électronique de la même manière que vous effectuez ces actions lorsque vous n’utilisez pas d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="38c37-191">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="38c37-192">La seule différence est que l’objet de service pour l’utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="38c37-192">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="38c37-193">L’ID d’élément inclus dans la demande de **GetItem** unique identifie l’élément dans le magasin de boîte aux lettres, dans le dossier de boîte de réception du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="38c37-193">The item ID included in the **GetItem** request uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="38c37-194">**Le tableau 3. Opérations EWS pour l’utilisation de la messagerie en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="38c37-194">**Table 3. EWS operations for working with email as a delegate**</span></span>

|<span data-ttu-id="38c37-195">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="38c37-195">**Task**</span></span>|<span data-ttu-id="38c37-196">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="38c37-196">**EWS operation**</span></span>|<span data-ttu-id="38c37-197">**Exemple de code**</span><span class="sxs-lookup"><span data-stu-id="38c37-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="38c37-198">Obtenir un message électronique</span><span class="sxs-lookup"><span data-stu-id="38c37-198">Get an email</span></span>  <br/> |[<span data-ttu-id="38c37-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="38c37-199">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="38c37-200">Obtenir un élément à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="38c37-201">Mettre à jour un message électronique</span><span class="sxs-lookup"><span data-stu-id="38c37-201">Update an email</span></span>  <br/> |<span data-ttu-id="38c37-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38c37-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="38c37-203">Mettre à jour un élément à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-203">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="38c37-204">Supprimer un message électronique</span><span class="sxs-lookup"><span data-stu-id="38c37-204">Delete an email</span></span>  <br/> |<span data-ttu-id="38c37-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="38c37-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="38c37-206">Supprimer un élément à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="38c37-206">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38c37-207">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="38c37-207">See also</span></span>

- [<span data-ttu-id="38c37-208">Accès délégué et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38c37-208">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)    
- [<span data-ttu-id="38c37-209">Ajouter et supprimer des délégués à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38c37-209">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="38c37-210">Définir des autorisations de dossier pour un autre utilisateur à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38c37-210">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="38c37-211">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="38c37-211">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

