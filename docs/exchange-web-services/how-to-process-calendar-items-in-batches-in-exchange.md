---
title: Traitement par lots des éléments de calendrier dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fb2952e2-cbfe-43ac-b746-f071faa7665c
description: Découvrez comment créer, obtenir, mettre à jour ou supprimer des lots des éléments de calendrier dans un seul appel à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 2c92b492d9b51d0a5ac3140af22e5527e7bf19be
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754943"
---
# <a name="process-calendar-items-in-batches-in-exchange"></a><span data-ttu-id="f57a4-103">Traitement par lots des éléments de calendrier dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f57a4-103">Process calendar items in batches in Exchange</span></span>

<span data-ttu-id="f57a4-104">Découvrez comment créer, obtenir, mettre à jour ou supprimer des lots des éléments de calendrier dans un seul appel à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="f57a4-104">Learn how to create, get, update, or delete batches of calendar items in a single call by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="f57a4-105">Vous pouvez utiliser l’API managée EWS ou EWS pour travailler avec des lots de rendez-vous et réunions afin de réduire le nombre d’appels un client permet à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="f57a4-105">You can use the EWS Managed API or EWS to work with batches of appointments and meetings to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="f57a4-106">Lorsque vous utilisez l’API managée EWS pour créer, obtenir, mettre à jour et supprimez un lot d’éléments de calendrier, vous utilisez les méthodes de l’objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , tandis que lorsque vous travaillez avec des éléments de calendrier, vous utilisez les méthodes de l’objet [rendez-vous](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f57a4-106">When you use the EWS Managed API to create, get, update, and delete a batch of calendar items, you use [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single calendar items, you use [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="f57a4-107">Si vous utilisez EWS, vous utilisez la même opération pour les appels de commandes que vous utilisez pour les appels uniques.</span><span class="sxs-lookup"><span data-stu-id="f57a4-107">If you are using EWS, you use the same operation for batch calls that you use for single calls.</span></span> 
  
<span data-ttu-id="f57a4-108">**Le tableau 1. Méthodes d’API managées et opérations EWS pour travailler avec des éléments de calendrier des lots**</span><span class="sxs-lookup"><span data-stu-id="f57a4-108">**Table 1. EWS Managed API methods and EWS operations for working with batches of calendar items**</span></span>

|<span data-ttu-id="f57a4-109">**Pour...**</span><span class="sxs-lookup"><span data-stu-id="f57a4-109">**In order to…**</span></span>|<span data-ttu-id="f57a4-110">**Utilisez cette méthode de l’API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="f57a4-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="f57a4-111">**Utilisez cette opération EWS**</span><span class="sxs-lookup"><span data-stu-id="f57a4-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f57a4-112">Créer des éléments de calendrier par lots</span><span class="sxs-lookup"><span data-stu-id="f57a4-112">Create calendar items in batches</span></span>  <br/> |[<span data-ttu-id="f57a4-113">CreateItems</span><span class="sxs-lookup"><span data-stu-id="f57a4-113">CreateItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f57a4-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="f57a4-114">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="f57a4-115">Obtenir des éléments de calendrier par lots</span><span class="sxs-lookup"><span data-stu-id="f57a4-115">Get calendar items in batches</span></span>  <br/> |[<span data-ttu-id="f57a4-116">BindToItems</span><span class="sxs-lookup"><span data-stu-id="f57a4-116">BindToItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f57a4-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="f57a4-117">GetItem</span></span>](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="f57a4-118">Éléments de calendrier de mise à jour par lots</span><span class="sxs-lookup"><span data-stu-id="f57a4-118">Update calendar items in batches</span></span>  <br/> |[<span data-ttu-id="f57a4-119">UpdateItems</span><span class="sxs-lookup"><span data-stu-id="f57a4-119">UpdateItems</span></span>](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f57a4-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="f57a4-120">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="f57a4-121">Supprimer des éléments de calendrier par lots</span><span class="sxs-lookup"><span data-stu-id="f57a4-121">Delete calendar items in batches</span></span>  <br/> |[<span data-ttu-id="f57a4-122">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="f57a4-122">DeleteItems</span></span>](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="f57a4-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="f57a4-123">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="f57a4-124">Dans cet article, vous allez apprendre à effectuer des tâches de lots des éléments de calendrier de base à l’aide de l’API managée EWS ou EWS.</span><span class="sxs-lookup"><span data-stu-id="f57a4-124">In this article, you'll learn how to complete basic tasks for batches of calendar items by using the EWS Managed API or EWS.</span></span>
  
<span data-ttu-id="f57a4-125">Notez que dans les exemples d’API managées dans cet article, si les méthodes sont appelées de manière séquentielle, vous pouvez créer, obtenir, mettre à jour et puis supprimez un lot d’éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="f57a4-125">Note that in the EWS Managed API examples in this article, if the methods are called sequentially, you can create, get, update, and then delete a batch of calendar items.</span></span>
  
```cs
Collection<ItemId> itemIds = BatchCreateCalendarItems(service);
Collection<Appointment> myAppointments = BatchGetCalendarItems(service, itemIds);
itemIds = BatchUpdateCalendarItems(service, myAppointments);
BatchDeleteCalendarItemsTwice(service, itemIds);

```

## <a name="create-calendar-items-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="f57a4-126">Créer des éléments de calendrier par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="f57a4-126">Create calendar items in batches by using the EWS Managed API</span></span>
<span data-ttu-id="f57a4-127"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f57a4-127"></span></span>

<span data-ttu-id="f57a4-128">Vous pouvez créer des éléments de calendrier par lots à l’aide de la méthode API managées [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f57a4-128">You can create calendar items in batches by using the [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="f57a4-129">Cet exemple crée trois objets de [rendez-vous](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) , une réunion, un rendez-vous périodique et un rendez-vous —, puis les ajouter à une collection.</span><span class="sxs-lookup"><span data-stu-id="f57a4-129">This example creates three [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) objects — a single-instance appointment, a recurring appointment, and a meeting — and then adds them to a collection.</span></span> 
  
<span data-ttu-id="f57a4-130">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="f57a4-130">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
public static Collection<ItemId> BatchCreateCalendarItems(ExchangeService service)
{
    // These are unsaved local instances of an Appointment object.
    // Despite the required parameter of an ExchangeService object (service), no call
    // to an Exchange server is made when the objects are instantiated.
    // A call to the Exchange server is made when the service.CreateItems() method is called.
    Appointment appt1 = new Appointment(service);
    Appointment recurrAppt2 = new Appointment(service);
    Appointment meeting3 = new Appointment(service);
    // Set the properties for a single instance appointment.
    appt1.Subject = "Review current quarterly deliverables";
    appt1.Body = "Wrap up all outstanding deliverables for this quarter and prepare for Q2.";
    appt1.Start = DateTime.Now.AddDays(2);
    appt1.End = appt1.Start.AddHours(3);
    appt1.Location = "My office";
    appt1.ReminderMinutesBeforeStart = 30;
    // Set the properties for a recurring appointment.
    recurrAppt2.Subject = "Food bank delivery";
    recurrAppt2.Body = "Deliver the team's weekly food drive collection to the food bank.";
    recurrAppt2.Start = DateTime.Now.AddDays(1);
    recurrAppt2.End = recurrAppt2.Start.AddHours(1);
    recurrAppt2.Location = "Local food bank";
    arecurrAppt2.ReminderMinutesBeforeStart = 30;
    DayOfTheWeek[] dow = new DayOfTheWeek[] {(DayOfTheWeek)recurrAppt2.Start.DayOfWeek};
    recurrAppt2.Recurrence = new Recurrence.WeeklyPattern(recurrAppt2.Start.Date, 1, dow);
    recurrAppt2.Recurrence.StartDate = recurrAppt2.Start.Date;
    recurrAppt2.Recurrence.NumberOfOccurrences = 10;
    // Set the properties for a single instance meeting.
    meeting3.Subject = "Code Blast";
    meeting3.Body = "Let's get together to finish all the methods and unit tests for the ContosoLive project.";
    meeting3.Start = DateTime.Now.AddDays(3);
    meeting3.End = meeting3.Start.AddHours(6);
    meeting3.Location = "The lounge";
    meeting3.RequiredAttendees.Add("Mack@contoso.com");
    meeting3.RequiredAttendees.Add("Sadie@contoso.com");
    meeting3.RequiredAttendees.Add("Magdalena@contoso.com");
    meeting3.ReminderMinutesBeforeStart = 30;
    // Add the appointment objects to a collection.
    Collection<Appointment> calendarItems = new Collection<Appointment>() { appt1, recurrAppt2, meeting3 };
    // Instantiate a collection of item IDs to populate from the values that are returned by the Exchange server.
    Collection<ItemId> itemIds = new Collection<ItemId>();
            
    // Send the batch of Appointment objects.
    // Note that multiple calls to the Exchange server might be made when Appointment objects have attachments.
    // Note also that the the ID of the item collection passed as the first parameter to CreateItems is set on return.
    ServiceResponseCollection<ServiceResponse> response = service.CreateItems(calendarItems,
                                                                              WellKnownFolderName.Calendar,
                                                                              MessageDisposition.SendAndSaveCopy,
                                                                              SendInvitationsMode.SendToAllAndSaveCopy);
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All appointments and meetings sucessfully created.");
    }
    // Collect the item IDs from the created calendar items.
    foreach (Appointment appt in calendarItems)
    {
        itemIds.Add(appt.Id);
    }
    int counter = 1;
    // Show the IDs and errors for each message.
    foreach (ServiceResponse resp in response)
    {
        // Because item IDs are long, show only five characters.
        Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(0, 5), resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        counter++;
    }
// Return the collection of item IDs.
return itemIds;
}

```

<span data-ttu-id="f57a4-131">Les objets de [rendez-vous](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) dans la collection peuvent être rendez-vous ou réunions et instances uniques ou une série périodique des deux.</span><span class="sxs-lookup"><span data-stu-id="f57a4-131">The [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) objects in the collection can be appointments or meetings, and either single instances or a recurring series of either.</span></span> 
  
## <a name="create-calendar-items-in-batches-by-using-ews"></a><span data-ttu-id="f57a4-132">Créer des éléments de calendrier par lots à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="f57a4-132">Create calendar items in batches by using EWS</span></span>
<span data-ttu-id="f57a4-133"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="f57a4-133"></span></span>

<span data-ttu-id="f57a4-134">Vous pouvez créer des éléments de calendrier par lots à l’aide de l’opération EWS [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="f57a4-134">You can create calendar items in batches by using the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="f57a4-135">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [créer des éléments de calendrier par lots](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="f57a4-135">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create calendar items in batches](#bk_createewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"  
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy" SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Review current quarterly deliverables</t:Subject>
          <t:Body BodyType="HTML">Wrap up all outstanding deliverables for this quarter and prepare for Q2.</t:Body>
          <t:ReminderDueBy>2014-01-07T12:13:40.333-08:00</t:ReminderDueBy>
          <t:Start>2014-01-08T13:13:37.717-08:00</t:Start>
          <t:End>2014-01-08T16:13:37.717-08:00</t:End>
          <t:Location>Local food bank</t:Location>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
        <t:CalendarItem>
          <t:Subject>Food bank delivery</t:Subject>
          <t:Body BodyType="HTML">Deliver the team's weekly food drive collection to the food bank.</t:Body>
          <t:Start>2014-01-07T13:13:40.333-08:00</t:Start>
          <t:End>2014-01-07T14:13:40.333-08:00</t:End>
          <t:Recurrence>
            <t:WeeklyRecurrence>
              <t:Interval>1</t:Interval>
              <t:DaysOfWeek>Tuesday</t:DaysOfWeek>
            </t:WeeklyRecurrence>
            <t:NumberedRecurrence>
              <t:StartDate>2014-01-07-08:00</t:StartDate>
              <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
            </t:NumberedRecurrence>
          </t:Recurrence>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
        <t:CalendarItem>
          <t:Subject>Code Blast</t:Subject>
          <t:Body BodyType="HTML">Let's get together to finish all the methods and unit tests for the ContosoLive project.</t:Body>
          <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
          <t:Start>2014-01-09T13:13:44.998-08:00</t:Start>
          <t:End>2014-01-09T19:13:44.998-08:00</t:End>
          <t:Location>The lounge</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="f57a4-136">Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** pour chacun des nouveaux éléments de calendrier, ce qui indique que chaque élément de calendrier a été créée. avec succès.</span><span class="sxs-lookup"><span data-stu-id="f57a4-136">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new calendar items, which indicates that each calendar item was created successfully.</span></span> 
  
<span data-ttu-id="f57a4-137">Notez que les éléments de calendrier sont des réunions ou rendez-vous, ou instances uniques ou une série périodique, selon les valeurs des éléments de chaque élément de calendrier transmis sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="f57a4-137">Note that the calendar items are either meetings or appointments, or single instances or a recurring series, according to the element values of each calendar item passed to the Exchange server.</span></span>
  
<span data-ttu-id="f57a4-138">Voici la réponse du serveur.</span><span class="sxs-lookup"><span data-stu-id="f57a4-138">The following is the response from the server.</span></span> <span data-ttu-id="f57a4-139">Les attributs **ItemId** et **ChangeKey** sont limitent pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="f57a4-139">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="847" MinorBuildNumber="12" Version="V2_8" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
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

## <a name="get-calendar-items-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="f57a4-140">Obtenir des éléments de calendrier par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="f57a4-140">Get calendar items in batches by using the EWS Managed API</span></span>
<span data-ttu-id="f57a4-141"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f57a4-141"></span></span>

<span data-ttu-id="f57a4-142">Vous pouvez obtenir des éléments de calendrier par lots à l’aide de la méthode API managées [BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f57a4-142">You can get calendar items in batches by using the [BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> 
  
<span data-ttu-id="f57a4-143">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="f57a4-143">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
public static Collection<Appointment> BatchGetCalendarItems(ExchangeService service, Collection<ItemId> itemIds)
{
    // As a best practice, create a property set that limits the properties returned by the Bind method to only those that are required.
    PropertySet appointmentProps = new PropertySet(BasePropertySet.IdOnly,
                                                   AppointmentSchema.Subject,
                                                   AppointmentSchema.Body,
                                                   AppointmentSchema.ReminderMinutesBeforeStart,
                                                   AppointmentSchema.Start,
                                                   AppointmentSchema.End,
                                                   AppointmentSchema.AppointmentType,
                                                   AppointmentSchema.Location,
                                                   AppointmentSchema.RequiredAttendees);
            
    ServiceResponseCollection<GetItemResponse> response = service.BindToItems(itemIds, appointmentProps);
    Collection<Appointment> calendarItems = new Collection<Appointment>();
    foreach (GetItemResponse items in response)
    {
        Item item = items.Item;
        Appointment appointmentItem = (Appointment)item;
        calendarItems.Add(appointmentItem);
        Console.WriteLine("Found item {0}.", appointmentItem.Id.ToString().Substring(144));
    }
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All calendar items retrieved successfully.");
        Console.WriteLine("\r\n");
    }
    else
    {
        int counter = 1;
        // List the status of each message.
        foreach (ServiceResponse resp in response)
        {
            // Because item IDs are long, show only last 8 characters.
            Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(144), resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            Console.WriteLine("\r\n");
            counter++;
        }
    }
    return calendarItems;
}

```

## <a name="get-calendar-items-in-batches-by-using-ews"></a><span data-ttu-id="f57a4-144">Obtenir des éléments de calendrier par lots à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="f57a4-144">Get calendar items in batches by using EWS</span></span>
<span data-ttu-id="f57a4-145"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="f57a4-145"></span></span>

<span data-ttu-id="f57a4-146">Vous pouvez obtenir des éléments de calendrier par lots à l’aide de l’opération EWS [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f57a4-146">You can get calendar items in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in the following example.</span></span> <span data-ttu-id="f57a4-147">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [obtenir des éléments de calendrier par lots](#bk_getewsma).</span><span class="sxs-lookup"><span data-stu-id="f57a4-147">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get calendar items in batches](#bk_getewsma).</span></span>
  
<span data-ttu-id="f57a4-148">Les attributs **ItemId** et **ChangeKey** sont limitent pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="f57a4-148">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:Body" />
          <t:FieldURI FieldURI="item:ReminderMinutesBeforeStart" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:RequiredAttendees" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="f57a4-149">Le serveur répond à la demande de **GetItem** avec un message [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) avec les propriétés requises pour chaque élément, comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f57a4-149">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message with the requested properties for each item, as shown in the following example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="847" MinorBuildNumber="16" Version="V2_8" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Review current quarterly deliverables</t:Subject>
              <t:Body BodyType="HTML">
                &amp;lt;html&amp;gt;
                &amp;lt;head&amp;gt;
                &amp;lt;meta http-equiv="Content-Type" content="text/html; charset=utf-8"&amp;gt;
                &amp;lt;/head&amp;gt;
                &amp;lt;body&amp;gt;
                Wrap up all outstanding deliverables for this quarter and prepare for Q2.
                &amp;lt;/body&amp;gt;
                &amp;lt;/html&amp;gt;
              </t:Body>
              <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
              <t:Start>2014-01-19T18:59:07Z</t:Start>
              <t:End>2014-01-19T21:59:07Z</t:End>
              <t:Location>Local food bank</t:Location>
              <t:CalendarItemType>Single</t:CalendarItemType>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Food bank delivery</t:Subject>
              <t:Body BodyType="HTML">
                &amp;lt;html&amp;gt;
                &amp;lt;head&amp;gt;
                &amp;lt;meta http-equiv="Content-Type" content="text/html; charset=utf-8"&amp;gt;
                &amp;lt;/head&amp;gt;
                &amp;lt;body&amp;gt;
                Deliver the team's weekly food drive collection to the food bank.
                &amp;lt;/body&amp;gt;
                &amp;lt;/html&amp;gt;
              </t:Body>
              <t:ReminderMinutesBeforeStart>15</t:ReminderMinutesBeforeStart>
              <t:Start>2014-01-18T18:59:07Z</t:Start>
              <t:End>2014-01-18T19:59:07Z</t:End>
              <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Code Blast</t:Subject>
              <t:Body BodyType="HTML">
                &amp;lt;html&amp;gt;
                &amp;lt;head&amp;gt;
                &amp;lt;meta http-equiv="Content-Type" content="text/html; charset=utf-8"&amp;gt;
                &amp;lt;/head&amp;gt;
                &amp;lt;body&amp;gt;
                Let's get together to finish all the methods and unit tests for the ContosoLive project.
                &amp;lt;/body&amp;gt;
                &amp;lt;/html&amp;gt;
              </t:Body>
              <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
              <t:Start>2014-01-20T18:59:08Z</t:Start>
              <t:End>2014-01-21T00:59:08Z</t:End>
              <t:Location>The lounge</t:Location>
              <t:CalendarItemType>Single</t:CalendarItemType>
              <t:RequiredAttendees>
                <t:Attendee>
                  <t:Mailbox>
                    <t:Name>Mack@contoso.com</t:Name>
                    <t:EmailAddress>Mack@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                  <t:ResponseType>Unknown</t:ResponseType>
                </t:Attendee>
                <t:Attendee>
                  <t:Mailbox>
                    <t:Name>Sadie@contoso.com</t:Name>
                    <t:EmailAddress>Sadie@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                  <t:ResponseType>Unknown</t:ResponseType>
                </t:Attendee>
                <t:Attendee>
                  <t:Mailbox>
                    <t:Name>Magdalena@contoso.com</t:Name>
                    <t:EmailAddress>Magdalena@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                  <t:ResponseType>Unknown</t:ResponseType>
                </t:Attendee>
              </t:RequiredAttendees>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-calendar-items-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="f57a4-150">Éléments de calendrier de mise à jour par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="f57a4-150">Update calendar items in batches by using the EWS Managed API</span></span>
<span data-ttu-id="f57a4-151"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f57a4-151"></span></span>

<span data-ttu-id="f57a4-152">Vous pouvez mettre à jour propriétés des éléments de calendrier par lots à l’aide de la méthode API managées [UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f57a4-152">You can update calendar item properties in batches by using the [UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> 
  
<span data-ttu-id="f57a4-153">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="f57a4-153">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
public static Collection<ItemId> BatchUpdateCalendarItems(ExchangeService service, Collection<Appointment> calenderItems)
{
    int i = 1;
    // Appointment item IDs to return.
    Collection<ItemId> itemIds = new Collection<ItemId>();
            
    // Update the subject of each calendar item locally.
    foreach (Appointment appointment in calenderItems)
    {
        // Update the subject of each calendar item in the collection
        appointment.Subject = "Company headquarters are moving down the street to 1234 Contoso Drive!: " + appointment.Subject.ToString();
        Console.WriteLine("Updated the subject property for calendar item {0} of {1}, item id {2}.", i, calenderItems.Count, appointment.Id.ToString().Substring(0, 5));
        i++;
        // Collect item IDs to return instead of appointment objects.
        itemIds.Add(appointment.Id);
    }
    // Send the updated items to the server.
    // This method call results in an UpdateItem call to EWS.
    ServiceResponseCollection<UpdateItemResponse> response = service.UpdateItems(calenderItems, 
                                                                                 WellKnownFolderName.Calendar, 
                                                                                 ConflictResolutionMode.AutoResolve, 
                                                                                 MessageDisposition.SendAndSaveCopy,
                                                                                    SendInvitationsOrCancellationsMode.SendToChangedAndSaveCopy);
    // Display the result of the UpdateItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("Calendar items successfully updated.\r\n");
    }
    else
    {
        Console.WriteLine("Not all items were successfully updated on the server.\r\n");
        i = 1;
        foreach (ServiceResponse srvResponse in response)
        {
            Console.WriteLine("Result for message {0}: {1}", i, srvResponse.Result);
            Console.WriteLine("Error code: {0}", srvResponse.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", srvResponse.ErrorMessage);
            i++;
        }
    }
    return itemIds;
}  

```

## <a name="update-calendar-items-in-batches-by-using-ews"></a><span data-ttu-id="f57a4-154">Éléments de calendrier de mise à jour par lots à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="f57a4-154">Update calendar items in batches by using EWS</span></span>
<span data-ttu-id="f57a4-155"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="f57a4-155"></span></span>

<span data-ttu-id="f57a4-156">Vous pouvez mettre à jour plusieurs éléments de calendrier à l’aide de l’opération EWS [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) , comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="f57a4-156">You can update multiple calendar items by using the [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS operation, as shown in following code example.</span></span> <span data-ttu-id="f57a4-157">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [mettre à jour des éléments de calendrier par lots](#bk_updateewsma).</span><span class="sxs-lookup"><span data-stu-id="f57a4-157">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update calendar items in batches](#bk_updateewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SendAndSaveCopy" ConflictResolution="AutoResolve" 
                  SendMeetingInvitationsOrCancellations="SendToChangedAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar" />
      </m:SavedItemFolderId>
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Company headquarters are moving down the street to 1234 Contoso Drive!: Review current quarterly deliverables
                </t:Subject>
                </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Company headquarters are moving down the street to 1234 Contoso Drive!: Food bank delivery</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Company headquarters are moving down the street to 1234 Contoso Drive!: Code Blast</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="f57a4-158">Le serveur répond à la demande **UpdateItem** avec un message [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, ce qui indique que les mises à jour a été correctement enregistré sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="f57a4-158">The server responds to the **UpdateItem** request with an [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server.</span></span> <span data-ttu-id="f57a4-159">Les conflits sont déclarées dans l’élément [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f57a4-159">Any conflicts are reported in the [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="859" MinorBuildNumber="13" 
                         Version="V2_8" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>1</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>1</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>1</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </m:UpdateItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="delete-calendar-items-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="f57a4-160">Supprimer des éléments de calendrier par lots à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="f57a4-160">Delete calendar items in batches by using the EWS Managed API</span></span>
<span data-ttu-id="f57a4-161"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="f57a4-161"></span></span>

<span data-ttu-id="f57a4-162">Vous pouvez supprimer des éléments de calendrier par lots à l’aide de la méthode API managées [DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="f57a4-162">You can delete calendar items in batches by using the [DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="f57a4-163">Cet exemple montre comment la suppression demander une deuxième fois pour que le serveur renvoie une erreur **ErrorItemNotFound** pour indiquer que les éléments à supprimer n’étaient pas dans le magasin lors de l’appel a été effectué qu’aucune exception n’est levée.</span><span class="sxs-lookup"><span data-stu-id="f57a4-163">This example makes the deletion request a second time to show that no exceptions are thrown but that the server will return an **ErrorItemNotFound** error to indicate that the items to delete weren't in the store when the call was made.</span></span> <span data-ttu-id="f57a4-164">Cette erreur est renvoyée si l’élément a déjà été supprimé ou si un ID d’élément incorrect est transmis au serveur.</span><span class="sxs-lookup"><span data-stu-id="f57a4-164">This error is returned if the item has already been deleted, or if a bad item ID is passed to the server.</span></span> 
  
<span data-ttu-id="f57a4-165">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="f57a4-165">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
public static void BatchDeleteCalendarItemsTwice(ExchangeService service, Collection<ItemId> itemIds)
{
    // Delete the batch of appointment objects
    // This method call results in a DeleteItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.DeleteItems(itemIds, 
                                                                                DeleteMode.MoveToDeletedItems, 
                                                                                SendCancellationsMode.SendToAllAndSaveCopy, 
                                                                                AffectedTaskOccurrence.AllOccurrences);
    int counter = 1;
    // Show the IDs and errors for each message.
    foreach (ServiceResponse resp in response)
    {
        // Because item IDs are long, show only five characters.
        Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(0, 5), resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        counter++;
    }
            
    // Now attempt to delete the same items again.
    response = service.DeleteItems(itemIds,
                                    DeleteMode.MoveToDeletedItems,
                                    SendCancellationsMode.SendToAllAndSaveCopy,
                                    AffectedTaskOccurrence.AllOccurrences);
    counter = 1;
    // Show the IDs and errors for each message.
    foreach (ServiceResponse resp in response)
    {
        // Because item IDs are long, show only five characters.
        Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(0, 5), resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        counter++;
    }
}

```

<span data-ttu-id="f57a4-166">Lors du deuxième appel de la méthode **DeleteItems** , aucune exception n’est levée, mais le serveur renvoie une erreur **ErrorItemNotFound** dans le résultat.</span><span class="sxs-lookup"><span data-stu-id="f57a4-166">When the **DeleteItems** method is called the second time, no exception is thrown, but the server returns an **ErrorItemNotFound** error in the result.</span></span> 
  
## <a name="delete-calendar-items-in-batches-by-using-ews"></a><span data-ttu-id="f57a4-167">Supprimer des éléments de calendrier par lots à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="f57a4-167">Delete calendar items in batches by using EWS</span></span>
<span data-ttu-id="f57a4-168"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="f57a4-168"></span></span>

<span data-ttu-id="f57a4-169">Vous pouvez supprimer des éléments de calendrier par lots à l’aide de l’opération EWS [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) , comme illustré dans l’exemple de code suivant.</span><span class="sxs-lookup"><span data-stu-id="f57a4-169">You can delete calendar items in batches by using the [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="f57a4-170">C’est également la demande XML qui envoie de l’API managée EWS lorsque vous utilisez l’API managée EWS pour [Supprimer des éléments de calendrier par lots](#bk_deleteewsma).</span><span class="sxs-lookup"><span data-stu-id="f57a4-170">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete calendar items in batches](#bk_deleteewsma).</span></span> 
  
<span data-ttu-id="f57a4-171">Les attributs **ItemId** et **ChangeKey** sont limitent pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="f57a4-171">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems" 
                  AffectedTaskOccurrences="AllOccurrences" 
                  SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="f57a4-172">Le serveur répond à la demande **DeleteItem** avec un message [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** pour chaque élément qui a été supprimé.</span><span class="sxs-lookup"><span data-stu-id="f57a4-172">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="859" MinorBuildNumber="13" Version="V2_8" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </m:DeleteItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="f57a4-173">Notez que si la demande **DeleteItem** est effectuée lorsque les éléments associés ont déjà été supprimés, aucune exception n’est levée, mais le serveur renvoie une erreur **ErrorItemNotFound** dans le résultat.</span><span class="sxs-lookup"><span data-stu-id="f57a4-173">Note that if the **DeleteItem** request is made when the associated items have already been deleted, no exception will be thrown, but the server will return an **ErrorItemNotFound** error in the result.</span></span> <span data-ttu-id="f57a4-174">L’exemple suivant montre la réponse du serveur à une demande **DeleteItem** lorsque les éléments associés ont déjà été supprimés.</span><span class="sxs-lookup"><span data-stu-id="f57a4-174">The following example shows the server response to a **DeleteItem** request when the associated items have already been deleted.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="859" MinorBuildNumber="13" Version="V2_8" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </m:DeleteItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="f57a4-175">Vérification réussie un traitement par lots</span><span class="sxs-lookup"><span data-stu-id="f57a4-175">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="f57a4-176"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="f57a4-176"></span></span>

<span data-ttu-id="f57a4-177">Lorsqu’un ou plusieurs éléments de calendrier dans une requête par lot ne peut pas être traités, une erreur est renvoyée pour chaque élément de calendrier qui a échoué, et le reste des éléments du calendrier dans le lot sont traitées comme prévu.</span><span class="sxs-lookup"><span data-stu-id="f57a4-177">When one or more calendar items in a batched request can't be processed as requested, an error is returned for each calendar item that failed, and the rest of the calendar items in the batch are processed as expected.</span></span> <span data-ttu-id="f57a4-178">Échecs dans le traitement par lots peuvent se produire si l’élément a été supprimé et par conséquent ne peut pas être envoyé, récupéré ou mis à jour, ou si l’élément déplacé vers un autre dossier et par conséquent ne possède un nouvel ID d’élément et ne peut pas être modifié avec l’ID d’élément envoyé.</span><span class="sxs-lookup"><span data-stu-id="f57a4-178">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent.</span></span> <span data-ttu-id="f57a4-179">Les informations contenues dans cette section montre comment obtenir des détails sur les échecs de l’erreur dans le traitement par lots des éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="f57a4-179">The information in this section shows how to get error details about failures in batch processing of calendar items.</span></span>
  
<span data-ttu-id="f57a4-180">Pour vérifier la réussite d’un processus de traitement par lots à l’aide de l’API managée EWS, vous pouvez vérifier que la propriété [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) de la [ServiceResponseCollection](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx) est égale à [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="f57a4-180">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="f57a4-181">Dans ce cas, tous les éléments de calendrier ont été correctement traités.</span><span class="sxs-lookup"><span data-stu-id="f57a4-181">If so, all the calendar items were processed successfully.</span></span> <span data-ttu-id="f57a4-182">Si **OverallResult** n’est pas égale à **ServiceResult.Success**, un ou plusieurs des éléments du calendrier qui n’ont pas été traités avec succès.</span><span class="sxs-lookup"><span data-stu-id="f57a4-182">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the calendar items were not processed successfully.</span></span> <span data-ttu-id="f57a4-183">Chacun des objets retournés dans le **ServiceResponseCollection** contient les propriétés suivantes :</span><span class="sxs-lookup"><span data-stu-id="f57a4-183">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span> 
  
- [<span data-ttu-id="f57a4-184">Code d’erreur</span><span class="sxs-lookup"><span data-stu-id="f57a4-184">ErrorCode</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="f57a4-185">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="f57a4-185">ErrorDetails</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="f57a4-186">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="f57a4-186">ErrorMessage</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="f57a4-187">ErrorProperties</span><span class="sxs-lookup"><span data-stu-id="f57a4-187">ErrorProperties</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="f57a4-188">Résultat</span><span class="sxs-lookup"><span data-stu-id="f57a4-188">Result</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
<span data-ttu-id="f57a4-189">Ces propriétés contiennent des informations sur la raison pour laquelle les éléments de calendrier pas peuvent être traitées comme demandé.</span><span class="sxs-lookup"><span data-stu-id="f57a4-189">These properties contain information about why the calendar items could not be processed as requested.</span></span> <span data-ttu-id="f57a4-190">Les exemples de cet article impriment les **résultats**, **code d’erreur**et **ErrorMessage** pour chaque élément ayant échoué.</span><span class="sxs-lookup"><span data-stu-id="f57a4-190">The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed item.</span></span> <span data-ttu-id="f57a4-191">Vous pouvez utiliser ces résultats pour rechercher le problème.</span><span class="sxs-lookup"><span data-stu-id="f57a4-191">You can use these results to investigate the issue.</span></span> 
  
<span data-ttu-id="f57a4-192">Pour EWS, pour vérifier la réussite d’un processus par lot, consultez l’attribut [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) pour chaque élément en cours de traitement.</span><span class="sxs-lookup"><span data-stu-id="f57a4-192">For EWS, to verify the success of a batched process, check the [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed.</span></span> <span data-ttu-id="f57a4-193">Voici la structure de base de la **ResponseMessageType**, le type de base à partir de la réponse de tous les messages sont dérivés.</span><span class="sxs-lookup"><span data-stu-id="f57a4-193">The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span> 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="f57a4-194">L’attribut **ResponseClass** est défini sur **succès** si l’élément de calendrier a réussi, ou **erreur** si elle n’a pas été traité avec succès.</span><span class="sxs-lookup"><span data-stu-id="f57a4-194">The **ResponseClass** attribute is set to **Success** if the calendar item was processed successfully, or **Error** if it was not processed successfully.</span></span> <span data-ttu-id="f57a4-195">Éléments de calendrier, vous ne rencontrerez pas un **Avertissement** au cours de traitement par lots.</span><span class="sxs-lookup"><span data-stu-id="f57a4-195">For calendar items, you will not encounter a **Warning** during batch processing.</span></span> <span data-ttu-id="f57a4-196">Si la **ResponseClass** est **opération réussie**, l’élément [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) qui suit est également définie sur **NoError**.</span><span class="sxs-lookup"><span data-stu-id="f57a4-196">If the **ResponseClass** is **Success**, the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**.</span></span> <span data-ttu-id="f57a4-197">Si la **ResponseClass** est **erreur**, vous devez vérifier les valeurs des éléments [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx) **ResponseCode**et [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) pour déterminer la cause du problème.</span><span class="sxs-lookup"><span data-stu-id="f57a4-197">If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem.</span></span> <span data-ttu-id="f57a4-198">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) n’est actuellement pas utilisé.</span><span class="sxs-lookup"><span data-stu-id="f57a4-198">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f57a4-199">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f57a4-199">See also</span></span>


- [<span data-ttu-id="f57a4-200">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f57a4-200">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="f57a4-201">Obtenir des rendez-vous et réunions à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f57a4-201">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="f57a4-202">Mettre à jour vos rendez-vous et réunions à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f57a4-202">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="f57a4-203">Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f57a4-203">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="f57a4-204">Traitement par lots des éléments de calendrier dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f57a4-204">Process calendar items in batches in Exchange</span></span>](how-to-process-calendar-items-in-batches-in-exchange.md)
    
- [<span data-ttu-id="f57a4-205">Limitation des implications en matière de requêtes de lots EWS</span><span class="sxs-lookup"><span data-stu-id="f57a4-205">Throttling implications for EWS batch requests</span></span>](ews-throttling-in-exchange.md#bk_ThrottlingBatch)
    

