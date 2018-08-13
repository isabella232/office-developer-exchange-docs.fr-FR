---
title: Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fdea70a4-9267-4e5d-9152-b749e2acc3b0
description: Découvrez comment créer des rendez-vous et des réunions à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 1c840fac2ecca9fb51a28044dfac6299cb4fc038
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754824"
---
# <a name="create-appointments-and-meetings-by-using-ews-in-exchange-2013"></a><span data-ttu-id="23973-103">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="23973-103">How to: Create appointments and meetings by using EWS in Exchange 2013</span></span>

<span data-ttu-id="23973-104">Découvrez comment créer des rendez-vous et des réunions à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="23973-104">Learn how to create appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="23973-p101">La principale différence entre les réunions et les rendez-vous réside dans la présence de participants aux réunions, mais pas aux rendez-vous. Les rendez-vous et les réunions peuvent être des instances uniques ou faire partie d'une série périodique. Cependant, les rendez-vous n'incluant ni participants, ni salles, ni ressources, ne nécessitent pas l'envoi d'un message. En interne, Exchange utilise le même objet pour les réunions et pour les rendez-vous. Pour utiliser les réunions et les rendez-vous, vous devez utiliser la classe [Appointment](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) de l'API managée EWS ou l'élément [CalendarItem](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) d'EWS.</span><span class="sxs-lookup"><span data-stu-id="23973-p101">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't. Both appointments and meetings can be single instances or part of a recurring series, but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent. Internally, Exchange uses the same object for both meetings and appointments. You use the EWS Managed API [Appointment class](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="23973-109">**Tableau 1. Méthodes d'API managée EWS et opérations EWS pour utiliser des rendez-vous et des réunions**</span><span class="sxs-lookup"><span data-stu-id="23973-109">**Table 1. EWS Managed API methods and EWS operations for working with appointments and meetings**</span></span>

|<span data-ttu-id="23973-110">**Méthode d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="23973-110">**EWS Managed API method**</span></span>|<span data-ttu-id="23973-111">**Opération EWS**</span><span class="sxs-lookup"><span data-stu-id="23973-111">**EWS operation**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23973-112">Appointment.Save</span><span class="sxs-lookup"><span data-stu-id="23973-112">Appointment.Save</span></span>](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="23973-113">Opération CreateItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="23973-113">CreateItem operation (calendar item)</span></span>](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="23973-114">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="23973-114">Item.Bind</span></span>](http://msdn.microsoft.com/fr-FR/library/dd634410%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="23973-115">Opération de GetItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="23973-115">GetItem operation (calendar item)</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
   
## <a name="create-an-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="23973-116">Création d’un rendez-vous avec l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="23973-116">Create an appointment by using the EWS Managed API</span></span>
<span data-ttu-id="23973-117"><a name="bk_CreateApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="23973-117"></span></span>

<span data-ttu-id="23973-118">L'exemple de code suivant montre comment utiliser l'objet [Appointment](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) pour créer un rendez-vous, la méthode [Save](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) pour l'enregistrer dans votre dossier de calendrier et la méthode [Item.Bind](http://msdn.microsoft.com/fr-FR/library/dd634410%28v=exchg.80%29.aspx) pour vérifier que le rendez-vous a bien été créé.</span><span class="sxs-lookup"><span data-stu-id="23973-118">The following code example shows how to use the [Appointment object](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) to create an appointment, the [Save](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to save it to your calendar folder, and the [Item.Bind](http://msdn.microsoft.com/fr-FR/library/dd634410%28v=exchg.80%29.aspx) method to verify that the appointment was created.</span></span> 
  
<span data-ttu-id="23973-119">Cet exemple suppose que vous avez été authentifié auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="23973-119">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
Appointment appointment = new Appointment(service);
// Set the properties on the appointment object to create the appointment.
appointment.Subject = "Tennis lesson";
appointment.Body = "Focus on backhand this week.";
appointment.Start = DateTime.Now.AddDays(2);
appointment.End = appointment.Start.AddHours(1);
appointment.Location = "Tennis club";
appointment.ReminderDueBy = DateTime.Now;
// Save the appointment to your calendar.
appointment.Save(SendInvitationsMode.SendToNone);
// Verify that the appointment was created by using the appointment's item ID.
Item item = Item.Bind(service, appointment.Id, new PropertySet(ItemSchema.Subject));
Console.WriteLine("\nAppointment created: " + item.Subject + "\n");

```

<span data-ttu-id="23973-120">Après avoir défini les propriétés sur l'objet Appointment, enregistrez le rendez-vous dans le dossier de calendrier à l'aide de la méthode [Save](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) de l'objet Appointment.</span><span class="sxs-lookup"><span data-stu-id="23973-120">After setting the properties on the appointment object, you save the appointment to the calendar folder by using the appointment object's [Save](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="23973-p102">Lors de la vérification, utilisez l'élément [Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) associé au rendez-vous pour vérifier qu'il se trouve dans le dossier de calendrier. Il est recommandé de limiter le nombre de propriétés renvoyées par le serveur à vos besoins (en l'occurrence, l'objet du rendez-vous).</span><span class="sxs-lookup"><span data-stu-id="23973-p102">Note that in the verification step, you use the item [Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) associated with the appointment to verify that the appointment is in the calendar folder. As a best practice, limit the properties returned by the server to only what you need — in this case, the appointment's subject.</span></span> 
  
## <a name="create-an-appointment-by-using-ews"></a><span data-ttu-id="23973-123">Création d’un rendez-vous avec EWS</span><span class="sxs-lookup"><span data-stu-id="23973-123">Create an appointment by using EWS</span></span>
<span data-ttu-id="23973-124"><a name="bk_CreateApptEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="23973-124"></span></span>

<span data-ttu-id="23973-p103">Les codes XML de demande et de réponse figurant dans les exemples suivants correspondent aux appels effectués par le code de l'API managée EWS à l'étape [Création d'un rendez-vous avec l'API managée EWS](#bk_CreateApptEWSMA). Les codes XML de demande et de réponse qui vérifient que les éléments de rendez-vous se trouvent dans le dossier de calendrier sont également affichés.</span><span class="sxs-lookup"><span data-stu-id="23973-p103">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Create an appointment by using the EWS Managed API](#bk_CreateApptEWSMA). The request and response XML that verifies that the appointment items are in the calendar folder are shown as well.</span></span>
  
<span data-ttu-id="23973-127">L'exemple suivant présente le code XML de demande généré lors de l'utilisation de l'opération [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour créer un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="23973-127">The following example shows the request XML when you use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create an appointment.</span></span> 
  
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
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Tennis lesson</t:Subject>
          <t:Body BodyType="HTML">Focus on backhand this week.</t:Body>
          <t:ReminderDueBy>2013-09-19T14:37:10.732-07:00</t:ReminderDueBy>
          <t:Start>2013-09-21T19:00:00.000Z</t:Start>
          <t:End>2013-09-21T20:00:00.000Z</t:End>
          <t:Location>Tennis club</t:Location>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

 <span data-ttu-id="23973-128">L'exemple suivant présente le code XML de réponse renvoyé par l'opération **CreateItem**.</span><span class="sxs-lookup"><span data-stu-id="23973-128">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="23973-129">Les attributs **ItemId** et **ChangeKey** ont été réduits pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="23973-129">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
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
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="23973-130">L'exemple suivant présente le code XML de demande généré lors de l'utilisation de l'opération [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) pour vérifier que vous avez créé le rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="23973-130">The following example shows the request XML that is generated when you use the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) operation to verify that the appointment was created.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="23973-131">Les attributs **ItemId** et **ChangeKey** ont été réduits pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="23973-131">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
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
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>

```

 <span data-ttu-id="23973-132">L'exemple suivant présente le code XML de réponse renvoyé par l'opération **GetItem**.</span><span class="sxs-lookup"><span data-stu-id="23973-132">The following example shows the response XML that is returned by the **GetItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="23973-133">Les attributs **ItemId** et **ChangeKey** ont été réduits pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="23973-133">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Tennis lesson</t:Subject>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="create-a-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="23973-134">Création d’une réunion avec l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="23973-134">Create a meeting by using the EWS Managed API</span></span>
<span data-ttu-id="23973-135"><a name="bk_CreateMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="23973-135"></span></span>

<span data-ttu-id="23973-p104">En général, lorsque vous créez une réunion, vous souhaitez non seulement enregistrer un élément dans le dossier de calendrier, mais également envoyer des demandes de réunion aux participants. L’exemple de code suivant indique comment créer une réunion et envoyer des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="23973-p104">When you create a meeting, in addition to saving an item to the calendar folder, you also typically want to send meeting requests to attendees. The following code example shows how to create a meeting and send meeting requests.</span></span>
  
<span data-ttu-id="23973-138">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="23973-138">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
Appointment meeting = new Appointment(service);
// Set the properties on the meeting object to create the meeting.
meeting.Subject = "Team building exercise";
meeting.Body = "Let's learn to really work as a team and then have lunch!";
meeting.Start = DateTime.Now.AddDays(2);            
meeting.End = meeting.Start.AddHours(4);
meeting.Location = "Conference Room 12";
meeting.RequiredAttendees.Add("Mack@contoso.com");
meeting.RequiredAttendees.Add("Sadie@contoso.com");
meeting.OptionalAttendees.Add("Magdalena@contoso.com");
meeting.ReminderMinutesBeforeStart = 60;
// Save the meeting to the Calendar folder and send the meeting request.
meeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);
// Verify that the meeting was created.
Item item = Item.Bind(service, meeting.Id, new PropertySet(ItemSchema.Subject));
Console.WriteLine("\nMeeting created: " + item.Subject + "\n");

```

<span data-ttu-id="23973-p105">Après avoir défini les propriétés sur l'objet [Appointment](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx), enregistrez la réunion dans votre dossier de calendrier à l'aide de la méthode [Save](http://msdn.microsoft.com/fr-FR/library/dd635394%28v=exchg.80%29.aspx). Lorsque vous définissez la valeur d'énumération [SendInvitationsMode](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.sendinvitationsmode%28v=exchg.80%29.aspx) sur **SendOnlyToAll** ou **SendToAllAndSaveCopy**, des invitations sont envoyées aux participants.</span><span class="sxs-lookup"><span data-stu-id="23973-p105">After setting the properties on the [Appointment](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object, save the meeting to your calendar folder by using the [Save](http://msdn.microsoft.com/fr-FR/library/dd635394%28v=exchg.80%29.aspx) method. When you set the [SendInvitationsMode](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.sendinvitationsmode%28v=exchg.80%29.aspx) enumeration value to **SendOnlyToAll** or **SendToAllAndSaveCopy**, invitations are sent to attendees.</span></span>
  
<span data-ttu-id="23973-p106">Utilisez la propriété [Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l'élément associé à la réunion pour vérifier qu'il se trouve bien dans le dossier de calendrier. Il est recommandé de limiter le nombre de propriétés renvoyées à vos besoins (en l'occurrence, le sujet de la réunion).</span><span class="sxs-lookup"><span data-stu-id="23973-p106">Use the item [Id](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) associated with the meeting to verify that it was saved in the calendar folder. As a best practice, limit the properties returned by the server to only what you need - in this case, the meeting's subject.</span></span> 
  
## <a name="create-a-meeting-by-using-ews"></a><span data-ttu-id="23973-143">Création d’une réunion avec EWS</span><span class="sxs-lookup"><span data-stu-id="23973-143">Create a meeting by using EWS</span></span>
<span data-ttu-id="23973-144"><a name="bk_CreateMtgEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="23973-144"></span></span>

<span data-ttu-id="23973-p107">Les codes XML de demande et de réponse figurant dans les exemples suivants correspondent aux appels effectués par le code de l'API managée EWS à l'étape [Création d'une réunion avec l'API managée EWS](#bk_CreateMtgEWSMA). Les codes XML de demande et de réponse qui vérifient que les éléments de réunion se trouvent dans le dossier de calendrier sont également affichés.</span><span class="sxs-lookup"><span data-stu-id="23973-p107">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Create a meeting by using the EWS Managed API](#bk_CreateMtgEWSMA). The request and response XML that verifies that the meeting items are in the calendar folder are shown as well.</span></span>
  
<span data-ttu-id="23973-147">L'exemple suivant présente le code XML de demande lors de l'utilisation de l'opération [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour créer une réunion.</span><span class="sxs-lookup"><span data-stu-id="23973-147">The following example shows the request XML when you use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a meeting.</span></span> 
  
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
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Team building exercise</t:Subject>
          <t:Body BodyType="HTML">Let's learn to really work as a team and then have lunch!</t:Body>
          <t:ReminderMinutesBeforeStart>60</t:ReminderMinutesBeforeStart>
          <t:Start>2013-09-21T16:00:00.000Z</t:Start>
          <t:End>2013-09-21T20:00:00.000Z</t:End>
          <t:Location>Conference Room 12</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Mack.Chaves@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Sadie.Daniels@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
          <t:OptionalAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>Magdalena.Kemp@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:OptionalAttendees>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="23973-148">L'exemple suivant présente le code XML de réponse renvoyé par l'opération **CreateItem**.</span><span class="sxs-lookup"><span data-stu-id="23973-148">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="23973-149">Les attributs **ItemId** et **ChangeKey** ont été réduits pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="23973-149">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
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

<span data-ttu-id="23973-150">L'exemple suivant présente le code XML de demande généré lors de l'utilisation de l'opération [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) pour vérifier que vous avez créé la réunion.</span><span class="sxs-lookup"><span data-stu-id="23973-150">The following example shows the request XML that is generated by the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) operation when you verify that the meeting was created.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="23973-151">Les attributs **ItemId** et **ChangeKey** ont été réduits pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="23973-151">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```xml
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
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="23973-152">L'exemple suivant présente le code XML de réponse renvoyé par l'opération **GetItem**.</span><span class="sxs-lookup"><span data-stu-id="23973-152">The following example shows the response XML that is returned by the **GetItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="23973-153">Les** attributs ItemId** et **ChangeKey** ont été réduits pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="23973-153">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
              <t:Subject>Team building exercise</t:Subject>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="23973-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="23973-154">See also</span></span>

- [<span data-ttu-id="23973-155">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="23973-155">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)  
- [<span data-ttu-id="23973-156">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="23973-156">How to: Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="23973-157">Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="23973-157">How to: Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="23973-158"> Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="23973-158">How to: Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="23973-159">Proposer une nouvelle heure de réunion à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="23973-159">How to: Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    

