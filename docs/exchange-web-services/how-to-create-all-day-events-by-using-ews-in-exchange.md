---
title: Créer des événements sur une journée entière à l'aide d’EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Découvrez comment créer des événements sur une journée entière à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 6be638c17cc0e0c86fa6b4217169aa7259dfd4aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456863"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a><span data-ttu-id="5f536-103">Créer des événements sur une journée entière à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5f536-103">Create all-day events by using EWS in Exchange</span></span>

<span data-ttu-id="5f536-104">Découvrez comment créer des événements sur une journée entière à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f536-104">Learn how to create all-day events by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="5f536-105">Les événements d’une journée entière permettent de représenter un événement qui se produit pendant une journée ou plusieurs jours, par exemple, un congé ou des jours de congés.</span><span class="sxs-lookup"><span data-stu-id="5f536-105">All-day events provide a way to represent something that happens for an entire day or multiple days—for example, a holiday, or vacation days.</span></span> <span data-ttu-id="5f536-106">La création d’événements d’une journée entière avec l’API managée EWS ou EWS est un Snap.</span><span class="sxs-lookup"><span data-stu-id="5f536-106">Creating all-day events with the EWS Managed API or EWS is a snap.</span></span> <span data-ttu-id="5f536-107">Cela revient à [créer des rendez-vous](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), mais avec quelques petites modifications.</span><span class="sxs-lookup"><span data-stu-id="5f536-107">It's just like [creating appointments](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), but with a few small changes.</span></span>
  
## <a name="setting-start-and-end-times"></a><span data-ttu-id="5f536-108">Définition des heures de début et de fin</span><span class="sxs-lookup"><span data-stu-id="5f536-108">Setting start and end times</span></span>

<span data-ttu-id="5f536-109">Par définition, les événements d’une journée entière commencent à minuit un jour donné et se terminent 24 heures (ou un multiple de 24 heures) plus tard.</span><span class="sxs-lookup"><span data-stu-id="5f536-109">By definition, all-day events start at midnight on a specific day, and end 24 hours (or a multiple of 24 hours) later.</span></span> <span data-ttu-id="5f536-110">Toutefois, l’API managée EWS et EWS vous permettent de spécifier des heures autres que minuit lors de la création d’événements d’une journée entière.</span><span class="sxs-lookup"><span data-stu-id="5f536-110">However, the EWS Managed API and EWS allow you to specify times other than midnight when creating all day events.</span></span> <span data-ttu-id="5f536-111">Cela peut entraîner un comportement involontaire si vous ne savez pas comment ces heures sont traduites sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="5f536-111">This can lead to unintended behavior if you're not aware of how these times get translated on the server.</span></span>
  
<span data-ttu-id="5f536-112">Lors de la réception d’une demande de création d’un événement d’une journée entière avec une date de début et/ou de fin non minuit (dans le [fuseau horaire de la demande ou du rendez-vous](time-zones-and-ews-in-exchange.md)), les heures sont ajustées à minuit dans le fuseau horaire approprié en fonction des règles suivantes :</span><span class="sxs-lookup"><span data-stu-id="5f536-112">When a request is received to create a new all-day event with non-midnight (in the [time zone of the request or appointment](time-zones-and-ews-in-exchange.md)) start and/or end times, those times get adjusted to midnight in the appropriate time zone according to the following rules:</span></span>
  
- <span data-ttu-id="5f536-113">Les heures de début non minuit sont ajustées à minuit avant l’heure spécifiée.</span><span class="sxs-lookup"><span data-stu-id="5f536-113">Non-midnight start times are adjusted to the midnight prior to the time specified.</span></span> <span data-ttu-id="5f536-114">Par exemple, 1:00 PM le 6 juin est ajusté à 12:00 AM le 6 juin.</span><span class="sxs-lookup"><span data-stu-id="5f536-114">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 6.</span></span>
    
- <span data-ttu-id="5f536-115">Les heures de fin non minuit sont ajustées à minuit après l’heure spécifiée.</span><span class="sxs-lookup"><span data-stu-id="5f536-115">Non-midnight end times are adjusted to the midnight after the time specified.</span></span> <span data-ttu-id="5f536-116">Par exemple, 1:00 PM le 6 juin est ajusté à 12:00 AM le 7 juin.</span><span class="sxs-lookup"><span data-stu-id="5f536-116">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 7.</span></span>
    
<span data-ttu-id="5f536-117">Par conséquent, l’événement d’une journée entière que vous créez est toujours inclus dans l’heure de début et de fin que vous spécifiez, mais peut réclamer du temps supplémentaire sur le calendrier de l’utilisateur en raison du changement de minuit.</span><span class="sxs-lookup"><span data-stu-id="5f536-117">So the all-day event that you create is always inclusive of the start and end time that you specify, but might claim additional time on the user's calendar due to the shift to midnight.</span></span> <span data-ttu-id="5f536-118">Étant donné que le serveur ajustera les heures de début et de fin à minuit, nous vous recommandons de spécifier votre heure de début et de fin à minuit afin d’éviter toute modification involontaire de ces heures.</span><span class="sxs-lookup"><span data-stu-id="5f536-118">Because the server will adjust the start and end time to midnight, we recommend that you specify your start and end time at midnight to avoid any unintended changes to the times.</span></span>
  
<span data-ttu-id="5f536-119">Il est également important de prendre en compte les fuseaux horaires lors de la création d’événements sur une journée entière.</span><span class="sxs-lookup"><span data-stu-id="5f536-119">It's also important to consider time zones when creating all-day events.</span></span> <span data-ttu-id="5f536-120">Étant donné que le serveur Exchange applique une heure de début et de fin de minuit dans le fuseau horaire de la demande ou du rendez-vous, l’affichage de l’événement d’une journée entière dans un client configuré pour un fuseau horaire différent peut produire des résultats inattendus.</span><span class="sxs-lookup"><span data-stu-id="5f536-120">Because the Exchange server enforces a midnight start and end time in the time zone of the request or appointment, viewing that all-day event in a client configured for a different time zone can yield unexpected results.</span></span> <span data-ttu-id="5f536-121">Selon le client, il peut apparaître comme un événement d’une journée entière avec des jours supplémentaires que vous n’avez pas prévu d’inclure, ou il peut ne pas apparaître comme un événement d’une journée entière.</span><span class="sxs-lookup"><span data-stu-id="5f536-121">Depending on the client, it might appear as an all-day event with extra days that you did not intend to include, or it might not appear as an all-day event altogether.</span></span> <span data-ttu-id="5f536-122">Pour cette raison, nous vous recommandons d’utiliser le fuseau horaire préféré de l’utilisateur chaque fois que cela est possible lorsque vous créez des événements sur une journée entière.</span><span class="sxs-lookup"><span data-stu-id="5f536-122">Because of this, we recommend that you use the user's preferred time zone whenever possible when you create all-day events.</span></span>
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a><span data-ttu-id="5f536-123">Créer un événement d’une journée entière à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5f536-123">Create an all-day event by using the EWS Managed API</span></span>

<span data-ttu-id="5f536-124">L’exemple suivant montre comment utiliser l’API managée EWS pour créer un événement d’une journée entière, en commençant à la date spécifiée par le paramètre _StartDate_ et en fonction du nombre de jours spécifié par le paramètre _numDays_ .</span><span class="sxs-lookup"><span data-stu-id="5f536-124">The following example shows how to use the EWS Managed API to create an all-day event, starting on the date specified by the  _startDate_ parameter and lasting for the number of days specified by the  _numDays_ parameter.</span></span> <span data-ttu-id="5f536-125">Notez que le rendez-vous sera créé dans le fuseau horaire spécifié par la propriété [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5f536-125">Note that the appointment will be created in the time zone specified by the [ExchangeService.TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="5f536-126">Cet exemple part du principe que l’objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) transmis dans le paramètre _service_ a été initialisé avec des valeurs valides pour les [informations d’identification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et les propriétés de l' [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5f536-126">This example assumes that the [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object passed in the  _service_ parameter has been initialized with valid values for the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
static void CreateAllDayAppointment(ExchangeService service, DateTime startDate, int numDays)
{
    // Best practice is to set the start date to midnight
    // on the first day of the all-day event.
    DateTime startDateMidnight = startDate.Date;
    // The end date should be midnight on the first day
    // after the event.
    DateTime endDateMidnight = startDateMidnight.AddDays(numDays);
    Appointment allDayEvent = new Appointment(service);
    // Set IsAllDayEvent to true.
    allDayEvent.IsAllDayEvent = true;
    // Set other properties.
    allDayEvent.Subject = "Vacation";
    allDayEvent.LegacyFreeBusyStatus = LegacyFreeBusyStatus.OOF;
    allDayEvent.Start = startDateMidnight;
    allDayEvent.End = endDateMidnight;
    // Save the appointment.
    try
    {
        allDayEvent.Save(WellKnownFolderName.Calendar, SendInvitationsMode.SendToNone);
        Console.WriteLine("All day event created.");
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving all day event: {0}", ex.Message);
    }
}
```

## <a name="create-an-all-day-event-by-using-ews"></a><span data-ttu-id="5f536-127">Créer un événement d’une journée entière à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="5f536-127">Create an all-day event by using EWS</span></span>

<span data-ttu-id="5f536-128">L’exemple suivant montre une demande d' [opération CREATEITEM](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS pour créer un événement sur une journée entière.</span><span class="sxs-lookup"><span data-stu-id="5f536-128">The following example shows an EWS [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request to create an all-day event.</span></span> <span data-ttu-id="5f536-129">Le rendez-vous est créé dans le fuseau horaire est, comme indiqué par l’élément [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5f536-129">The appointment is created in the Eastern time zone, as indicated by the [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="5f536-130">Notez que la partie heure des valeurs des éléments de [début](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) et de [fin](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) est comprise entre 04:00Z, qui est convertie en minuit dans le fuseau horaire est lors de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="5f536-130">Notice that the time portion of the values of the [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) and [End](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) elements are both 04:00Z, which converts to midnight in the Eastern time zone during daylight saving time.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Vacation</t:Subject>
          <t:Start>2014-06-09T04:00:00.000Z</t:Start>
          <t:End>2014-06-10T04:00:00.000Z</t:End>
          <t:IsAllDayEvent>true</t:IsAllDayEvent>
          <t:LegacyFreeBusyStatus>OOF</t:LegacyFreeBusyStatus>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="5f536-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5f536-131">See also</span></span>


- [<span data-ttu-id="5f536-132">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5f536-132">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="5f536-133">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="5f536-133">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="5f536-134">Fuseaux horaires et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5f536-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    

