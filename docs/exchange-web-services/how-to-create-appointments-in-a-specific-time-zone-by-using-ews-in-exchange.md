---
title: Créer des rendez-vous dans un fuseau horaire spécifique à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e68aaa27-250e-4170-b099-077a979c127c
description: Découvrez comment créer des rendez-vous dans des fuseaux horaires spécifiques à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 1725498847f89a417b62a06fb8a3109af5c4deb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754825"
---
# <a name="create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange"></a><span data-ttu-id="5aa90-103">Créer des rendez-vous dans un fuseau horaire spécifique à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5aa90-103">Create appointments in a specific time zone by using EWS in Exchange</span></span>

<span data-ttu-id="5aa90-104">Découvrez comment créer des rendez-vous dans des fuseaux horaires spécifiques à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="5aa90-104">Learn how to create appointments in specific time zones by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="5aa90-105">Création d’un rendez-vous ou une réunion dans un calendrier Exchange, le fuseau horaire permet de spécifier les heures de début et de fin est enregistré en tant que le fuseau horaire de création pour le rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="5aa90-105">When an appointment or meeting is created on an Exchange calendar, the time zone used to specify the start and end times is saved as the creation time zone for the appointment.</span></span> <span data-ttu-id="5aa90-106">Ce fuseau horaire est également utilisé pour [interpréter les valeurs de date et heure qui n’ont pas un indication de fuseau horaire explicit](time-zones-and-ews-in-exchange.md), il est important de comprendre les options pour spécifier le fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="5aa90-106">That time zone is also used to [interpret date and time values that do not have an explicit time zone specified](time-zones-and-ews-in-exchange.md), so it is important to understand your options to specify the time zone.</span></span>
  
## <a name="creating-appointments-in-different-time-zones-by-using-the-ews-managed-api"></a><span data-ttu-id="5aa90-107">Création de rendez-vous dans différents fuseaux horaires à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="5aa90-107">Creating appointments in different time zones by using the EWS Managed API</span></span>

<span data-ttu-id="5aa90-108">Lorsque vous créez des rendez-vous ou des réunions à l’aide de l’API managée EWS, vous disposez de trois options pour spécifier le fuseau horaire :</span><span class="sxs-lookup"><span data-stu-id="5aa90-108">When creating appointments or meetings using the EWS Managed API, you have three options for specifying the time zone:</span></span>
  
- <span data-ttu-id="5aa90-109">Pour utiliser le fuseau horaire de l’ordinateur où s’exécute votre API managées, ne spécifiez pas un fuseau horaire lors de la création de l’objet [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5aa90-109">To use the time zone of the computer where your EWS Managed API is executing, do not specify a time zone when creating the [ExchangeService](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object.</span></span> 
    
- <span data-ttu-id="5aa90-110">Pour utiliser un fuseau horaire spécifique pour toutes les propriétés de date/heure, y compris les propriétés lors de la création d’un nouveau rendez-vous ou une réunion, spécifiez un fuseau horaire dans le constructeur de l’objet **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="5aa90-110">To use a specific time zone for all date/time properties, including properties when creating a new appointment or meeting, specify a time zone in the constructor for the **ExchangeService** object.</span></span> 
    
- <span data-ttu-id="5aa90-111">Pour utiliser un fuseau horaire différent de celui spécifié dans la propriété [ExchangeService.TimeZone](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) , utilisez les propriétés [Appointment.StartTimeZone](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) et [Appointment.EndTimeZone](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5aa90-111">To use a different time zone than the one specified in the [ExchangeService.TimeZone](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property, use the [Appointment.StartTimeZone](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) and [Appointment.EndTimeZone](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) properties.</span></span> 
    
    > [!NOTE]
    > <span data-ttu-id="5aa90-112">La propriété **EndTimeZone** est disponible uniquement lorsque la propriété [ExchangeService.RequestedServerVersion](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) est définie sur **Exchange2010** ou version ultérieure.</span><span class="sxs-lookup"><span data-stu-id="5aa90-112">The **EndTimeZone** property is only available when the [ExchangeService.RequestedServerVersion](http://msdn.microsoft.com/fr-fr/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) property is set to **Exchange2010** or later.</span></span> <span data-ttu-id="5aa90-113">S’il n’est pas disponible, définition **StartTimeZone** s’applique aux heures de début et de fin du rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="5aa90-113">If it is not available, setting the **StartTimeZone** applies to both the start and end times of the appointment.</span></span> 
  
<span data-ttu-id="5aa90-114">Dans l’exemple suivant, l’API managée EWS est utilisée pour créer des trois rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="5aa90-114">In the following example, the EWS Managed API is used to create three appointments.</span></span> <span data-ttu-id="5aa90-115">Chaque rendez-vous est configuré pour démarrer à 1 h 00 deux jours à partir de maintenant, dans un fuseau horaire non spécifié et de fin, une heure plus tard.</span><span class="sxs-lookup"><span data-stu-id="5aa90-115">Each appointment is set to start at 1:00 PM two days from now, in an unspecified time zone, and end one hour later.</span></span> <span data-ttu-id="5aa90-116">Le premier rendez-vous est créé dans le fuseau horaire de l’ordinateur client à l’aide de comportement d’API managées par défaut.</span><span class="sxs-lookup"><span data-stu-id="5aa90-116">The first appointment is created in the client computer's time zone by using default EWS Managed API behavior.</span></span> <span data-ttu-id="5aa90-117">Le second est créé dans le fuseau horaire Central en utilisant les propriétés **Appointment.StartTimeZone** et **Appointment.EndTimeZone** .</span><span class="sxs-lookup"><span data-stu-id="5aa90-117">The second is created in the Central time zone by using the **Appointment.StartTimeZone** and **Appointment.EndTimeZone** properties.</span></span> <span data-ttu-id="5aa90-118">La troisième est créée dans Paris à l’aide de la propriété **ExchangeService.TimeZone** .</span><span class="sxs-lookup"><span data-stu-id="5aa90-118">The third is created in the Mountain time zone by using the **ExchangeService.TimeZone** property.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
using System.Security;
static void CreateAppointments(string userEmail, SecureString userPass)
{
    // *****************************************************
    // Create an appointment using the client computer's time zone.
    // *****************************************************
    // Do not specify a time zone when creating the ExchangeService.
    ExchangeService clientTZService = new ExchangeService(ExchangeVersion.Exchange2010);
    clientTZService.Credentials = new NetworkCredential(userEmail, userPass);
    clientTZService.AutodiscoverUrl(userEmail, redirectionCallback);
    // Create the appointment.
    Appointment clientTZAppt = new Appointment(clientTZService);
    clientTZAppt.Subject = "Appointment created using client time zone";
    clientTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", clientTZService.TimeZone.DisplayName));
    // Set the start time to 1:00 PM two days from today.
    DateTime startTime = new DateTime(DateTime.Now.Year, DateTime.Now.Month, DateTime.Now.Day + 2);
    startTime = startTime.AddHours(13);
    clientTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    DateTime endTime = startTime.AddHours(1);
    clientTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        clientTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
    // *****************************************************
    // Create an appointment in the Central time zone by
    // using the StartTimeZone property.
    // *****************************************************
    // Retrieve the Central time zone.
    TimeZoneInfo centralTZ = TimeZoneInfo.FindSystemTimeZoneById("Central Standard Time");
    // Create the appointment.
    Appointment centralTZAppt = new Appointment(clientTZService);
    centralTZAppt.Subject = "Appointment created using Central time zone";
    centralTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", centralTZ.DisplayName));
    // Set the time zone on the appointment.
    centralTZAppt.StartTimeZone = centralTZ;
    centralTZAppt.EndTimeZone = centralTZ;
    // Set the start time to 1:00 PM two days from today.
    centralTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    centralTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        centralTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
    // *****************************************************
    // Create an appointment in the Mountain time zone by
    // using the ExchangeService.TimeZone property.
    // *****************************************************
    // Specify the Mountain time zone when creating the ExchangeService.
    TimeZoneInfo mountainTZ = TimeZoneInfo.FindSystemTimeZoneById("Mountain Standard Time");
    ExchangeService mountainTZService = new ExchangeService(ExchangeVersion.Exchange2010, mountainTZ);
    mountainTZService.Credentials = new NetworkCredential(userEmail, userPass);
    mountainTZService.AutodiscoverUrl(userEmail, redirectionCallback);
    // Create the appointment.
    Appointment mountainTZAppt = new Appointment(mountainTZService);
    mountainTZAppt.Subject = "Appointment created using Mountain time zone";
    mountainTZAppt.Body = new MessageBody(string.Format("Time zone: {0}", mountainTZService.TimeZone.DisplayName));
    // Set the start time to 1:00 PM two days from today.
    mountainTZAppt.Start = startTime;
    // Set the end time to 2:00 PM on that same day.
    mountainTZAppt.End = endTime;
    // Save the appointment to the default calendar.
    try
    {
        // This method results in a call to EWS.
        mountainTZAppt.Save(SendInvitationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error saving appointment: {0}", ex.Message);
    }
}
```

<span data-ttu-id="5aa90-119">Lorsque cet exemple est exécuté sur un ordinateur client configuré dans le fuseau horaire, et il crée trois rendez-vous sont affichés à partir d’un client configuré dans le fuseau horaire, ils apparaissent à 1:00 PM, 2 h 00 et 3 h 00, respectivement.</span><span class="sxs-lookup"><span data-stu-id="5aa90-119">When this example is executed on a client computer configured in the Eastern time zone, and the three appointments it creates are viewed from a client configured in the Eastern time zone, they appear at 1:00 PM, 2:00 PM, and 3:00 PM, respectively.</span></span>
  
## <a name="creating-appointments-in-different-time-zones-by-using-ews"></a><span data-ttu-id="5aa90-120">Création de rendez-vous dans différents fuseaux horaires à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="5aa90-120">Creating appointments in different time zones by using EWS</span></span>

<span data-ttu-id="5aa90-121">Lorsque vous créez des rendez-vous ou des réunions à l’aide de EWS, vous disposez de trois options pour spécifier le fuseau horaire :</span><span class="sxs-lookup"><span data-stu-id="5aa90-121">When creating appointments or meetings using EWS, you have three options for specifying the time zone:</span></span>
  
- <span data-ttu-id="5aa90-122">Pour utiliser le temps universel coordonné (UTC), ne pas inclure un élément [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) , élément (Exchange 2007 uniquement), ou [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et éléments [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (Exchange 2010 et versions ultérieur) dans le [ Opération CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) demande.</span><span class="sxs-lookup"><span data-stu-id="5aa90-122">To use Coordinated Universal Time (UTC), do not include a [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element, [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) element (Exchange 2007 only), or [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) and [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) elements (Exchange 2010 and later) in the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request.</span></span> 
    
- <span data-ttu-id="5aa90-123">Pour utiliser un fuseau horaire spécifique pour toutes les propriétés de date/heure, y compris les propriétés lors de la création d’un nouveau rendez-vous ou une réunion, spécifiez un fuseau horaire dans l’élément [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) dans la requête [d’opération CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5aa90-123">To use a specific time zone for all date/time properties, including properties when creating a new appointment or meeting, specify a time zone in the [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element in the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request.</span></span> 
    
- <span data-ttu-id="5aa90-124">Pour utiliser un fuseau horaire différent de celui spécifié dans l’élément [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , incluez un élément [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) , élément (Exchange 2007 uniquement) ou (éléments) [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) Exchange 2010 et versions ultérieur) dans la requête [d’opération CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="5aa90-124">To use a different time zone than the one specified in the [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element, include a [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) element, [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) element (Exchange 2007 only), or [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) and [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) elements (Exchange 2010 and later) in the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request.</span></span> 
    
<span data-ttu-id="5aa90-125">L’exemple de requête [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) suivant crée un rendez-vous à l’aide au format UTC.</span><span class="sxs-lookup"><span data-stu-id="5aa90-125">The following example [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request creates an appointment using UTC.</span></span> <span data-ttu-id="5aa90-126">Notez que l’élément **TimeZoneContext** , l’élément **StartTimeZone** et l’élément **EndTimeZone** sont absents.</span><span class="sxs-lookup"><span data-stu-id="5aa90-126">Notice that the **TimeZoneContext** element, the **StartTimeZone** element, and the **EndTimeZone** element are absent.</span></span> <span data-ttu-id="5aa90-127">Les valeurs d’élément **Start** et **End** sont exprimés au format UTC.</span><span class="sxs-lookup"><span data-stu-id="5aa90-127">The **Start** and **End** element values are expressed in UTC.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using UTC</t:Subject>
          <t:Body BodyType="HTML">Time zone: UTC</t:Body>
          <t:Start>2014-06-07T17:00:00.000Z</t:Start>
          <t:End>2014-06-07T18:00:00.000Z</t:End>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="5aa90-128">L’exemple de requête [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) suivant utilise les éléments **StartTimeZone** et **EndTimeZone** pour spécifier le fuseau horaire Central pour le rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="5aa90-128">The following example [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request uses the **StartTimeZone** and **EndTimeZone** elements to specify the Central time zone for the appointment.</span></span> <span data-ttu-id="5aa90-129">Notez que l’élément **TimeZoneContext** est absent.</span><span class="sxs-lookup"><span data-stu-id="5aa90-129">Notice that the **TimeZoneContext** element is absent.</span></span> <span data-ttu-id="5aa90-130">Toutefois, s’il s’agissait il est présent, les valeurs des éléments **StartTimeZone** et **EndTimeZone** seraient remplacer sa valeur.</span><span class="sxs-lookup"><span data-stu-id="5aa90-130">However, if it were present, the values of the **StartTimeZone** and **EndTimeZone** elements would override its value.</span></span> <span data-ttu-id="5aa90-131">Encore une fois, les valeurs d’élément **Start** et **End** sont exprimés au format UTC.</span><span class="sxs-lookup"><span data-stu-id="5aa90-131">Again, the **Start** and **End** element values are expressed in UTC.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using Central time zone</t:Subject>
          <t:Body BodyType="HTML">Time zone: (UTC-06:00) Central Time (US &amp;amp; Canada)</t:Body>
          <t:Start>2014-06-07T18:00:00.000Z</t:Start>
          <t:End>2014-06-07T19:00:00.000Z</t:End>
          <t:StartTimeZone Id="Central Standard Time" />
          <t:EndTimeZone Id="Central Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="5aa90-132">L’exemple de requête [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) suivant définit l’élément **TimeZoneContext** Paris.</span><span class="sxs-lookup"><span data-stu-id="5aa90-132">The following example [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) request sets the **TimeZoneContext** element to the Mountain time zone.</span></span> <span data-ttu-id="5aa90-133">Notez que les éléments **StartTimeZone** et **EndTimeZone** absents.</span><span class="sxs-lookup"><span data-stu-id="5aa90-133">Notice that the **StartTimeZone** and **EndTimeZone** elements are absent.</span></span> <span data-ttu-id="5aa90-134">Encore une fois, les valeurs d’élément **Start** et **End** sont exprimés au format UTC.</span><span class="sxs-lookup"><span data-stu-id="5aa90-134">Again, the **Start** and **End** element values are expressed in UTC.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Mountain Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Appointment created using Mountain time zone</t:Subject>
          <t:Body BodyType="HTML">Time zone: (UTC-07:00) Mountain Time (US &amp;amp; Canada)</t:Body>
          <t:Start>2014-06-07T19:00:00.000Z</t:Start>
          <t:End>2014-06-07T20:00:00.000Z</t:End>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="5aa90-135">Lorsque les trois rendez-vous créés par les demandes d’exemple EWS précédentes sont affichés à partir d’un client configuré dans le fuseau horaire, elles apparaissent à 13 h 00, 2 h 00 et 3 h 00, respectivement.</span><span class="sxs-lookup"><span data-stu-id="5aa90-135">When the three appointments created by the previous EWS example requests are viewed from a client configured in the Eastern time zone, they appear at 1:00 PM, 2:00 PM, and 3:00 PM, respectively.</span></span>
  
## 

<span data-ttu-id="5aa90-136">Maintenant que vous savez comment créer un rendez-vous dans des fuseaux horaires spécifiques, vous souhaiterez [mettre à jour les fuseaux horaires dans les rendez-vous existants](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md) vers un autre.</span><span class="sxs-lookup"><span data-stu-id="5aa90-136">Now that you know how to create appointments in specific time zones, you might want to [update the time zones on existing appointments](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md) to a different one.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5aa90-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5aa90-137">See also</span></span>


- [<span data-ttu-id="5aa90-138">Fuseaux horaires et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5aa90-138">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)
    
- [<span data-ttu-id="5aa90-139">Mettre à jour le fuseau horaire pour un rendez-vous à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5aa90-139">Update the time zone for an appointment by using EWS in Exchange</span></span>](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="5aa90-140">Créer des rendez-vous et réunions à l’aide de EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="5aa90-140">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    

