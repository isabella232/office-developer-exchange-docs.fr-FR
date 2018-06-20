---
title: Créer des événements à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Découvrez comment créer des événements à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 0547fdf0ca92ba0648caeb5de6940d90d2a8ff46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754815"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a><span data-ttu-id="a2a3c-103">Créer des événements à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a2a3c-103">Create all-day events by using EWS in Exchange</span></span>

<span data-ttu-id="a2a3c-104">Découvrez comment créer des événements à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-104">Learn how to create all-day events by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="a2a3c-105">Événements sur une journée entière offrent un moyen pour représenter quelque chose qui se produit pour une journée entière ou plusieurs jours, par exemple, un jour férié ou des jours de congés.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-105">All-day events provide a way to represent something that happens for an entire day or multiple days—for example, a holiday, or vacation days.</span></span> <span data-ttu-id="a2a3c-106">Création d’événements avec les API managées EWS est un composant logiciel enfichable.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-106">Creating all-day events with the EWS Managed API or EWS is a snap.</span></span> <span data-ttu-id="a2a3c-107">Il est tout comme la [Création de rendez-vous](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), mais avec quelques modifications mineures.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-107">It's just like [creating appointments](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), but with a few small changes.</span></span>
  
## <a name="setting-start-and-end-times"></a><span data-ttu-id="a2a3c-108">Définition des heures de début et de fin</span><span class="sxs-lookup"><span data-stu-id="a2a3c-108">Setting start and end times</span></span>

<span data-ttu-id="a2a3c-109">Par définition, les événements d’une journée démarrent à minuit sur un jour spécifique et fin 24 heures (ou un multiple de 24 heures) ultérieurement.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-109">By definition, all-day events start at midnight on a specific day, and end 24 hours (or a multiple of 24 hours) later.</span></span> <span data-ttu-id="a2a3c-110">Toutefois, les API managées EWS permettent de spécifier le temps de minuit lors de la création de tous les événements du jour.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-110">However, the EWS Managed API and EWS allow you to specify times other than midnight when creating all day events.</span></span> <span data-ttu-id="a2a3c-111">Cela peut entraîner un comportement inattendu si vous n’êtes pas au courant de la façon dont ces heures obtient traduits sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-111">This can lead to unintended behavior if you're not aware of how these times get translated on the server.</span></span>
  
<span data-ttu-id="a2a3c-112">Lorsqu’une demande est reçue pour créer un nouvel événement d’une journée entière avec non minuit (dans le [fuseau horaire de la demande ou un rendez-vous](time-zones-and-ews-in-exchange.md)) début et/ou à la fin des heures, les durées ajustées à minuit dans le fuseau horaire approprié en fonction des règles suivantes :</span><span class="sxs-lookup"><span data-stu-id="a2a3c-112">When a request is received to create a new all-day event with non-midnight (in the [time zone of the request or appointment](time-zones-and-ews-in-exchange.md)) start and/or end times, those times get adjusted to midnight in the appropriate time zone according to the following rules:</span></span>
  
- <span data-ttu-id="a2a3c-113">Heures de début non-minuit sont ajustées le minuit avant l’heure spécifiée.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-113">Non-midnight start times are adjusted to the midnight prior to the time specified.</span></span> <span data-ttu-id="a2a3c-114">Par exemple, 1:00 PM 6 juin est réglé à 12:00 AM 6 juin.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-114">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 6.</span></span>
    
- <span data-ttu-id="a2a3c-115">Heure de fin non-minuit est ajustées le minuit après l’heure spécifiée.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-115">Non-midnight end times are adjusted to the midnight after the time specified.</span></span> <span data-ttu-id="a2a3c-116">Par exemple, 1:00 PM 6 juin est réglé à 12:00 AM 7 juin.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-116">For example, 1:00 PM on June 6 gets adjusted to 12:00 AM on June 7.</span></span>
    
<span data-ttu-id="a2a3c-117">Afin que vous créez la journée est toujours y compris l’heure de début et de fin que vous spécifiez, mais pouvez demander davantage de temps sur l’utilisateur du calendrier en raison du travail d’équipe à minuit.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-117">So the all-day event that you create is always inclusive of the start and end time that you specify, but might claim additional time on the user's calendar due to the shift to midnight.</span></span> <span data-ttu-id="a2a3c-118">Car le serveur ajuste l’heure de début et de fin à minuit, nous vous recommandons de spécifier votre heure de début et de fin à minuit pour éviter toute modification accidentelle aux fois.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-118">Because the server will adjust the start and end time to midnight, we recommend that you specify your start and end time at midnight to avoid any unintended changes to the times.</span></span>
  
<span data-ttu-id="a2a3c-119">Il est également important de prendre en compte les fuseaux horaires lors de la création d’événements sur une journée entière.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-119">It's also important to consider time zones when creating all-day events.</span></span> <span data-ttu-id="a2a3c-120">Étant donné que la version d’Exchange server impose une minuit début et heure de fin dans le fuseau horaire de la demande ou d’un rendez-vous, affichage de cet événement d’une journée entière dans un client configuré pour un fuseau horaire différent peut produire des résultats inattendus.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-120">Because the Exchange server enforces a midnight start and end time in the time zone of the request or appointment, viewing that all-day event in a client configured for a different time zone can yield unexpected results.</span></span> <span data-ttu-id="a2a3c-121">Selon le client, il peut apparaître en tant que journée avec jours supplémentaires que vous n’êtes pas à inclure ou celui-ci n’apparaîtra pas entièrement en tant qu’un événement d’une journée entière.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-121">Depending on the client, it might appear as an all-day event with extra days that you did not intend to include, or it might not appear as an all-day event altogether.</span></span> <span data-ttu-id="a2a3c-122">Pour cette raison, nous vous recommandons d’utiliser fuseau horaire préféré son la mesure du possible lorsque vous créez des événements d’une journée.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-122">Because of this, we recommend that you use the user's preferred time zone whenever possible when you create all-day events.</span></span>
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a><span data-ttu-id="a2a3c-123">Créer un événement à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="a2a3c-123">Create an all-day event by using the EWS Managed API</span></span>

<span data-ttu-id="a2a3c-124">L’exemple suivant montre comment utiliser l’API managée EWS pour créer un événement d’une journée entière, commençant à la date spécifiée par le paramètre _startDate_ et une durée pour le nombre de jours spécifié par le paramètre _numDays_ .</span><span class="sxs-lookup"><span data-stu-id="a2a3c-124">The following example shows how to use the EWS Managed API to create an all-day event, starting on the date specified by the  _startDate_ parameter and lasting for the number of days specified by the  _numDays_ parameter.</span></span> <span data-ttu-id="a2a3c-125">Notez que le rendez-vous sera créé dans le fuseau horaire spécifié par la propriété [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a2a3c-125">Note that the appointment will be created in the time zone specified by the [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="a2a3c-126">Cet exemple suppose que l’objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) transmis dans le paramètre de _service_ a été initialisé avec les valeurs valides pour les propriétés [d’Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) et les [informations d’identification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a2a3c-126">This example assumes that the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object passed in the  _service_ parameter has been initialized with valid values for the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

## <a name="create-an-all-day-event-by-using-ews"></a><span data-ttu-id="a2a3c-127">Créer un événement à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="a2a3c-127">Create an all-day event by using EWS</span></span>

<span data-ttu-id="a2a3c-128">L’exemple suivant montre une demande EWS [opération CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) pour créer un événement d’une journée entière.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-128">The following example shows an EWS [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request to create an all-day event.</span></span> <span data-ttu-id="a2a3c-129">Le rendez-vous est créé dans le fuseau horaire, comme indiqué par l’élément [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a2a3c-129">The appointment is created in the Eastern time zone, as indicated by the [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="a2a3c-130">Notez que la partie heure des valeurs des éléments [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) et [End](http://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) sont les deux 04:00Z, qui convertit à minuit dans le fuseau horaire lors de l’heure d’été.</span><span class="sxs-lookup"><span data-stu-id="a2a3c-130">Notice that the time portion of the values of the [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) and [End](http://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) elements are both 04:00Z, which converts to midnight in the Eastern time zone during daylight saving time.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

## <a name="see-also"></a><span data-ttu-id="a2a3c-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a2a3c-131">See also</span></span>


- [<span data-ttu-id="a2a3c-132">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a2a3c-132">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a2a3c-133">Créer des rendez-vous et réunions à l’aide de EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a2a3c-133">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="a2a3c-134">Fuseaux horaires et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a2a3c-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    

