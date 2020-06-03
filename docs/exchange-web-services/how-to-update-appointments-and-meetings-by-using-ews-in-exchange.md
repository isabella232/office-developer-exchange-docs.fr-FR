---
title: Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 12/9/2015
ms.audience: Developer
ms.assetid: 13256625-083e-4a17-8fd1-2bed1f7cc14e
description: Découvrez comment mettre à jour des rendez-vous et des réunions à l’aide de l’API managée EWS ou EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 553f52e3d9c7119ee249e0e162d057e4acc993ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527606"
---
# <a name="update-appointments-and-meetings-by-using-ews-in-exchange"></a><span data-ttu-id="2be6e-103">Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2be6e-103">Update appointments and meetings by using EWS in Exchange</span></span>

<span data-ttu-id="2be6e-104">Découvrez comment mettre à jour des rendez-vous et des réunions à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="2be6e-104">Learn how to update appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="2be6e-p101">La principale différence entre les réunions et les rendez-vous réside dans la présence de participants aux réunions, mais pas aux rendez-vous. Les rendez-vous et les réunions peuvent être des instances uniques ou faire partie d'une série périodique. Cependant, les rendez-vous n'incluant ni participants, ni salles, ni ressources, ne nécessitent pas l'envoi d'un message. En interne, Exchange utilise le même objet pour les réunions et pour les rendez-vous. Pour utiliser les réunions et les rendez-vous, vous devez utiliser la classe [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) de l'API managée EWS ou l'élément [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) d'EWS.</span><span class="sxs-lookup"><span data-stu-id="2be6e-p101">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't. Both appointments and meetings can be single instances or part of a recurring series, but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent. Internally, Exchange uses the same object for both meetings and appointments. You use the EWS Managed API [Appointment class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="2be6e-109">**Tableau 1. Méthode de l’API managée EWS et opérations EWS pour la mise à jour des rendez-vous et des réunions**</span><span class="sxs-lookup"><span data-stu-id="2be6e-109">**Table 1. EWS Managed API method and EWS operations for updating appointments and meetings**</span></span>

|<span data-ttu-id="2be6e-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="2be6e-110">**EWS Managed API method**</span></span>|<span data-ttu-id="2be6e-111">**Opérations EWS correspondantes**</span><span class="sxs-lookup"><span data-stu-id="2be6e-111">**Corresponding EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2be6e-112">Rendez-vous. Update</span><span class="sxs-lookup"><span data-stu-id="2be6e-112">Appointment.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="2be6e-113">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="2be6e-113">UpdateItem</span></span>](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)<br/><br/>          [<span data-ttu-id="2be6e-114">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="2be6e-114">UpdateItemResponse</span></span>](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) <br/> |
   
## <a name="update-an-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="2be6e-115">Mettre à jour un rendez-vous à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="2be6e-115">Update an appointment by using the EWS Managed API</span></span>
<span data-ttu-id="2be6e-116"><a name="bk_UpdateApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="2be6e-116"><a name="bk_UpdateApptEWSMA"> </a></span></span>

<span data-ttu-id="2be6e-117">L’exemple de code suivant montre comment utiliser l' [objet de rendez-vous](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) pour mettre à jour les propriétés associées à un rendez-vous et la méthode [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) pour enregistrer le rendez-vous dans votre dossier calendrier.</span><span class="sxs-lookup"><span data-stu-id="2be6e-117">The following code example shows how to use the [Appointment object](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) to update properties associated with an appointment and the [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) method to save the appointment to your calendar folder.</span></span> 
  
<span data-ttu-id="2be6e-118">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="2be6e-118">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="2be6e-119">La variable locale `appointmentId` est un identificateur associé à un rendez-vous existant.</span><span class="sxs-lookup"><span data-stu-id="2be6e-119">The local variable  `appointmentId` is an identifier associated with an existing appointment.</span></span> 
  
```cs
// Instantiate an appointment object by binding to it by using the ItemId.
// As a best practice, limit the properties returned to only the ones you need.
Appointment appointment = Appointment.Bind(service, appointmentId, new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End));
string oldSubject = appointment.Subject;
// Update properties on the appointment with a new subject, start time, and end time.
appointment.Subject = appointment.Subject + " moved one hour later and to the day after " + appointment.Start.DayOfWeek + "!";
appointment.Start.AddHours(25);
appointment.End.AddHours(25);
// Unless explicitly specified, the default is to use SendToAllAndSaveCopy.
// This can convert an appointment into a meeting. To avoid this,
// explicitly set SendToNone on non-meetings.
SendInvitationsOrCancellationsMode mode = appointment.IsMeeting ? 
    SendInvitationsOrCancellationsMode.SendToAllAndSaveCopy : SendInvitationsOrCancellationsMode.SendToNone;
// Send the update request to the Exchange server.
appointment.Update(ConflictResolutionMode.AlwaysOverwrite, mode);
// Verify the update.
Console.WriteLine("Subject for the appointment was \"" + oldSubject + "\". The new subject is \"" + appointment.Subject + "\"");

```

## <a name="update-an-appointment-by-using-ews"></a><span data-ttu-id="2be6e-120">Mettre à jour un rendez-vous à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="2be6e-120">Update an appointment by using EWS</span></span>
<span data-ttu-id="2be6e-121"><a name="bk_UpdateApptEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2be6e-121"><a name="bk_UpdateApptEWS"> </a></span></span>

<span data-ttu-id="2be6e-122">Les codes XML de demande et de réponse dans les exemples suivants correspondent aux appels effectués par le code de l’API managée EWS dans [Update a rendez-vous à l’aide de l’API managée EWS](#bk_UpdateApptEWSMA).</span><span class="sxs-lookup"><span data-stu-id="2be6e-122">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Update an appointment by using the EWS Managed API](#bk_UpdateApptEWSMA).</span></span>
  
<span data-ttu-id="2be6e-123">L’exemple suivant montre le code XML de la demande lorsque vous utilisez l’opération [UpdateItem](https://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) pour mettre à jour un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="2be6e-123">The following example shows the request XML when you use the [UpdateItem](https://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) operation to update an appointment.</span></span> 
  
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
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToNone">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAAB" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Tennis Lesson moved one hour later and to the day after Wednesday!</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="2be6e-124">L’exemple suivant montre le code XML renvoyé en réponse à une demande [UpdateItem](https://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2be6e-124">The following example shows the XML that is returned in response to an [UpdateItem](https://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) request.</span></span> <span data-ttu-id="2be6e-125">[!REMARQUE] Les attributs **ItemId** et **ChangeKey** ont été réduits pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="2be6e-125">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="815" MinorBuildNumber="6" Version="V2_7" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exc
hange/services/2006/types">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAAB" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>0</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </m:UpdateItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-a-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="2be6e-126">Mettre à jour une réunion à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="2be6e-126">Update a meeting by using the EWS Managed API</span></span>
<span data-ttu-id="2be6e-127"><a name="bk_UpdateMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="2be6e-127"><a name="bk_UpdateMtgEWSMA"> </a></span></span>

<span data-ttu-id="2be6e-128">Lors de la mise à jour d’une réunion, outre l’enregistrement de l’élément de rendez-vous modifié dans le dossier calendrier, vous souhaitez généralement envoyer aux participants des demandes de réunion mises à jour.</span><span class="sxs-lookup"><span data-stu-id="2be6e-128">When you update a meeting, in addition to saving the modified appointment item to the calendar folder, you also typically want to send updated meeting requests to attendees.</span></span> <span data-ttu-id="2be6e-129">L’exemple de code suivant montre comment mettre à jour une réunion et envoyer des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="2be6e-129">The following code example shows how to update a meeting and send meeting requests.</span></span>
  
<span data-ttu-id="2be6e-130">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="2be6e-130">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="2be6e-131">La variable locale `meetingId` est un identificateur qui est associé à un rendez-vous existant.</span><span class="sxs-lookup"><span data-stu-id="2be6e-131">The local variable  `meetingId` is an identifier that is associated with an existing appointment.</span></span> 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet(AppointmentSchema.Subject, 
                                                                           AppointmentSchema.Location, 
                                                                           AppointmentSchema.RequiredAttendees, 
                                                                           AppointmentSchema.Resources));
string oldSubject = meeting.Subject;
// Update properties on the appointment with a new subject, location, an additional required attendee, and a resource.
meeting.Subject = "Team building exercise has moved!";
meeting.Location = "4567 Contoso Way, Redmond, OH 33333, USA";
meeting.RequiredAttendees.Add("alisa@contoso.com");
meeting.Resources.Add("dlpprojector@contoso.com");
// Send the update request to the Exchange server.
meeting.Update(ConflictResolutionMode.AlwaysOverwrite, SendInvitationsOrCancellationsMode.SendToAllAndSaveCopy);
// Verify the update.
Console.WriteLine("Subject for the meeting was \"" + oldSubject + "\". The new subject is \"" + meeting.Subject + "\"");

```

<span data-ttu-id="2be6e-132">Après avoir défini les propriétés sur [l’objet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) appointment, enregistrez la réunion dans votre dossier calendrier et envoyez les demandes de réunion mises à jour à l’aide de la méthode [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2be6e-132">After setting the properties on the [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object, save the meeting to your calendar folder and send updated meeting requests by using the [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="2be6e-133">Vous pouvez transmettre l’une des deux valeurs d’énumération en tant que paramètres lorsque vous appelez la méthode [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) :</span><span class="sxs-lookup"><span data-stu-id="2be6e-133">You can pass in one of two enumeration values as parameters when you call the [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) method:</span></span> 
  
- <span data-ttu-id="2be6e-134">[ConflictResolutionMode, énumération](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conflictresolutionmode%28v=exchg.80%29.aspx) : détermine le mode de traitement des États en conflit entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="2be6e-134">[ConflictResolutionMode enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conflictresolutionmode%28v=exchg.80%29.aspx) — Determines how conflicting states between client and server are handled.</span></span> 
    
- <span data-ttu-id="2be6e-135">[SendInvitationsOrCancellationsMode, énumération](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsorcancellationsmode%28v=exchg.80%29.aspx) : affecte l’envoi et l’enregistrement des demandes de mise à jour de réunion.</span><span class="sxs-lookup"><span data-stu-id="2be6e-135">[SendInvitationsOrCancellationsMode enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsorcancellationsmode%28v=exchg.80%29.aspx) — Affects the sending and saving of meeting update requests.</span></span> 
    
<span data-ttu-id="2be6e-136">Lorsque vous définissez la valeur d’énumération [ConflictResolutionMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conflictresolutionmode%28v=exchg.80%29.aspx) sur **AlwaysOverwrite**, votre version de la réunion sera toujours enregistrée dans le dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="2be6e-136">When you set the [ConflictResolutionMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conflictresolutionmode%28v=exchg.80%29.aspx) enumeration value to **AlwaysOverwrite**, your version of the meeting will always be saved to the calendar folder.</span></span>
  
## <a name="update-a-meeting-by-using-ews"></a><span data-ttu-id="2be6e-137">Mettre à jour une réunion à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="2be6e-137">Update a meeting by using EWS</span></span>
<span data-ttu-id="2be6e-138"><a name="bk_UpdateMtgEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="2be6e-138"><a name="bk_UpdateMtgEWS"> </a></span></span>

<span data-ttu-id="2be6e-139">Les codes XML de demande et de réponse dans les exemples suivants correspondent aux appels effectués par le code de l’API managée EWS dans [mettre à jour une réunion à l’aide de l’API managée EWS](#bk_UpdateMtgEWSMA).</span><span class="sxs-lookup"><span data-stu-id="2be6e-139">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Update a meeting by using the EWS Managed API](#bk_UpdateMtgEWSMA).</span></span> 
  
<span data-ttu-id="2be6e-140">L’exemple suivant montre le code XML de la demande lorsque vous utilisez l’opération [UpdateItem](https://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) pour mettre à jour une réunion.</span><span class="sxs-lookup"><span data-stu-id="2be6e-140">The following example shows the request XML when you use the [UpdateItem](https://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) operation to update a meeting.</span></span> 
  
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
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToAllAndSaveCopy">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:CalendarItem>
                <t:Subject>Team building exercise has moved!</t:Subject>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Location" />
              <t:CalendarItem>
                <t:Location>4567 Contoso Way, Redmond, OH 33333, USA</t:Location>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:RequiredAttendees" />
              <t:CalendarItem>
                <t:RequiredAttendees>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Mack.Chaves@contoso.com</t:Name>
                      <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:Name>Sadie.Daniels@contoso.com</t:Name>
                      <t:EmailAddress>Sadie.Daniels@contoso.com</t:EmailAddress>
                      <t:RoutingType>SMTP</t:RoutingType>
                    </t:Mailbox>
                  </t:Attendee>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:EmailAddress>alisa@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                </t:RequiredAttendees>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Resources" />
              <t:CalendarItem>
                <t:Resources>
                  <t:Attendee>
                    <t:Mailbox>
                      <t:EmailAddress>dlpprojector@contoso.com</t:EmailAddress>
                    </t:Mailbox>
                  </t:Attendee>
                </t:Resources>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

 <span data-ttu-id="2be6e-141">L’exemple suivant montre le code XML renvoyé en réponse à une demande [UpdateItem](https://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2be6e-141">The following example shows the XML that is returned in response to an [UpdateItem](https://msdn.microsoft.com/library/34643d58-2743-45b0-a08d-bff6dc1da61d%28Office.15%29.aspx) request.</span></span> <span data-ttu-id="2be6e-142">Les attributs **ChangeKey** et **ItemId** ont été réduits pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="2be6e-142">The **ChangeKey** and **ItemId** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="815" MinorBuildNumber="6" Version="V2_7" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
          <m:ConflictResults>
            <t:Count>0</t:Count>
          </m:ConflictResults>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </m:UpdateItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="2be6e-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2be6e-143">See also</span></span>

- [<span data-ttu-id="2be6e-144">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2be6e-144">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)   
- [<span data-ttu-id="2be6e-145">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="2be6e-145">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)   
- [<span data-ttu-id="2be6e-146">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2be6e-146">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="2be6e-147"> Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2be6e-147">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="2be6e-148">Proposer une nouvelle heure de réunion à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2be6e-148">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    

