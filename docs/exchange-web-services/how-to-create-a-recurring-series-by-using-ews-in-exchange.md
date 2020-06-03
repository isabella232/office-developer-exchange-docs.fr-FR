---
title: Créer une série périodique à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 88ed6e87-25f7-4a54-83fa-d757a0ff2528
description: Découvrez comment créer des réunions périodiques à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 1d04bd48c56a1a0e94eb1368166f776b3dfeb23a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456870"
---
# <a name="create-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="36ffd-103">Créer une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="36ffd-103">Create a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="36ffd-104">Découvrez comment créer des réunions périodiques à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="36ffd-104">Learn how to create recurring meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="36ffd-105">La création d’un rendez-vous ou d’une réunion périodique n’est pas très différente de [la création d’une réunion ou d’un rendez-vous unique d’instance](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="36ffd-105">Creating a recurring appointment or meeting isn't all that much different than creating [a single instance appointment or meeting](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span></span> <span data-ttu-id="36ffd-106">Il vous suffit d’affecter des valeurs à quelques propriétés supplémentaires liées à la récurrence.</span><span class="sxs-lookup"><span data-stu-id="36ffd-106">You just need to assign values to a few additional recurrence-related properties.</span></span> <span data-ttu-id="36ffd-107">Celles-ci sont définies sur un objet [rerecurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) de l’objet [ExchangeService.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) Appointment (si vous utilisez l’API managée EWS) ou l’élément enfant de [récurrence](https://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) d’un élément [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) (si vous utilisez EWS).</span><span class="sxs-lookup"><span data-stu-id="36ffd-107">These are set on an [ExchangeService.Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object's [Recurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) object (if you're using the EWS Managed API), or the [Recurrence](https://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) child element of a [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) element (if you're using EWS).</span></span> <span data-ttu-id="36ffd-108">L’un des éléments à prendre en compte lors de la création d’une réunion périodique, au lieu d’une réunion à instance unique, est que l’élément de calendrier que vous créez est le masque périodique d’une série.</span><span class="sxs-lookup"><span data-stu-id="36ffd-108">One thing to consider when you create a recurring, rather than a single-instance meeting, is that the calendar item you create is the recurring master for a series.</span></span> <span data-ttu-id="36ffd-109">Un certain nombre de propriétés ne sont définies que sur un masque périodique ; ces propriétés peuvent vous aider à rechercher, modifier ou supprimer des instances individuelles dans une série.</span><span class="sxs-lookup"><span data-stu-id="36ffd-109">A number of properties are set only on a recurring master; these properties can help you find, modify, or delete individual instances in a series.</span></span> <span data-ttu-id="36ffd-110">Pour cette raison, il peut être utile d’effectuer le suivi de l’ID de la forme de base périodique lorsque vous créez une série périodique.</span><span class="sxs-lookup"><span data-stu-id="36ffd-110">For this reason, it might be useful to keep track of the ID of the recurring master when you create a recurring series.</span></span> 
  
<span data-ttu-id="36ffd-111">**Tableau 1. Propriétés définies sur les éléments de calendrier principal périodiques**</span><span class="sxs-lookup"><span data-stu-id="36ffd-111">**Table 1. Properties set on recurring master calendar items**</span></span>

|<span data-ttu-id="36ffd-112">**Classe ou propriété de l’API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="36ffd-112">**EWS Managed API class or property**</span></span>|<span data-ttu-id="36ffd-113">**Élément XML EWS**</span><span class="sxs-lookup"><span data-stu-id="36ffd-113">**EWS XML element**</span></span>|<span data-ttu-id="36ffd-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="36ffd-114">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="36ffd-115">Classe de récurrence</span><span class="sxs-lookup"><span data-stu-id="36ffd-115">Recurrence class</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence%28v=exchg.80%29.aspx) <br/> <span data-ttu-id="36ffd-116">La classe **Recurrence** est la classe de base d’une classe de modèle dérivée, [IntervalPattern](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.intervalpattern%28v=exchg.80%29.aspx), [RelativeYearlyPattern](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx)ou [YearlyPattern](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="36ffd-116">The **Recurrence** class is the base class for a derived pattern class, either [IntervalPattern](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.intervalpattern%28v=exchg.80%29.aspx), [RelativeYearlyPattern](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx), or [YearlyPattern](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx).</span></span>  <br/> |[<span data-ttu-id="36ffd-117">Récurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="36ffd-117">Recurrence (RecurrenceType)</span></span>](https://msdn.microsoft.com/library/3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12%28Office.15%29.aspx) <br/> |<span data-ttu-id="36ffd-118">Contient des informations relatives à la périodicité, dont le modèle de périodicité (quotidien, hebdomadaire, mensuel, etc.), la date de début et de fin, le nombre d’occurrences, etc.</span><span class="sxs-lookup"><span data-stu-id="36ffd-118">Contains recurrence-related information, including the recurrence pattern (daily, weekly, monthly, and so on), start and end date, number of occurrences, and so on.</span></span>  <br/> |
|[<span data-ttu-id="36ffd-119">FirstOccurrence, propriété</span><span class="sxs-lookup"><span data-stu-id="36ffd-119">FirstOccurrence property</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="36ffd-120">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="36ffd-120">FirstOccurrence</span></span>](https://msdn.microsoft.com/library/d6748860-ce0d-4d2e-b7e4-9ed834f1e45a%28Office.15%29.aspx) <br/> |<span data-ttu-id="36ffd-121">Contient les heures de début et de fin et l’ID d’élément de la première réunion d’une série.</span><span class="sxs-lookup"><span data-stu-id="36ffd-121">Contains the start and end times and the item ID for the first meeting in a series.</span></span>  <br/> |
|[<span data-ttu-id="36ffd-122">LastOccurrence, propriété</span><span class="sxs-lookup"><span data-stu-id="36ffd-122">LastOccurrence property</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="36ffd-123">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="36ffd-123">LastOccurrence</span></span>](https://msdn.microsoft.com/library/c9ef0fcb-4265-4e60-9986-fff0f211d00b%28Office.15%29.aspx) <br/> |<span data-ttu-id="36ffd-124">Contient les heures de début et de fin et l’ID d’élément de la dernière réunion d’une série.</span><span class="sxs-lookup"><span data-stu-id="36ffd-124">Contains the start and end times and the item ID for the last meeting in a series.</span></span>  <br/> |
|[<span data-ttu-id="36ffd-125">ModifiedOccurrences, propriété</span><span class="sxs-lookup"><span data-stu-id="36ffd-125">ModifiedOccurrences property</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="36ffd-126">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="36ffd-126">ModifiedOccurrences</span></span>](https://msdn.microsoft.com/library/552932fc-b3b4-486e-8d73-32c0bb10bd68%28Office.15%29.aspx) <br/> |<span data-ttu-id="36ffd-127">Contient le jeu de toutes les réunions de la série qui ont été modifiées à partir de la périodicité d’origine.</span><span class="sxs-lookup"><span data-stu-id="36ffd-127">Contains the set of all meetings in the series that have been modified from the original recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="36ffd-128">DeletedOccurrences, propriété</span><span class="sxs-lookup"><span data-stu-id="36ffd-128">DeletedOccurrences property</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="36ffd-129">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="36ffd-129">DeletedOccurrences</span></span>](https://msdn.microsoft.com/library/736fb305-9528-4be8-ad37-65d7556edbf2%28Office.15%29.aspx) <br/> |<span data-ttu-id="36ffd-130">Contient l’ensemble de toutes les réunions de la série qui ont été supprimées de la périodicité d’origine.</span><span class="sxs-lookup"><span data-stu-id="36ffd-130">Contains the set of all meetings in the series that have been deleted from the original recurrence pattern.</span></span>  <br/> |
   
<span data-ttu-id="36ffd-131">Étant donné que les réunions sont essentiellement des rendez-vous qui incluent des participants, les exemples de code de cet article montrent comment créer des réunions périodiques.</span><span class="sxs-lookup"><span data-stu-id="36ffd-131">Because meetings are essentially appointments that include attendees, the code examples in this article show how to create recurring meetings.</span></span> <span data-ttu-id="36ffd-132">Si vous souhaitez créer un rendez-vous périodique, vous pouvez modifier les exemples en supprimant le code lié aux participants.</span><span class="sxs-lookup"><span data-stu-id="36ffd-132">If you want to create a recurring appointment, you can modify the examples by removing code related to attendees.</span></span>
  
## <a name="create-a-recurring-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="36ffd-133">Créer une réunion périodique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="36ffd-133">Create a recurring meeting by using the EWS Managed API</span></span>
<span data-ttu-id="36ffd-134"><a name="bk_CreateMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="36ffd-134"><a name="bk_CreateMtgEWSMA"> </a></span></span>

<span data-ttu-id="36ffd-135">L’exemple de code suivant montre comment créer une réunion périodique.</span><span class="sxs-lookup"><span data-stu-id="36ffd-135">The following code example shows how to create a recurring meeting.</span></span> <span data-ttu-id="36ffd-136">Tout d’abord, affectez des valeurs aux propriétés d’un [objet de rendez-vous](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) utilisé pour créer une réunion, puis utilisez la méthode [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) pour enregistrer la série périodique dans votre dossier de calendrier et envoyer les demandes de réunion aux participants.</span><span class="sxs-lookup"><span data-stu-id="36ffd-136">First, assign values to the properties of an [Appointment object](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) used to create a meeting, then use the [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to save the recurring series to your calendar folder, and send meeting requests to your attendees.</span></span> <span data-ttu-id="36ffd-137">Enfin, utilisez la méthode appointment [. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) pour examiner les valeurs définies sur le masque périodique de la série périodique que vous venez de créer.</span><span class="sxs-lookup"><span data-stu-id="36ffd-137">Finally, use the [Appointment.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) method to look at the values set on the recurring master for the recurring series you just created.</span></span> 
  
<span data-ttu-id="36ffd-138">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="36ffd-138">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="36ffd-139">La méthode de cet exemple renvoie l' [ID d’élément](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) du masque périodique de la série périodique.</span><span class="sxs-lookup"><span data-stu-id="36ffd-139">The method in this example returns the [item ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the recurring series' recurring master.</span></span> 
  
```cs
public static ItemId CreateARecurringMeeting(ExchangeService service)
{        Appointment recurrMeeting = new Appointment(service);
        // Set the properties you need to create a meeting.
        recurrMeeting.Subject = "Weekly Update Meeting";
        recurrMeeting.Body = "Come hear about how the project is coming along!";
        recurrMeeting.Start = DateTime.Now.AddDays(1);
        recurrMeeting.End = recurrMeeting.Start.AddHours(1);
        recurrMeeting.Location = "Contoso Main Gallery";
        recurrMeeting.RequiredAttendees.Add("Mack@contoso.com");
        recurrMeeting.RequiredAttendees.Add("Sadie@contoso.com");
        recurrMeeting.RequiredAttendees.Add("Magdalena@contoso.com"); recurrMeeting.ReminderMinutesBeforeStart = 30;
             
        DayOfTheWeek[] dow = new DayOfTheWeek[] { (DayOfTheWeek)recurrMeeting.Start.DayOfWeek };
        // The following are the recurrence-specific properties for the meeting.
        recurrMeeting.Recurrence = new Recurrence.WeeklyPattern(recurrMeeting.Start.Date, 1, dow);
        recurrMeeting.Recurrence.StartDate = recurrMeeting.Start.Date;
        recurrMeeting.Recurrence.NumberOfOccurrences = 10;
        // This method results in in a CreateItem call to EWS.
        recurrMeeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);
        // Retrieve the meeting subject and the properties that are set on a recurring master when a recurring series is created.
        recurrMeeting = Appointment.Bind(service, recurrMeeting.Id, new PropertySet(AppointmentSchema.Subject,
                                                                                    AppointmentSchema.AppointmentType, 
                                                                                    AppointmentSchema.Recurrence, 
                                                                                    AppointmentSchema.FirstOccurrence,
                                                                                    AppointmentSchema.LastOccurrence,
                                                                                    AppointmentSchema.ModifiedOccurrences,
                                                                                    AppointmentSchema.DeletedOccurrences));
        // Print out the recurring master properties.
        Console.WriteLine("\nAppointment created: " + recurrMeeting.Subject);
        Console.WriteLine("Appointment Type: {0}\n", recurrMeeting.AppointmentType);
        Console.WriteLine("These property values are always null unless the item is a recurring master:\n");
        Console.WriteLine("\tRecurrence pattern: {0}", recurrMeeting.Recurrence.ToString());
        Console.WriteLine("\tRecurring series start Date: {0}", recurrMeeting.Recurrence.StartDate.ToString());
        Console.WriteLine("\tRecurring series end Date: {0}", 
                        recurrMeeting.Recurrence.EndDate == null ? "Null" : recurrMeeting.Recurrence.EndDate.ToString());
        Console.WriteLine("\tHas end: {0}", recurrMeeting.Recurrence.HasEnd.ToString());
        Console.WriteLine("\tNumber of occurrances: {0}", recurrMeeting.Recurrence.NumberOfOccurrences);
        Console.WriteLine("\tLast 24 characters of the first occurrence's item ID:\t {0}", 
                        recurrMeeting.FirstOccurrence.ItemId.ToString().Substring(144));
        Console.WriteLine("\tLast 24 characters of the last occurrence's item ID:\t {0}", 
                        recurrMeeting.LastOccurrence.ItemId.ToString().Substring(144)); 
        Console.WriteLine("\tModified Occurrences: {0}", 
                        (recurrMeeting.ModifiedOccurrences == null ? "Null" : recurrMeeting.ModifiedOccurrences.Count.ToString()));
        Console.WriteLine("\tDeleted Occurrences: {0}", 
                        recurrMeeting.DeletedOccurrences == null ? "Null" : recurrMeeting.ModifiedOccurrences.Count.ToString());
        // Return the ID of the recurring master.
        return recurrMeeting.Id;
}

```

## <a name="create-a-recurring-meeting-by-using-ews"></a><span data-ttu-id="36ffd-140">Créer une réunion périodique à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="36ffd-140">Create a recurring meeting by using EWS</span></span>
<span data-ttu-id="36ffd-141"><a name="bk_CreateMtgEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="36ffd-141"><a name="bk_CreateMtgEWS"> </a></span></span>

<span data-ttu-id="36ffd-142">Les données XML de demande et de réponse dans les exemples suivants correspondent aux appels effectués pour [créer une réunion périodique à l’aide de l’API managée EWS](#bk_CreateMtgEWSMA).</span><span class="sxs-lookup"><span data-stu-id="36ffd-142">The request and response XML in the following examples correspond to calls made to [create a recurring meeting by using the EWS Managed API](#bk_CreateMtgEWSMA).</span></span> <span data-ttu-id="36ffd-143">Notez qu’il n’est pas possible de définir des valeurs propres à la périodicité sur l’élément de [périodicité](https://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) , mais la demande est essentiellement identique à celle que vous utiliseriez pour créer un rendez-vous unique.</span><span class="sxs-lookup"><span data-stu-id="36ffd-143">Note that other than setting recurrence-specific values on the [Recurrence](https://msdn.microsoft.com/library/5f164e5b-47b6-4242-b6b9-8d650090a831%28Office.15%29.aspx) element, the request is essentially the same as one you would use to create a single-instance appointment.</span></span> <span data-ttu-id="36ffd-144">L'exemple suivant présente le code XML de demande lors de l'utilisation de l'opération [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour créer une réunion.</span><span class="sxs-lookup"><span data-stu-id="36ffd-144">The following example shows the request XML when you use the [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a meeting.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Name="(UTC-08:00) Pacific Time (US &amp;amp; Canada)" Id="Pacific Standard Time">
        <t:Periods>
          <t:Period Bias="P0DT8H0M0.0S" Name="Standard" Id="Std" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/1" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/2007" />
        </t:Periods>
        <t:TransitionsGroups>
          <t:TransitionsGroup Id="0">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/1</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>4</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>10</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>-1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
          <t:TransitionsGroup Id="1">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/2007</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>3</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>2</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>11</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
        </t:TransitionsGroups>
        <t:Transitions>
          <t:Transition>
            <t:To Kind="Group">0</t:To>
          </t:Transition>
          <t:AbsoluteDateTransition>
            <t:To Kind="Group">1</t:To>
            <t:DateTime>2007-01-01T08:00:00.000Z</t:DateTime>
          </t:AbsoluteDateTransition>
        </t:Transitions>
      </t:TimeZoneDefinition>
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Weekly Update Meeting</t:Subject>
          <t:Body BodyType="HTML">Come hear about how the Organized Observational Paradigm SkyNet project is coming along!</t:Body>
          <t:ReminderMinutesBeforeStart>30</t:ReminderMinutesBeforeStart>
          <t:Start>2014-03-08T13:21:32.868-08:00</t:Start>
          <t:End>2014-03-08T14:21:32.868-08:00</t:End>
          <t:Location>Contoso Main Gallery</t:Location>
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
          <t:Recurrence>
            <t:WeeklyRecurrence>
              <t:Interval>1</t:Interval>
              <t:DaysOfWeek>Saturday</t:DaysOfWeek>
            </t:WeeklyRecurrence>
            <t:NumberedRecurrence>
              <t:StartDate>2014-03-08-08:00</t:StartDate>
              <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
            </t:NumberedRecurrence>
          </t:Recurrence>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

 <span data-ttu-id="36ffd-145">L'exemple suivant présente le code XML de réponse renvoyé par l'opération **CreateItem**.</span><span class="sxs-lookup"><span data-stu-id="36ffd-145">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
<span data-ttu-id="36ffd-146">Les attributs **ItemId** et **ChangeKey** sont raccourcis pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="36ffd-146">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="893" MinorBuildNumber="10" 
                         Version="V2_10" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="36ffd-147">L’exemple suivant montre le code XML de demande généré lorsque vous utilisez l’opération [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) et l' **ItemId** pour la série que vous avez créée, et les propriétés de requête définies uniquement sur une forme de base périodique pour confirmer que l' **ItemId** renvoyé par le serveur lors de la création d’une série périodique est destiné à une forme de base périodique.</span><span class="sxs-lookup"><span data-stu-id="36ffd-147">The following example shows the request XML that is generated when you use the [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) operation and the **ItemId** for the series you created, and request properties only set on a recurring master to confirm that the **ItemId** returned by the server when creating a recurring series is for a recurring master.</span></span> 
  
<span data-ttu-id="36ffd-148">Les attributs **ItemId** et **ChangeKey** sont raccourcis pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="36ffd-148">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Recurrence" />
          <t:FieldURI FieldURI="calendar:FirstOccurrence" />
          <t:FieldURI FieldURI="calendar:LastOccurrence" />
          <t:FieldURI FieldURI="calendar:ModifiedOccurrences" />
          <t:FieldURI FieldURI="calendar:DeletedOccurrences" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>

```

 <span data-ttu-id="36ffd-149">L'exemple suivant présente le code XML de réponse renvoyé par l'opération **GetItem**.</span><span class="sxs-lookup"><span data-stu-id="36ffd-149">The following example shows the response XML that is returned by the **GetItem** operation.</span></span> 
  
<span data-ttu-id="36ffd-150">Les attributs **ItemId** et **ChangeKey** sont raccourcis pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="36ffd-150">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="893" MinorBuildNumber="10" 
                         Version="V2_10" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAD" ChangeKey="DwAAAB" />
              <t:Subject>Weekly Update Meeting</t:Subject>
              <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              <t:Recurrence>
                <t:WeeklyRecurrence>
                  <t:Interval>1</t:Interval>
                  <t:DaysOfWeek>Saturday</t:DaysOfWeek>
                </t:WeeklyRecurrence>
                <t:NumberedRecurrence>
                  <t:StartDate>2014-03-08-08:00</t:StartDate>
                  <t:NumberOfOccurrences>10</t:NumberOfOccurrences>
                </t:NumberedRecurrence>
              </t:Recurrence>
              <t:FirstOccurrence>
                <t:ItemId Id="AAMkAD" ChangeKey="DwAAABY" />
                <t:Start>2014-03-08T21:21:00Z</t:Start>
                <t:End>2014-03-08T22:21:00Z</t:End>
                <t:OriginalStart>2014-03-08T21:21:00Z</t:OriginalStart>
              </t:FirstOccurrence>
              <t:LastOccurrence>
                <t:ItemId Id="AAMkAD" ChangeKey="DwAAABY" />
                <t:Start>2014-05-10T20:21:00Z</t:Start>
                <t:End>2014-05-10T21:21:00Z</t:End>
                <t:OriginalStart>2014-05-10T20:21:00Z</t:OriginalStart>
              </t:LastOccurrence>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="36ffd-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="36ffd-151">See also</span></span>


- [<span data-ttu-id="36ffd-152">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="36ffd-152">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="36ffd-153">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="36ffd-153">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="36ffd-154">Périodicités et EWS</span><span class="sxs-lookup"><span data-stu-id="36ffd-154">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="36ffd-155">Accéder à une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="36ffd-155">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="36ffd-156">Supprimer des rendez-vous dans une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="36ffd-156">Delete appointments in a recurring series by using EWS in Exchange</span></span>](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="36ffd-157">Mettre à jour une série périodique à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="36ffd-157">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="36ffd-158">Mettre à jour une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="36ffd-158">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    

