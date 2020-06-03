---
title: Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 42412265-3968-468a-a8c2-7e8af3c6deb9
description: Découvrez comment supprimer des rendez-vous et des réunions à l’aide de l’API managée EWS ou EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 6a2fdaa357f4088da4bbd0643187d05a5bc51c0c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528131"
---
# <a name="delete-appointments-and-cancel-meetings-by-using-ews-in-exchange"></a><span data-ttu-id="70115-103">Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="70115-103">Delete appointments and cancel meetings by using EWS in Exchange</span></span>

<span data-ttu-id="70115-104">Découvrez comment supprimer des rendez-vous et des réunions à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="70115-104">Learn how to delete appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="70115-p101">La principale différence entre les réunions et les rendez-vous réside dans la présence de participants aux réunions, mais pas aux rendez-vous. Les rendez-vous et les réunions peuvent être des instances uniques ou faire partie d'une série périodique. Cependant, les rendez-vous n'incluant ni participants, ni salles, ni ressources, ne nécessitent pas l'envoi d'un message. En interne, Exchange utilise le même objet pour les réunions et pour les rendez-vous. Pour utiliser les réunions et les rendez-vous, vous devez utiliser la classe [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) de l'API managée EWS ou l'élément [CalendarItem](https://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) d'EWS.</span><span class="sxs-lookup"><span data-stu-id="70115-p101">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't. Both appointments and meetings can be single instances or part of a recurring series, but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent. Internally, Exchange uses the same object for both meetings and appointments. You use the EWS Managed API [Appointment class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](https://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="70115-109">**Tableau 1. Méthodes d’API managée EWS et opérations EWS pour la suppression de rendez-vous et de réunions**</span><span class="sxs-lookup"><span data-stu-id="70115-109">**Table 1. EWS Managed API methods and EWS operations for deleting appointments and meetings**</span></span>

|<span data-ttu-id="70115-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="70115-110">**EWS Managed API method**</span></span>|<span data-ttu-id="70115-111">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="70115-111">**EWS Operation**</span></span>|<span data-ttu-id="70115-112">**Fonction**</span><span class="sxs-lookup"><span data-stu-id="70115-112">**What it does**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="70115-113">Rendez-vous. Delete</span><span class="sxs-lookup"><span data-stu-id="70115-113">Appointment.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="70115-114">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="70115-114">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |<span data-ttu-id="70115-115">Supprime un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="70115-115">Deletes an appointment.</span></span>  <br/> |
|[<span data-ttu-id="70115-116">Rendez-vous. Delete</span><span class="sxs-lookup"><span data-stu-id="70115-116">Appointment.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="70115-117">CreateItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="70115-117">CreateItem (calendar item)</span></span>](../web-service-reference/createitem-operation-calendar-item.md) <br/> |<span data-ttu-id="70115-118">Supprime une réunion.</span><span class="sxs-lookup"><span data-stu-id="70115-118">Deletes a meeting.</span></span>  <br/> |
   
<span data-ttu-id="70115-119">Notez que lorsque vous supprimez un rendez-vous à l’aide d’EWS, vous utilisez l’opération [DeleteItem](../web-service-reference/deleteitem-operation.md) , mais lorsque vous supprimez une réunion, vous utilisez l’opération [CreateItem](../web-service-reference/createitem-operation-calendar-item.md) .</span><span class="sxs-lookup"><span data-stu-id="70115-119">Note that when you delete an appointment by using EWS, you use the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation, but when you delete a meeting, you use the [CreateItem](../web-service-reference/createitem-operation-calendar-item.md) operation.</span></span> <span data-ttu-id="70115-120">Cela peut sembler counterintuitive, mais vous devez créer un objet de réponse à une réunion pour envoyer des messages d’annulation de réunion aux participants.</span><span class="sxs-lookup"><span data-stu-id="70115-120">This might seem counterintuitive, but it is because you have to create a meeting response object to send meeting cancellation messages to attendees.</span></span> 

<span data-ttu-id="70115-121"><a name="bk_DeleteApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="70115-121"><a name="bk_DeleteApptEWSMA"> </a></span></span>

## <a name="delete-an-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="70115-122">Supprimer un rendez-vous à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="70115-122">Delete an appointment by using the EWS Managed API</span></span>

<span data-ttu-id="70115-123">L’exemple de code suivant montre comment utiliser la méthode [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) pour supprimer un rendez-vous de votre dossier de calendrier, et la méthode [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) pour vérifier que le rendez-vous a été supprimé en le recherchant dans le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="70115-123">The following code example shows how to use the [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method to delete an appointment from your calendar folder, and the [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method to verify that the appointment was deleted by looking for it in the Deleted Items folder.</span></span> 
  
<span data-ttu-id="70115-124">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="70115-124">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="70115-125">La variable locale `appointmentId` est un identificateur associé à un rendez-vous existant.</span><span class="sxs-lookup"><span data-stu-id="70115-125">The local variable  `appointmentId` is an identifier associated with an existing appointment.</span></span> 
  
```cs
// Instantiate an appointment object by binding to it by using the ItemId.
// As a best practice, limit the properties returned to only the ones you need.
Appointment appointment = Appointment.Bind(service, appointmentId, new PropertySet());
// Delete the appointment. Note that the item ID will change when the item is moved to the Deleted Items folder.
appointment.Delete(DeleteMode.MoveToDeletedItems);
// Verify that the appointment has been deleted by looking for a matching subject in the Deleted Items folder's first entry.
ItemView itemView = new ItemView(1);
itemView.Traversal = ItemTraversal.Shallow;
// Just retrieve the properties you need.
itemView.PropertySet = new PropertySet(ItemSchema.Id, ItemSchema.ParentFolderId, ItemSchema.Subject);
// Note that the FindItems method results in a call to EWS.
FindItemsResults<Item> deletedItems = service.FindItems(WellKnownFolderName.DeletedItems, itemView);
Item deletedItem = deletedItems.First();
Folder parentFolder = Folder.Bind(service, deletedItem.ParentFolderId, new PropertySet(FolderSchema.DisplayName));
Console.WriteLine("The appointment " + "\"" + deletedItem.Subject + "\"" + " is now in the " + parentFolder.DisplayName + " folder.");

```

<span data-ttu-id="70115-126">Cet exemple montre un moyen simple de vérifier que le rendez-vous a été supprimé, en vérifiant que l’objet du premier élément dans le dossier éléments supprimés correspond à celui du rendez-vous supprimé.</span><span class="sxs-lookup"><span data-stu-id="70115-126">This example shows a simple way to verify that the appointment was deleted, by verifying that the subject of the first item in the Deleted Items folder matches that of the deleted appointment.</span></span> <span data-ttu-id="70115-127">La manière dont vous choisissez de vérifier que votre rendez-vous a été supprimé dépend des besoins de votre application.</span><span class="sxs-lookup"><span data-stu-id="70115-127">How you choose to verify that your appointment was deleted will vary based the needs of your application.</span></span>
  
<span data-ttu-id="70115-128">Comme vous pouvez le constater, la suppression d’un rendez-vous est simple et à peu près ce que vous pouvez attendre.</span><span class="sxs-lookup"><span data-stu-id="70115-128">As you can see, deleting an appointment is straightforward and pretty much what you might expect.</span></span> <span data-ttu-id="70115-129">Remarque Lorsque vous créez votre étape de vérification que l’élément de rendez-vous dans le dossier éléments supprimés a un ItemId différent de celui de l’élément de rendez-vous dans le dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="70115-129">Note when you create your verification step that the appointment item in the Deleted Items folder has a different ItemId than the appointment item in the calendar folder.</span></span> <span data-ttu-id="70115-130">L’élément est copié et supprimé au lieu d’être déplacé vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="70115-130">The item is copied and deleted rather than simply moved to the Deleted Items folder.</span></span> 
  
## <a name="delete-an-appointment-by-using-ews"></a><span data-ttu-id="70115-131">Supprimer un rendez-vous à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="70115-131">Delete an appointment by using EWS</span></span>
<span data-ttu-id="70115-132"><a name="bk_DeleteApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="70115-132"><a name="bk_DeleteApptEWSMA"> </a></span></span>

<span data-ttu-id="70115-133">Les codes XML de demande et de réponse dans les exemples suivants correspondent aux appels effectués par le code de l’API managée EWS dans Delete a appointment [by using the EWS Managed API](#bk_DeleteApptEWSMA).</span><span class="sxs-lookup"><span data-stu-id="70115-133">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Delete an appointment by using the EWS Managed API](#bk_DeleteApptEWSMA).</span></span> <span data-ttu-id="70115-134">Le code XML de demande et de réponse qui vérifie que l’élément de rendez-vous se trouve dans le dossier éléments supprimés est également affiché.</span><span class="sxs-lookup"><span data-stu-id="70115-134">The request and response XML that verifies that the appointment item is in the Deleted Items folder is shown as well.</span></span>
  
<span data-ttu-id="70115-135">L’exemple suivant montre le code XML de demande pour l’opération [DeleteItem](../web-service-reference/deleteitem-operation.md) afin de supprimer un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="70115-135">The following example shows the request XML for the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation to delete an appointment.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems" SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="70115-136">L’exemple suivant montre le code XML de réponse renvoyé par l’opération [DeleteItem](../web-service-reference/deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="70115-136">The following example shows the response XML that is returned by the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation.</span></span> <span data-ttu-id="70115-137">Les attributs **ItemId** et **ChangeKey** sont raccourcis pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="70115-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </m:DeleteItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="70115-138">L’exemple suivant montre le code XML de demande pour l’opération [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) qui récupère le premier élément dans le dossier éléments supprimés afin de comparer l’objet de l’élément avec celui de l’objet de rendez-vous supprimé.</span><span class="sxs-lookup"><span data-stu-id="70115-138">The following example shows the request XML for the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation that retrieves the first item in the Deleted Items folder in order to compare the item's subject with that of the deleted appointment object.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages
" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ItemId" />
          <t:FieldURI FieldURI="item:ParentFolderId" />
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="70115-139">L’exemple suivant montre le code XML de réponse renvoyé par l’opération [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) au cours de l’étape de vérification.</span><span class="sxs-lookup"><span data-stu-id="70115-139">The following example shows the response XML that is returned by the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation during the verification step.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="70115-140">Les attributs **ItemId** et **ChangeKey** sont raccourcis pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="70115-140">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="10748" IncludesLastItemInRange="false">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkA=" ChangeKey="DwAAA" />
                <t:ParentFolderId Id="AAMkA" ChangeKey="AQAAA" />
                <t:Subject>Tennis lesson</t:Subject>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="70115-141"><a name="bk_DeleteMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="70115-141"><a name="bk_DeleteMtgEWSMA"> </a></span></span>

## <a name="delete-a-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="70115-142">Supprimer une réunion à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="70115-142">Delete a meeting by using the EWS Managed API</span></span>

<span data-ttu-id="70115-143">Lorsque vous supprimez une réunion, outre la suppression de l’élément de rendez-vous du dossier calendrier, vous pouvez également envoyer des annulations de réunion aux participants.</span><span class="sxs-lookup"><span data-stu-id="70115-143">When you delete a meeting, in addition to removing the appointment item from the calendar folder, you might also want to send meeting cancellations to attendees.</span></span> <span data-ttu-id="70115-144">Vous pouvez utiliser les trois méthodes suivantes pour annuler une réunion :</span><span class="sxs-lookup"><span data-stu-id="70115-144">You can use the following three methods to cancel a meeting:</span></span>
  
- [<span data-ttu-id="70115-145">Rendez-vous. Delete</span><span class="sxs-lookup"><span data-stu-id="70115-145">Appointment.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="70115-146">Appointment. CancelMeeting</span><span class="sxs-lookup"><span data-stu-id="70115-146">Appointment.CancelMeeting</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="70115-147">CancelMeetingMessage</span><span class="sxs-lookup"><span data-stu-id="70115-147">CancelMeetingMessage</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx)
    
<span data-ttu-id="70115-148">La méthode que vous choisissez dépend du niveau de détail que vous devez fournir dans votre message d’annulation.</span><span class="sxs-lookup"><span data-stu-id="70115-148">The method that you choose depends on the level of detail you need to provide in your cancellation message.</span></span> <span data-ttu-id="70115-149">[Rendez-vous. CancelMeeting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) facilite la mise à jour du message d’annulation en transmettant un message mis à jour en tant que paramètre.</span><span class="sxs-lookup"><span data-stu-id="70115-149">[Appointment.CancelMeeting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) makes it easy to update the cancellation message by passing an updated message as a parameter.</span></span> <span data-ttu-id="70115-150">[CancelMeetingMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx) vous permet de modifier les propriétés de votre message avant d’envoyer une annulation, afin que vous puissiez effectuer des actions comme demander un accusé de réception.</span><span class="sxs-lookup"><span data-stu-id="70115-150">[CancelMeetingMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx) allows you to modify properties on your message before sending a cancellation, so you can do things like request a receipt.</span></span> 
  
<span data-ttu-id="70115-151">Les exemples de code de cette section présentent les différentes façons de supprimer une réunion et d’envoyer des annulations de réunion.</span><span class="sxs-lookup"><span data-stu-id="70115-151">The code examples in this section show the different ways to delete a meeting and send meeting cancellations.</span></span> <span data-ttu-id="70115-152">Les exemples partent du principe que vous avez été authentifié auprès d’un serveur Exchange et que vous avez acquis un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) nommé **service**.</span><span class="sxs-lookup"><span data-stu-id="70115-152">The examples assume that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="70115-153">La variable locale `meetingId` est un identificateur associé à une réunion existante où l’utilisateur cible est l’organisateur de la réunion.</span><span class="sxs-lookup"><span data-stu-id="70115-153">The local variable  `meetingId` is an identifier associated with an existing meeting where the target user is the meeting organizer.</span></span> 
  
<span data-ttu-id="70115-154">L’exemple de code suivant montre comment supprimer une réunion à l’aide de la méthode appointment [. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="70115-154">The following code example shows how to delete a meeting by using the [Appointment.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method.</span></span> 
  
```cs
// Instantiate an appointment object for the meeting by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
            
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the Delete method.
meeting.Delete(DeleteMode.MoveToDeletedItems, SendCancellationsMode.SendToAllAndSaveCopy);
// Verify that the meeting has been deleted by looking for a matching subject in the Deleted Items folder's first entry.
ItemView itemView = new ItemView(1);
itemView.Traversal = ItemTraversal.Shallow;
// Just retrieve the properties you need.
itemView.PropertySet = new PropertySet(ItemSchema.Id, ItemSchema.ParentFolderId, ItemSchema.Subject);
// Note that the FindItems method results in a call to EWS.
FindItemsResults<Item> deletedItems = service.FindItems(WellKnownFolderName.DeletedItems, itemView);
Item deletedItem = deletedItems.First();
Folder parentFolder = Folder.Bind(service, deletedItem.ParentFolderId, new PropertySet(FolderSchema.DisplayName));
Console.WriteLine("The meeting " + "\"" + deletedItem.Subject + "\"" + " is now in the " + parentFolder.DisplayName + " folder.");

```

<span data-ttu-id="70115-155">L’exemple de code suivant montre comment supprimer une réunion à l’aide de la méthode [CancelMeeting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="70115-155">The following code example shows how to delete a meeting by using the [CancelMeeting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) method.</span></span> 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the CancelMeeting method.
meeting.CancelMeeting("The outdoor meeting has been cancelled due to hailstorms.");

```

<span data-ttu-id="70115-156">L’exemple de code suivant montre comment supprimer une réunion à l’aide de la méthode appointment [. CreateCancelMeetingMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="70115-156">The following code example shows how to delete a meeting by using the [Appointment.CreateCancelMeetingMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx) method.</span></span> 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the CreateCancelMeetingMessage method.
CancelMeetingMessage cancelMessage = meeting.CreateCancelMeetingMessage();
cancelMessage.Body = new MessageBody("The outdoor meeting has been canceled due to hailstorms.");
cancelMessage.IsReadReceiptRequested = true;
cancelMessage.SendAndSaveCopy();

```

## <a name="delete-a-meeting-by-using-ews"></a><span data-ttu-id="70115-157">Supprimer une réunion à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="70115-157">Delete a meeting by using EWS</span></span>
<span data-ttu-id="70115-158"><a name="bk_EWSDeleteApptAndMeeting"> </a></span><span class="sxs-lookup"><span data-stu-id="70115-158"><a name="bk_EWSDeleteApptAndMeeting"> </a></span></span>

<span data-ttu-id="70115-159">Les codes XML de demande et de réponse dans les exemples suivants correspondent aux appels effectués par le code de l’API managée EWS dans [Delete a Meeting using the EWS Managed API](#bk_DeleteMtgEWSMA) by using the appointment [. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) , méthode.</span><span class="sxs-lookup"><span data-stu-id="70115-159">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Delete a meeting by using the EWS Managed API](#bk_DeleteMtgEWSMA) by using the [Appointment.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="70115-160">L’exemple suivant montre le code XML de requête lorsque vous utilisez l’opération [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour envoyer des messages d’annulation aux participants et supprimer une réunion.</span><span class="sxs-lookup"><span data-stu-id="70115-160">The following example shows the request XML when you use the [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to send cancellation messages to attendees and delete a meeting.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:CancelCalendarItem>
          <t:ReferenceItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:NewBodyContent BodyType="HTML">The outdoor meeting has been canceled due to hailstorms.</t:NewBodyContent>
        </t:CancelCalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="70115-161">L’exemple suivant montre le code XML renvoyé en réponse à une demande d’opération [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) utilisée pour supprimer une réunion.</span><span class="sxs-lookup"><span data-stu-id="70115-161">The following example shows the XML that is returned in response to a [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation request used to delete a meeting.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="70115-162">Les attributs **ItemId** et **ChangeKey** sont raccourcis pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="70115-162">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="70115-163">L’exemple suivant montre le code XML de demande pour l’opération [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) qui récupère le premier élément dans le dossier éléments supprimés afin de comparer l’objet de l’élément avec celui de l’objet de rendez-vous supprimé.</span><span class="sxs-lookup"><span data-stu-id="70115-163">The following example shows the request XML for the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation that retrieves the first item in the Deleted Items folder in order to compare the item's subject with that of the deleted appointment object.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ItemId" />
          <t:FieldURI FieldURI="item:ParentFolderId" />
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="70115-164">L’exemple suivant montre le code XML renvoyé par l’opération [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) au cours de l’étape de vérification.</span><span class="sxs-lookup"><span data-stu-id="70115-164">The following example shows the XML that is returned by the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation during the verification step.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="70115-165">Les attributs **ID** et **ChangeKey** sont raccourcis pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="70115-165">The **Id** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="10750" IncludesLastItemInRange="false">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
                <t:ParentFolderId Id="AAMkA" ChangeKey="AQAAA" />
                <t:Subject>Team building exercise</t:Subject>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="70115-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="70115-166">See also</span></span>

- [<span data-ttu-id="70115-167">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="70115-167">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)    
- [<span data-ttu-id="70115-168">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="70115-168">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)  
- [<span data-ttu-id="70115-169">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="70115-169">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="70115-170">Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="70115-170">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="70115-171">Proposer une nouvelle heure de réunion à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="70115-171">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="70115-172">Proposer une nouvelle heure de réunion à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="70115-172">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    

