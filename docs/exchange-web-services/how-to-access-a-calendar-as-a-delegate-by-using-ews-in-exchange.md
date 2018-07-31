---
title: Accéder à un calendrier en tant que délégué à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Découvrez comment accéder à un calendrier en tant que délégué à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 609e5f0bb22c78174289a2eb10210999c8391a3d
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353839"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="25016-103">Accéder à un calendrier en tant que délégué à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="25016-103">Access a calendar as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="25016-104">Découvrez comment accéder à un calendrier en tant que délégué à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="25016-104">Learn how to access a calendar as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="25016-105">Vous pouvez utiliser l’API managée EWS ou EWS pour donner à un utilisateur délégué l’accès au dossier de calendrier d’un propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-105">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Calendar folder.</span></span> <span data-ttu-id="25016-106">Le délégué peut ensuite créer des demandes de réunion pour le compte du propriétaire de boîte aux lettres, créer des rendez-vous, répondre aux demandes de réunion, extraire et mettre à jour, supprimer des réunions à partir du dossier de calendrier du propriétaire de la boîte aux lettres, en fonction de leurs autorisations.</span><span class="sxs-lookup"><span data-stu-id="25016-106">The delegate can then create meeting requests on behalf of the mailbox owner, create appointments, respond to meeting requests, and retrieve, update, and delete meetings from the mailbox owner's Calendar folder, depending on their permissions.</span></span>
  
<span data-ttu-id="25016-107">En tant que délégué, vous utilisez les mêmes méthodes et opérations pour accéder au dossier calendrier du propriétaire de la boîte aux lettres que vous utilisez pour accéder à votre propre dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="25016-107">As a delegate, you use the same methods and operations to access a mailbox owner's Calendar folder that you use to access your own Calendar folder.</span></span> <span data-ttu-id="25016-108">La principale différence est que vous devez utiliser [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicit) pour trouver ou créer un élément de calendrier ou d’un sous-dossier de calendrier, puis après avoir identifié l’ID d’élément ou dossier, vous pouvez utiliser [un accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) pour obtenir, de mettre à jour ou de supprimer l’élément.</span><span class="sxs-lookup"><span data-stu-id="25016-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a calendar item or calendar subfolder, and then after you identify the item ID or folder ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="25016-109">**Le tableau 1. Méthodes d’API managées et opérations EWS pour accéder à un calendrier en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="25016-109">**Table 1. EWS Managed API methods and EWS operations for accessing a calendar as a delegate**</span></span>

|<span data-ttu-id="25016-110">**Si vous souhaitez...**</span><span class="sxs-lookup"><span data-stu-id="25016-110">**If you want to…**</span></span>|<span data-ttu-id="25016-111">**Utilisez cette méthode d’API managées...**</span><span class="sxs-lookup"><span data-stu-id="25016-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="25016-112">**Utilisez cette opération EWS...**</span><span class="sxs-lookup"><span data-stu-id="25016-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="25016-113">Créer une réunion ou un rendez-vous en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="25016-113">Create a meeting or appointment as a delegate</span></span>  <br/> |<span data-ttu-id="25016-114">[Appointment.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) où le paramètre [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de calendrier du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="25016-114">[Appointment.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="25016-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="25016-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="25016-116">Créer plusieurs réunions ou rendez-vous en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="25016-116">Create multiple meetings or appointments as a delegate</span></span>  <br/> |<span data-ttu-id="25016-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de calendrier du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="25016-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="25016-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="25016-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="25016-119">Recherchez ou rechercher un rendez-vous ou une réunion en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="25016-119">Search for or find an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="25016-120">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit [un accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de calendrier du propriétaire de la boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="25016-120">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="25016-121">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) où l’élément de [boîte aux lettres](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="25016-121">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="25016-122">Obtenir un rendez-vous ou une réunion en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="25016-122">Get an appointment or meeting as a delegate</span></span>  <br/> |[<span data-ttu-id="25016-123">Appointment.Bind</span><span class="sxs-lookup"><span data-stu-id="25016-123">Appointment.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="25016-124">GetItem</span><span class="sxs-lookup"><span data-stu-id="25016-124">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="25016-125">Mettre à jour un rendez-vous ou une réunion en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="25016-125">Update an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="25016-126">[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) suivi [Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="25016-126">[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="25016-127">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="25016-127">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="25016-128">Supprimer un rendez-vous ou une réunion en tant que délégué</span><span class="sxs-lookup"><span data-stu-id="25016-128">Delete an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="25016-129">[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) suivi [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="25016-129">[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="25016-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="25016-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="25016-131">Dans les exemples de code dans cet article, primary@contoso.com est le propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-131">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="25016-132">Les tâches préalables</span><span class="sxs-lookup"><span data-stu-id="25016-132">Prerequisite tasks</span></span>
<span data-ttu-id="25016-133"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="25016-133"></span></span>

<span data-ttu-id="25016-134">Qu’un utilisateur puisse accéder dossier de calendrier d’un propriétaire de boîte aux lettres en tant que délégué, l’utilisateur doit être [ajouté en tant que délégué disposant des autorisations](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) au dossier de calendrier du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-134">Before a user can access a mailbox owner's Calendar folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="25016-135">Un délégué doit avoir une boîte aux lettres associé à leur compte pour mettre à jour le calendrier d’un propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-135">A delegate must have a mailbox attached to their account to update the calendar of a mailbox owner.</span></span>
  
<span data-ttu-id="25016-136">Si un délégué a besoin travailler avec des demandes de réunion et réponses uniquement, vous pouvez ajouter le délégué au dossier de calendrier et utiliser la valeur d’énumération API managées par défaut [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) ou le [ DeliverMeetingRequests](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) valeur de l’élément EWS de **DelegatesAndSendInformationToMe** d’envoyer les demandes au délégué et messages d’information au propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-136">If a delegate needs to work with meeting requests and responses only, you can add the delegate to the Calendar folder, and use the default [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS Managed API enumeration value or the [DeliverMeetingRequests](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) EWS element value of **DelegatesAndSendInformationToMe** to send the requests to the delegate and informational messages to the mailbox owner.</span></span> <span data-ttu-id="25016-137">Puis le délégué n'a pas besoin d’avoir accès au dossier de boîte de réception du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-137">The delegate then does not need to be given access to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="25016-138">Créer une réunion ou un rendez-vous en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="25016-138">Create a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="25016-139"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="25016-139"></span></span>

<span data-ttu-id="25016-140">L’API managée EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour créer des éléments de calendrier pour le propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-140">The EWS Managed API enables you to use the service object for the delegate user to create calendar items for the mailbox owner.</span></span> <span data-ttu-id="25016-141">Cet exemple montre comment utiliser la méthode [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) pour créer une réunion et envoyer les demandes de réunion aux participants.</span><span class="sxs-lookup"><span data-stu-id="25016-141">This example shows how to use the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="25016-142">Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le délégué et le délégué a été accordé les autorisations appropriées pour le dossier de calendrier du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-142">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Calendar folder.</span></span> 
  
```cs
private static void DelegateAccessCreateMeeting(ExchangeService service)
{
    Appointment meeting = new Appointment(service);
    // Set the properties on the meeting object to create the meeting.
    meeting.Subject = "Team building exercise";
    meeting.Body = "Let's learn to really work as a team and then have lunch!";
    meeting.Start = DateTime.Now.AddDays(2);
    meeting.End = meeting.Start.AddHours(4);
    meeting.Location = "Conference Room 12";
    meeting.RequiredAttendees.Add("sadie@contoso.com");
    meeting.ReminderMinutesBeforeStart = 60;
    // Save the meeting to the Calendar folder for 
    // the mailbox owner and send the meeting request.
    // This method call results in a CreateItem call to EWS.
    meeting.Save(new FolderId(WellKnownFolderName.Calendar, 
        "primary@contoso.com"), 
        SendInvitationsMode.SendToAllAndSaveCopy);
    // Verify that the meeting was created.
    Item item = Item.Bind(service, meeting.Id, new PropertySet(ItemSchema.Subject));
    Console.WriteLine("\nMeeting created: " + item.Subject + "\n");
}
```

<span data-ttu-id="25016-143">Notez que lorsque vous enregistrez l’élément, l’appel de méthode [Enregistrer](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) doit identifier le dossier de calendrier du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-143">Note that when you save the item, the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="25016-144">Si le dossier de calendrier du propriétaire de la boîte aux lettres n’est pas spécifié, la demande de réunion est enregistrée pour le calendrier du délégué et non le dossier de calendrier du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-144">If the mailbox owner's Calendar folder is not specified, the meeting request gets saved to the delegate's calendar and not the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="25016-145">Vous pouvez inclure le dossier de calendrier du propriétaire de la boîte aux lettres dans l’appel de méthode **Enregistrer** de deux manières.</span><span class="sxs-lookup"><span data-stu-id="25016-145">You can include the mailbox owner's Calendar folder in the **Save** method call in two ways.</span></span> <span data-ttu-id="25016-146">Il est recommandé que vous instanciez une nouvelle instance de l’objet [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) à l’aide de la [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et l’adresse SMTP du propriétaire de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-146">We recommend that you instantiate a new instance of the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

<span data-ttu-id="25016-147">Toutefois, vous pouvez également [lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) au dossier de calendrier tout d’abord, puis utilisez l’ID du dossier de l’appel de méthode **Enregistrer** .</span><span class="sxs-lookup"><span data-stu-id="25016-147">However, you can also [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Calendar folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="25016-148">Sachez, toutefois, que cette opération crée un appel EWS supplémentaire.</span><span class="sxs-lookup"><span data-stu-id="25016-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
```cs
    // Identify the mailbox owner's SMTP address
    // and bind to their Calendar folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryCalendar = Folder.Bind(service, 
        new FolderId(WellKnownFolderName.Calendar, primary)); 
…
    // Save the meeting to the Calendar folder for the mailbox owner and send the meeting request.
    meeting.Save(primaryCalendar.Id, 
        SendInvitationsMode.SendToAllAndSaveCopy);
```

## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="25016-149">Créer une réunion ou un rendez-vous en tant que délégué à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="25016-149">Create a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="25016-150"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="25016-150"></span></span>

<span data-ttu-id="25016-151">EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour créer des éléments de calendrier pour le propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-151">EWS enables you to use the service object for the delegate user to create calendar items for the mailbox owner.</span></span> <span data-ttu-id="25016-152">Cet exemple montre comment utiliser l’opération [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour créer une réunion et envoyer les demandes de réunion aux participants.</span><span class="sxs-lookup"><span data-stu-id="25016-152">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="25016-153">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **Save** pour [créer une réunion ou un rendez-vous en tant que délégué](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="25016-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a meeting or appointment as a delegate](#bk_createewsma).</span></span>
  
<span data-ttu-id="25016-154">L’en-tête SOAP a été supprimée de l’exemple suivant par souci de concision.</span><span class="sxs-lookup"><span data-stu-id="25016-154">The SOAP header has been removed from the following example for brevity.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
         xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
…
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Team building exercise</t:Subject>
          <t:Body BodyType="HTML">Let's learn to really work as a 
              team and then have lunch!</t:Body>
          <t:ReminderMinutesBeforeStart>60</t:ReminderMinutesBeforeStart>
          <t:Start>2014-03-09T23:26:33.756-05:00</t:Start>
          <t:End>2014-03-10T03:26:33.756-05:00</t:End>
          <t:Location>Conference Room 12</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="25016-155">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que la réunion a été créée avec succès.</span><span class="sxs-lookup"><span data-stu-id="25016-155">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the meeting was created successfully.</span></span> <span data-ttu-id="25016-156">La réponse contient également l’ID d’élément de la réunion nouvellement créée.</span><span class="sxs-lookup"><span data-stu-id="25016-156">The response also contains the item ID of the newly created meeting.</span></span>
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="25016-157">Rechercher une réunion ou un rendez-vous en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="25016-157">Search for a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="25016-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="25016-158"></span></span>

<span data-ttu-id="25016-159">Pour rechercher une réunion, vous devez utiliser une des méthodes [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) qui comprend un paramètre [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , afin que vous pouvez spécifier le dossier de calendrier du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-159">To search for a meeting, you must use one of the [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Calendar folder.</span></span> 
  
```cs
static void DelegateAccessSearchWithFilter
    (ExchangeService service, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Define the sort order.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Call FindItems to find matching calendar items. 
        // The FindItems parameters must denote the mailbox owner,
        // mailbox, and Calendar folder.
        // This method call results in a FindItem call to EWS.
        FindItemsResults<Item> results = service.FindItems(
        new FolderId(WellKnownFolderName.Calendar, 
            "primary@contoso.com"), 
            filter, 
            view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while 
            enumerating results: {0}", ex.Message);
    }
}
```

<span data-ttu-id="25016-160">Une fois l’appel **FindItems** retourne une réponse avec un ID, vous pouvez obtenir, mettre à jour ou supprimer cette réunion à l’aide de l’ID et [l’accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) — et vous n’avez pas besoin de spécifier l’adresse SMTP de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that meeting by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="25016-161">Rechercher une réunion ou un rendez-vous en tant que délégué à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="25016-161">Search for a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="25016-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="25016-162"></span></span>

<span data-ttu-id="25016-163">EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué pour rechercher des rendez-vous et réunions répondant à un ensemble de critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="25016-163">EWS enables you to use the service object for the delegate user to search for appointments and meetings that meet a set of search criteria.</span></span> <span data-ttu-id="25016-164">Cet exemple montre comment utiliser l’opération [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour rechercher des réunions dans le dossier calendrier du propriétaire de la boîte aux lettres qui contiennent le mot « building » dans l’objet.</span><span class="sxs-lookup"><span data-stu-id="25016-164">This example shows how to use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Calendar folder that contain the word "building" in the subject.</span></span> 
  
<span data-ttu-id="25016-165">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez la méthode **FindItem** au [service de recherche pour une réunion ou un rendez-vous en tant que délégué](#bk_searchewsma).</span><span class="sxs-lookup"><span data-stu-id="25016-165">This is also the XML request that the EWS Managed API sends when you use the **FindItem** method to [search for a meeting or appointment as a delegate](#bk_searchewsma).</span></span>
  
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
          <t:Constant Value="building" />
        </t:Contains>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="25016-166">Le serveur répond à la demande **FindItem** avec un message [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) qui contient une valeur élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, qui indique que la recherche s’est terminée correctement.</span><span class="sxs-lookup"><span data-stu-id="25016-166">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully.</span></span> <span data-ttu-id="25016-167">La réponse contient un [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) pour un rendez-vous ou les réunions qui répondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="25016-167">The response contains a [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) for any appointments or meetings that met the search criteria.</span></span> <span data-ttu-id="25016-168">Dans ce cas, seule réunion est trouvée.</span><span class="sxs-lookup"><span data-stu-id="25016-168">In this case, only one meeting is found.</span></span> 
  
<span data-ttu-id="25016-169">La valeur de l’élément [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="25016-169">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="10"
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
              <t:CalendarItem>
                <t:ItemId Id="IJpUAAA="
                          ChangeKey="DwAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAAAIKhS" />
                <t:Subject>Team building exercise</t:Subject>
                <t:DateTimeReceived>2014-03-04T21:27:22Z</t:DateTimeReceived>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="25016-170">Maintenant que vous avez l' **ItemId** de la réunion qui répond à vos critères, vous pouvez obtenir, mettre à jour ou supprimer cette réunion à l’aide de **l’ItemId** et [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) — et vous n’avez pas besoin de spécifier l’adresse SMTP de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-170">Now that you have the **ItemId** for the meeting that meets your criteria, you can get, update, or delete that meeting by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="25016-171">Obtenir, mettre à jour ou supprimer des éléments de calendrier en tant que délégué à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="25016-171">Get, update, or delete calendar items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="25016-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="25016-172"></span></span>

<span data-ttu-id="25016-173">Vous pouvez utiliser l’API managée EWS pour obtenir, mettre à jour ou supprimer une réunion ou un rendez-vous de la même manière que vous effectuez ces actions lorsque vous n’utilisez pas d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="25016-173">You can use the EWS Managed API to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="25016-174">La seule différence est que l’objet de service pour l’utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="25016-174">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="25016-175">L’ID d’élément inclus dans l’appel de méthode **lier** unique identifie l’élément dans le magasin de boîte aux lettres, dans le dossier de calendrier du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-175">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="25016-176">**Le tableau 2. Méthodes d’API managées pour travailler avec des rendez-vous et réunions en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="25016-176">**Table 2. EWS Managed API methods for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="25016-177">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="25016-177">**Task**</span></span>|<span data-ttu-id="25016-178">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="25016-178">**EWS Managed API method**</span></span>|<span data-ttu-id="25016-179">**Code example**</span><span class="sxs-lookup"><span data-stu-id="25016-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="25016-180">Obtenir un rendez-vous ou une réunion</span><span class="sxs-lookup"><span data-stu-id="25016-180">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="25016-181">Créer une liaison</span><span class="sxs-lookup"><span data-stu-id="25016-181">Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="25016-182">Obtention d’un élément à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="25016-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="25016-183">Mettre à jour un rendez-vous ou une réunion</span><span class="sxs-lookup"><span data-stu-id="25016-183">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="25016-184">[Lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) le suivi de [mise à jour](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="25016-184">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="25016-185">Mettre à jour une réunion à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="25016-185">Update a meeting by using the EWS Managed API</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|<span data-ttu-id="25016-186">Supprimer un rendez-vous ou une réunion</span><span class="sxs-lookup"><span data-stu-id="25016-186">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="25016-187">[Lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) suivie à [Supprimer](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="25016-187">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="25016-188">Supprimer une réunion à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="25016-188">Delete a meeting by using the EWS Managed API</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="25016-189">Obtenir, mettre à jour ou supprimer des éléments de calendrier en tant que délégué à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="25016-189">Get, update, or delete calendar items as a delegate by using EWS</span></span>
<span data-ttu-id="25016-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="25016-190"></span></span>

<span data-ttu-id="25016-191">Vous pouvez utiliser EWS pour obtenir, mettre à jour ou supprimer une réunion ou un rendez-vous de la même manière que vous effectuez ces actions lorsque vous n’utilisez pas d’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="25016-191">You can use EWS to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="25016-192">La seule différence est que l’objet de service pour l’utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="25016-192">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="25016-193">L’ID d’élément inclus dans l’appel de méthode [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) unique identifie l’élément dans le magasin de boîte aux lettres, dans le dossier de calendrier du propriétaire de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="25016-193">The item ID included in the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="25016-194">**Le tableau 3. Opérations EWS pour travailler avec des rendez-vous et réunions en tant que délégué**</span><span class="sxs-lookup"><span data-stu-id="25016-194">**Table 3. EWS operations for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="25016-195">**Tâche**</span><span class="sxs-lookup"><span data-stu-id="25016-195">**Task**</span></span>|<span data-ttu-id="25016-196">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="25016-196">**EWS operation**</span></span>|<span data-ttu-id="25016-197">**Code example**</span><span class="sxs-lookup"><span data-stu-id="25016-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="25016-198">Obtenir un rendez-vous ou une réunion</span><span class="sxs-lookup"><span data-stu-id="25016-198">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="25016-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="25016-199">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="25016-200">Obtention d’un élément à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="25016-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="25016-201">Mettre à jour un rendez-vous ou une réunion</span><span class="sxs-lookup"><span data-stu-id="25016-201">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="25016-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="25016-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="25016-203">Mettre à jour une réunion à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="25016-203">Update a meeting by using EWS</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|<span data-ttu-id="25016-204">Supprimer un rendez-vous ou une réunion</span><span class="sxs-lookup"><span data-stu-id="25016-204">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="25016-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="25016-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25016-206">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="25016-206">See also</span></span>

- [<span data-ttu-id="25016-207">Accès délégué et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="25016-207">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="25016-208">Ajouter et supprimer des délégués à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="25016-208">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="25016-209">Définir des autorisations de dossier pour un autre utilisateur à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="25016-209">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="25016-210">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="25016-210">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

