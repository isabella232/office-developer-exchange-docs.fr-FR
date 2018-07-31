---
title: Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 42412265-3968-468a-a8c2-7e8af3c6deb9
description: Découvrez comment supprimer des rendez-vous et réunions à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: c71272bf753432a9f343adc917b444424fe3ba33
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354077"
---
# <a name="delete-appointments-and-cancel-meetings-by-using-ews-in-exchange"></a><span data-ttu-id="e28fe-103">Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e28fe-103">Delete appointments and cancel meetings by using EWS in Exchange</span></span>

<span data-ttu-id="e28fe-104">Découvrez comment supprimer des rendez-vous et réunions à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="e28fe-104">Learn how to delete appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="e28fe-p101">La principale différence entre les réunions et les rendez-vous réside dans la présence de participants aux réunions, mais pas aux rendez-vous. Les rendez-vous et les réunions peuvent être des instances uniques ou faire partie d'une série périodique. Cependant, les rendez-vous n'incluant ni participants, ni salles, ni ressources, ne nécessitent pas l'envoi d'un message. En interne, Exchange utilise le même objet pour les réunions et pour les rendez-vous. Pour utiliser les réunions et les rendez-vous, vous devez utiliser la classe [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) de l'API managée EWS ou l'élément [CalendarItem](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) d'EWS.</span><span class="sxs-lookup"><span data-stu-id="e28fe-p101">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't. Both appointments and meetings can be single instances or part of a recurring series, but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent. Internally, Exchange uses the same object for both meetings and appointments. You use the EWS Managed API [Appointment class](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="e28fe-109">**Le tableau 1. Méthodes d’API managées et opérations EWS pour supprimer des rendez-vous et réunions**</span><span class="sxs-lookup"><span data-stu-id="e28fe-109">**Table 1. EWS Managed API methods and EWS operations for deleting appointments and meetings**</span></span>

|<span data-ttu-id="e28fe-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="e28fe-110">**EWS Managed API method**</span></span>|<span data-ttu-id="e28fe-111">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="e28fe-111">**EWS Operation**</span></span>|<span data-ttu-id="e28fe-112">**Fonction**</span><span class="sxs-lookup"><span data-stu-id="e28fe-112">**What it does**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="e28fe-113">Appointment.Delete</span><span class="sxs-lookup"><span data-stu-id="e28fe-113">Appointment.Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="e28fe-114">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="e28fe-114">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |<span data-ttu-id="e28fe-115">Supprime un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="e28fe-115">Deletes an appointment.</span></span>  <br/> |
|[<span data-ttu-id="e28fe-116">Appointment.Delete</span><span class="sxs-lookup"><span data-stu-id="e28fe-116">Appointment.Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="e28fe-117">CreateItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="e28fe-117">CreateItem (calendar item)</span></span>](../web-service-reference/createitem-operation-calendar-item.md) <br/> |<span data-ttu-id="e28fe-118">Supprime une réunion.</span><span class="sxs-lookup"><span data-stu-id="e28fe-118">Deletes a meeting.</span></span>  <br/> |
   
<span data-ttu-id="e28fe-119">Notez que lorsque vous supprimez un rendez-vous à l’aide de EWS, vous utilisez l’opération [DeleteItem](../web-service-reference/deleteitem-operation.md) , mais lorsque vous supprimez une réunion, vous utilisez l’opération [CreateItem](../web-service-reference/createitem-operation-calendar-item.md) .</span><span class="sxs-lookup"><span data-stu-id="e28fe-119">Note that when you delete an appointment by using EWS, you use the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation, but when you delete a meeting, you use the [CreateItem](../web-service-reference/createitem-operation-calendar-item.md) operation.</span></span> <span data-ttu-id="e28fe-120">Cela peut sembler intuitive, mais c’est parce que vous devez créer une réunion des messages d’objet response pour envoyer l’annulation de réunion aux participants.</span><span class="sxs-lookup"><span data-stu-id="e28fe-120">This might seem counterintuitive, but it is because you have to create a meeting response object to send meeting cancellation messages to attendees.</span></span> 

<span data-ttu-id="e28fe-121"><a name="bk_DeleteApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="e28fe-121"></span></span>

## <a name="delete-an-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="e28fe-122">Supprimer un rendez-vous à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="e28fe-122">Delete an appointment by using the EWS Managed API</span></span>

<span data-ttu-id="e28fe-123">L’exemple de code suivant montre comment utiliser la méthode [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) pour supprimer un rendez-vous de votre dossier de calendrier et la méthode [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) pour vérifier que le rendez-vous a été supprimé en recherchant dans le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="e28fe-123">The following code example shows how to use the [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method to delete an appointment from your calendar folder, and the [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method to verify that the appointment was deleted by looking for it in the Deleted Items folder.</span></span> 
  
<span data-ttu-id="e28fe-124">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="e28fe-124">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="e28fe-125">La variable locale `appointmentId` est un identificateur associé à un rendez-vous existant.</span><span class="sxs-lookup"><span data-stu-id="e28fe-125">The local variable  `appointmentId` is an identifier associated with an existing appointment.</span></span> 
  
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

<span data-ttu-id="e28fe-126">Cet exemple montre un moyen simple pour vérifier que le rendez-vous a été supprimé, en vérifiant que l’objet du premier élément dans le dossier éléments supprimés correspond à qui le rendez-vous supprimé.</span><span class="sxs-lookup"><span data-stu-id="e28fe-126">This example shows a simple way to verify that the appointment was deleted, by verifying that the subject of the first item in the Deleted Items folder matches that of the deleted appointment.</span></span> <span data-ttu-id="e28fe-127">Comment vous choisissez vérifier que vos rendez-vous a été supprimé varie en fonction des besoins de votre application.</span><span class="sxs-lookup"><span data-stu-id="e28fe-127">How you choose to verify that your appointment was deleted will vary based the needs of your application.</span></span>
  
<span data-ttu-id="e28fe-128">Comme vous pouvez le constater, la suppression d’un rendez-vous est simple et pratiquement ce que vous attendez.</span><span class="sxs-lookup"><span data-stu-id="e28fe-128">As you can see, deleting an appointment is straightforward and pretty much what you might expect.</span></span> <span data-ttu-id="e28fe-129">Remarque Lorsque vous créez votre étape de vérification que l’élément de rendez-vous dans le dossier éléments supprimés a un ItemId autre que l’élément de rendez-vous dans le dossier calendrier.</span><span class="sxs-lookup"><span data-stu-id="e28fe-129">Note when you create your verification step that the appointment item in the Deleted Items folder has a different ItemId than the appointment item in the calendar folder.</span></span> <span data-ttu-id="e28fe-130">L’élément est copié et supprimé plutôt que simplement déplacé vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="e28fe-130">The item is copied and deleted rather than simply moved to the Deleted Items folder.</span></span> 
  
## <a name="delete-an-appointment-by-using-ews"></a><span data-ttu-id="e28fe-131">Supprimer un rendez-vous à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="e28fe-131">Delete an appointment by using EWS</span></span>
<span data-ttu-id="e28fe-132"><a name="bk_DeleteApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="e28fe-132"></span></span>

<span data-ttu-id="e28fe-133">La demande et la réponse XML dans les exemples suivants correspondent aux appels effectués par le code d’API managées de [Supprimer un rendez-vous à l’aide de l’API managée EWS](#bk_DeleteApptEWSMA).</span><span class="sxs-lookup"><span data-stu-id="e28fe-133">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Delete an appointment by using the EWS Managed API](#bk_DeleteApptEWSMA).</span></span> <span data-ttu-id="e28fe-134">La demande et la réponse XML qui vérifie que l’élément de rendez-vous dans le dossier éléments supprimés est également affiché.</span><span class="sxs-lookup"><span data-stu-id="e28fe-134">The request and response XML that verifies that the appointment item is in the Deleted Items folder is shown as well.</span></span>
  
<span data-ttu-id="e28fe-135">L’exemple suivant montre la requête XML pour l’opération [DeleteItem](../web-service-reference/deleteitem-operation.md) supprimer un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="e28fe-135">The following example shows the request XML for the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation to delete an appointment.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="e28fe-136">L’exemple suivant montre la réponse XML renvoyée par l’opération [DeleteItem](../web-service-reference/deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e28fe-136">The following example shows the response XML that is returned by the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation.</span></span> <span data-ttu-id="e28fe-137">Les attributs **ItemId** et **ChangeKey** sont limitent pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="e28fe-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </m:DeleteItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="e28fe-138">L’exemple suivant montre la requête XML de l’opération [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) qui Récupère le premier élément dans le dossier éléments supprimés afin de comparer le sujet de l’élément avec celle de l’objet rendez-vous supprimé.</span><span class="sxs-lookup"><span data-stu-id="e28fe-138">The following example shows the request XML for the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation that retrieves the first item in the Deleted Items folder in order to compare the item's subject with that of the deleted appointment object.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages
" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="e28fe-139">L’exemple suivant montre la réponse XML renvoyée par l’opération [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pendant l’étape de vérification.</span><span class="sxs-lookup"><span data-stu-id="e28fe-139">The following example shows the response XML that is returned by the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation during the verification step.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e28fe-140">Les attributs **ItemId** et **ChangeKey** sont limitent pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="e28fe-140">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="e28fe-141"><a name="bk_DeleteMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="e28fe-141"></span></span>

## <a name="delete-a-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="e28fe-142">Supprimer une réunion à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="e28fe-142">Delete a meeting by using the EWS Managed API</span></span>

<span data-ttu-id="e28fe-143">Lorsque vous supprimez une réunion, en plus de supprimer l’élément de rendez-vous dans le dossier calendrier, vous pourriez également envoyer des annulations de réunion aux participants.</span><span class="sxs-lookup"><span data-stu-id="e28fe-143">When you delete a meeting, in addition to removing the appointment item from the calendar folder, you might also want to send meeting cancellations to attendees.</span></span> <span data-ttu-id="e28fe-144">Vous pouvez utiliser trois méthodes suivantes pour annuler une réunion :</span><span class="sxs-lookup"><span data-stu-id="e28fe-144">You can use the following three methods to cancel a meeting:</span></span>
  
- [<span data-ttu-id="e28fe-145">Appointment.Delete</span><span class="sxs-lookup"><span data-stu-id="e28fe-145">Appointment.Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="e28fe-146">Appointment.CancelMeeting</span><span class="sxs-lookup"><span data-stu-id="e28fe-146">Appointment.CancelMeeting</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="e28fe-147">CancelMeetingMessage</span><span class="sxs-lookup"><span data-stu-id="e28fe-147">CancelMeetingMessage</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx)
    
<span data-ttu-id="e28fe-148">La méthode que vous choisissez dépend du niveau de détail, que vous devez indiquer dans votre message d’annulation.</span><span class="sxs-lookup"><span data-stu-id="e28fe-148">The method that you choose depends on the level of detail you need to provide in your cancellation message.</span></span> <span data-ttu-id="e28fe-149">[Appointment.CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) facilite la mise à jour le message d’annulation en transmettant un message mis à jour en tant que paramètre.</span><span class="sxs-lookup"><span data-stu-id="e28fe-149">[Appointment.CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) makes it easy to update the cancellation message by passing an updated message as a parameter.</span></span> <span data-ttu-id="e28fe-150">[CancelMeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx) permet de modifier les propriétés de votre message avant d’envoyer une annulation, afin que vous pouvez effectuer des opérations comme demande un accusé de réception.</span><span class="sxs-lookup"><span data-stu-id="e28fe-150">[CancelMeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx) allows you to modify properties on your message before sending a cancellation, so you can do things like request a receipt.</span></span> 
  
<span data-ttu-id="e28fe-151">Les exemples de code de cette section montrent les différentes façons de supprimer une réunion et envoyer des annulations de réunion.</span><span class="sxs-lookup"><span data-stu-id="e28fe-151">The code examples in this section show the different ways to delete a meeting and send meeting cancellations.</span></span> <span data-ttu-id="e28fe-152">Les exemples supposent que vous avez authentifié à un serveur Exchange et avez acquis un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) appelé **service**.</span><span class="sxs-lookup"><span data-stu-id="e28fe-152">The examples assume that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="e28fe-153">La variable locale `meetingId` est un identificateur associé à une réunion existante où l’utilisateur cible est l’organisateur de la réunion.</span><span class="sxs-lookup"><span data-stu-id="e28fe-153">The local variable  `meetingId` is an identifier associated with an existing meeting where the target user is the meeting organizer.</span></span> 
  
<span data-ttu-id="e28fe-154">L’exemple de code suivant montre comment supprimer une réunion à l’aide de la méthode [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e28fe-154">The following code example shows how to delete a meeting by using the [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method.</span></span> 
  
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

<span data-ttu-id="e28fe-155">L’exemple de code suivant montre comment supprimer une réunion à l’aide de la méthode [CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e28fe-155">The following code example shows how to delete a meeting by using the [CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) method.</span></span> 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the CancelMeeting method.
meeting.CancelMeeting("The outdoor meeting has been cancelled due to hailstorms.");

```

<span data-ttu-id="e28fe-156">L’exemple de code suivant montre comment supprimer une réunion à l’aide de la méthode [Appointment.CreateCancelMeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e28fe-156">The following code example shows how to delete a meeting by using the [Appointment.CreateCancelMeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx) method.</span></span> 
  
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

## <a name="delete-a-meeting-by-using-ews"></a><span data-ttu-id="e28fe-157">Supprimer une réunion à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="e28fe-157">Delete a meeting by using EWS</span></span>
<span data-ttu-id="e28fe-158"><a name="bk_EWSDeleteApptAndMeeting"> </a></span><span class="sxs-lookup"><span data-stu-id="e28fe-158"></span></span>

<span data-ttu-id="e28fe-159">La demande et la réponse XML dans les exemples suivants correspondent aux appels effectués par le code d’API managées de [Supprimer une réunion à l’aide de l’API managée EWS](#bk_DeleteMtgEWSMA) à l’aide de la méthode [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e28fe-159">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Delete a meeting by using the EWS Managed API](#bk_DeleteMtgEWSMA) by using the [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="e28fe-160">L’exemple suivant montre la requête XML lorsque vous utilisez l’opération [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour envoyer des messages d’annulation aux participants et supprimer une réunion.</span><span class="sxs-lookup"><span data-stu-id="e28fe-160">The following example shows the request XML when you use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to send cancellation messages to attendees and delete a meeting.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="e28fe-161">L’exemple suivant montre le code XML qui est retourné en réponse à une demande d’opération [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) permet de supprimer une réunion.</span><span class="sxs-lookup"><span data-stu-id="e28fe-161">The following example shows the XML that is returned in response to a [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation request used to delete a meeting.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e28fe-162">Les attributs **ItemId** et **ChangeKey** sont limitent pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="e28fe-162">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="e28fe-163">L’exemple suivant montre la requête XML de l’opération [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) qui Récupère le premier élément dans le dossier éléments supprimés afin de comparer le sujet de l’élément avec celle de l’objet rendez-vous supprimé.</span><span class="sxs-lookup"><span data-stu-id="e28fe-163">The following example shows the request XML for the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation that retrieves the first item in the Deleted Items folder in order to compare the item's subject with that of the deleted appointment object.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="e28fe-164">L’exemple suivant montre le code XML renvoyé par l’opération [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pendant l’étape de vérification.</span><span class="sxs-lookup"><span data-stu-id="e28fe-164">The following example shows the XML that is returned by the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation during the verification step.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e28fe-165">Les attributs **Id** et **ChangeKey** sont limitent pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="e28fe-165">The **Id** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="see-also"></a><span data-ttu-id="e28fe-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e28fe-166">See also</span></span>

- [<span data-ttu-id="e28fe-167">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e28fe-167">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)    
- [<span data-ttu-id="e28fe-168">Créer des rendez-vous et réunions à l’aide de EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e28fe-168">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)  
- [<span data-ttu-id="e28fe-169">Obtenir des rendez-vous et réunions à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e28fe-169">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="e28fe-170">Mettre à jour vos rendez-vous et réunions à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e28fe-170">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="e28fe-171">Proposer une nouvelle heure de réunion à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e28fe-171">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="e28fe-172">Proposer une nouvelle heure de réunion à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e28fe-172">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    

