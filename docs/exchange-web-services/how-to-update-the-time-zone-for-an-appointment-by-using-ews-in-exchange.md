---
title: Mettre à jour le fuseau horaire pour un rendez-vous à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: dc2240c1-5500-4d5c-97d5-09d63ffd30d5
description: Découvrez comment mettre à jour le fuseau horaire pour un rendez-vous ou une réunion existante à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 535eb9f546d9a4353408579f3a24750f32237699
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754952"
---
# <a name="update-the-time-zone-for-an-appointment-by-using-ews-in-exchange"></a><span data-ttu-id="757ed-103">Mettre à jour le fuseau horaire pour un rendez-vous à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="757ed-103">Update the time zone for an appointment by using EWS in Exchange</span></span>

<span data-ttu-id="757ed-104">Découvrez comment mettre à jour le fuseau horaire pour un rendez-vous ou une réunion existante à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="757ed-104">Learn how to update the time zone for an existing appointment or meeting by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="757ed-105">Création d’un rendez-vous ou une réunion dans un calendrier Exchange, le fuseau horaire permet de spécifier les heures de début et de fin est enregistré en tant que le fuseau horaire de création pour le rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="757ed-105">When an appointment or meeting is created on an Exchange calendar, the time zone used to specify the start and end times is saved as the creation time zone for the appointment.</span></span> <span data-ttu-id="757ed-106">Vous pouvez modifier ce fuseau horaire à l’aide de l’API managée EWS ou EWS.</span><span class="sxs-lookup"><span data-stu-id="757ed-106">You can change that time zone by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="757ed-107">Toutefois, la modification du fuseau horaire d’un rendez-vous a autres effets de l’heure de début et de fin du rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="757ed-107">However, changing the time zone on an appointment has other effects on the start and end time of the appointment.</span></span>
  
<span data-ttu-id="757ed-108">Valeurs d’heure sont stockés sur le serveur Exchange en coordonner le temps universel (UTC).</span><span class="sxs-lookup"><span data-stu-id="757ed-108">Time values are stored on the Exchange server in Coordinate Universal Time (UTC).</span></span> <span data-ttu-id="757ed-109">Par conséquent, si un rendez-vous est configuré pour démarrer à 13 h 00 (13:00) dans le fuseau horaire (UTC-05:00), que la valeur est stockée en tant que 6 h 00 (18:00) sur le serveur, en supposant que le fuseau horaire est dans sa phase d’heure standard.</span><span class="sxs-lookup"><span data-stu-id="757ed-109">So if an appointment is set to start at 1:00 PM (13:00) in the Eastern time zone (UTC-05:00), that value is stored as 6:00 PM (18:00) on the server, assuming that the time zone is in its standard time phase.</span></span> <span data-ttu-id="757ed-110">Lorsque ce rendez-vous est affiché dans les autres fuseaux horaires, le nombre d’heures approprié est ajouté ou soustraite de la valeur UTC pour déterminer le temps de fuseau horaire spécifique.</span><span class="sxs-lookup"><span data-stu-id="757ed-110">When that appointment is viewed in other time zones, the appropriate number of hours is added or subtracted from the UTC value to determine the time zone-specific time.</span></span> <span data-ttu-id="757ed-111">Par exemple, si un rendez-vous a une heure de début à 1 h 00 orientale (18 h 00 UTC) et est affiché à partir d’un client dans le fuseau horaire Pacifique (UTC-08:00), heure de début du fuseau horaire spécifiques pour que le client serait 10:00:00 (18:00-08:00).</span><span class="sxs-lookup"><span data-stu-id="757ed-111">For example, if an appointment has a start time at 1:00 PM Eastern (6:00 PM UTC), and is viewed from a client in the Pacific time zone (UTC-08:00), the time-zone specific start time for that client would be 10:00 AM (18:00 - 08:00).</span></span>
  
<span data-ttu-id="757ed-112">Lorsque vous mettez à jour le fuseau horaire du rendez-vous sans mise à jour de l’heure de début et de fin, le serveur met à jour les valeurs d’heure UTC stockés sur le serveur pour conserver l’heure de début et de fin en tant que le temps de fuseau horaire spécifiques.</span><span class="sxs-lookup"><span data-stu-id="757ed-112">When you update the time zone of the appointment without updating the start and end time, the server updates the UTC values stored on the server to keep the start and end time as the same time zone-specific times.</span></span> <span data-ttu-id="757ed-113">Par exemple, considérez le rendez-vous est 1 h 00.</span><span class="sxs-lookup"><span data-stu-id="757ed-113">For example, consider the 1:00 PM Eastern appointment.</span></span> <span data-ttu-id="757ed-114">L’heure est stockée en tant que 18 h 00 UTC sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="757ed-114">The time is stored as 18:00 UTC on the server.</span></span> <span data-ttu-id="757ed-115">Si le fuseau horaire du rendez-vous est modifié pour le fuseau horaire Pacifique, le serveur décale l’heure de début à 1 h 00 PST (21 h 00 UTC).</span><span class="sxs-lookup"><span data-stu-id="757ed-115">If the time zone of the appointment is changed to the Pacific time zone, the server shifts the start time to 1:00 PM Pacific (21:00 UTC).</span></span>
  
<span data-ttu-id="757ed-116">Vous pouvez modifier ce comportement en définissant explicitement les heures de début et de fin.</span><span class="sxs-lookup"><span data-stu-id="757ed-116">You can change this behavior by explicitly setting the start and end times.</span></span>
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="757ed-117">Mise à jour le fuseau horaire sur un rendez-vous existant à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="757ed-117">Updating the time zone on an existing appointment by using the EWS Managed API</span></span>

<span data-ttu-id="757ed-118">Dans l’exemple suivant, l’API managée EWS est utilisée pour mettre à jour le fuseau horaire sur un rendez-vous existant pour le fuseau horaire Central en mettant à jour les propriétés de **Appointment.EndTimeZone** et de **Appointment.StartTimeZone** .</span><span class="sxs-lookup"><span data-stu-id="757ed-118">In the following example, the EWS Managed API is used to update the time zone on an existing appointment to the Central time zone by updating the **Appointment.StartTimeZone** and **Appointment.EndTimeZone** properties.</span></span> <span data-ttu-id="757ed-119">Si le paramètre _shiftAppointnment_ est défini sur **true**, le code ne définit pas explicitement les heures de début et de fin du rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="757ed-119">If the  _shiftAppointnment_ parameter is set to **true**, the code does not explicitly set the start and end times on the appointment.</span></span> <span data-ttu-id="757ed-120">Dans ce cas, le serveur place les heures de début et de fin pour les conserver au même moment relative du fuseau horaire dans le nouveau fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="757ed-120">In this case, the server will shift the start and end times to keep them at the same time zone-relative times in the new time zone.</span></span> <span data-ttu-id="757ed-121">Si la valeur **false**, le code convertit les heures de début et de fin explicitement pour conserver le rendez-vous en même temps au format UTC.</span><span class="sxs-lookup"><span data-stu-id="757ed-121">If set to **false**, the code converts the start and end times explicitly to keep the appointment at the same time in UTC.</span></span> 

<span data-ttu-id="757ed-122">Cet exemple suppose que l’objet **ExchangeService** a été initialisée avec des valeurs valides dans les propriétés [d’Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) et les [informations d’identification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="757ed-122">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
static void UpdateAppointmentTimeZone(ExchangeService service, ItemId apptId, bool shiftAppointment)
{
    PropertySet includeTimeZones = new PropertySet(AppointmentSchema.Subject,
                                                   AppointmentSchema.Start,
                                                   AppointmentSchema.ReminderDueBy,
                                                   AppointmentSchema.End,
                                                   AppointmentSchema.StartTimeZone,
                                                   AppointmentSchema.EndTimeZone);
    Appointment apptToUpdate;
    // Load the existing appointment.
    // This will result in a call to EWS.
    try
    {
        apptToUpdate = Appointment.Bind(service, apptId, includeTimeZones);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error retrieving existing appointment: {0}", ex.Message);
        return;
    }
    Console.WriteLine("Before update:");
    // Output the current start, reminder, end, and time zones.
    Console.WriteLine("  Start: {0}", apptToUpdate.Start);
    Console.WriteLine("  Start time zone: {0}", apptToUpdate.StartTimeZone.DisplayName);
    Console.WriteLine("  Reminder: {0}", apptToUpdate.ReminderDueBy);
    Console.WriteLine("  End: {0}", apptToUpdate.End);
    Console.WriteLine("  End time zone: {0}", apptToUpdate.EndTimeZone.DisplayName);
    // Retrieve the Central time zone.
    TimeZoneInfo centralTZ = TimeZoneInfo.FindSystemTimeZoneById("Central Standard Time");
    // Update the time zones on the appointment.
    apptToUpdate.StartTimeZone = centralTZ;
    apptToUpdate.EndTimeZone = centralTZ;
    if (!shiftAppointment)
    {
        // Set the start and end times explicitly so that the appointment
        // will start and end at the same UTC time.
        // Convert the times to then Central time zone. This
        // will keep them at the same time in UTC.
        // For example, 1:00 PM Eastern becomes 12:00 PM Central.
        DateTime newStartTime = TimeZoneInfo.ConvertTime(
            apptToUpdate.Start, centralTZ);
        DateTime newEndTime = TimeZoneInfo.ConvertTime(
            apptToUpdate.End, centralTZ);
        apptToUpdate.Start = newStartTime;
        apptToUpdate.End = newEndTime;
    }
    try
    {
        // Save the changes. This will result in a call to EWS.
        apptToUpdate.Update(ConflictResolutionMode.AlwaysOverwrite, 
            SendInvitationsOrCancellationsMode.SendToNone);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error updating appointment: {0}", ex.Message);
        return;
    }
    // Now rebind to the appointment to get the new values.
    Appointment apptAfterUpdate;
    
    try
    {
        // This will result in a call to EWS.
        apptAfterUpdate = Appointment.Bind(service, apptId, includeTimeZones);
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error retrieving existing appointment: {0}", ex.Message);
        return;
    }
    Console.WriteLine("After update:");
    // Output the current start, reminder, end, and time zones.
    Console.WriteLine("  Start: {0}", apptAfterUpdate.Start);
    Console.WriteLine("  Start time zone: {0}", apptAfterUpdate.StartTimeZone.DisplayName);
    Console.WriteLine("  Reminder: {0}", apptAfterUpdate.ReminderDueBy);
    Console.WriteLine("  End: {0}", apptAfterUpdate.End);
    Console.WriteLine("  End time zone: {0}", apptAfterUpdate.EndTimeZone.DisplayName);
}
```

<span data-ttu-id="757ed-123">Lorsque l’exemple est utilisé pour mettre à jour un rendez-vous qui commence à 1 h 00 est et se termine à 2 h 00 orientale, avec le paramètre _shiftAppointment_ défini sur true et la propriété [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) définie sur le fuseau horaire est, les résultats doivent ressembler comme suit.</span><span class="sxs-lookup"><span data-stu-id="757ed-123">When the example is used to update an appointment that starts at 1:00 PM Eastern and ends at 2:00 PM Eastern, with the  _shiftAppointment_ parameter set to true, and the [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property set to the Eastern time zone, the output looks like the following.</span></span> 
  
```MS-DOS
Before update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
After update:
  Start: 6/20/2014 2:00:00 PM
  Start time zone: (UTC-06:00) Central Time (US &amp; Canada)
  Reminder: 6/20/2014 2:00:00 PM
  End: 6/20/2014 3:00:00 PM
  End time zone: (UTC-06:00) Central Time (US &amp; Canada)
```

<span data-ttu-id="757ed-124">Lorsque l’exemple est utilisé pour mettre à jour le même rendez-vous avec le paramètre _shiftAppointment_ défini sur false et la propriété de **fuseau horaire** à nouveau définie sur le fuseau horaire est, la sortie est légèrement différente.</span><span class="sxs-lookup"><span data-stu-id="757ed-124">When the example is used to update the same appointment with the  _shiftAppointment_ parameter set to false, and with the **TimeZone** property again set to the Eastern time zone, the output looks a little different.</span></span> 
  
```MS-DOS
Before update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-05:00) Eastern Time (US &amp; Canada)
After update:
  Start: 6/20/2014 1:00:00 PM
  Start time zone: (UTC-06:00) Central Time (US &amp; Canada)
  Reminder: 6/20/2014 1:00:00 PM
  End: 6/20/2014 2:00:00 PM
  End time zone: (UTC-06:00) Central Time (US &amp; Canada)
```

<span data-ttu-id="757ed-125">Notez que les heures de début et de fin n’a pas changé.</span><span class="sxs-lookup"><span data-stu-id="757ed-125">Notice that the start and end times did not change.</span></span> <span data-ttu-id="757ed-126">C’est parce que les heures sont en cours interprétés dans le fuseau horaire de la zone (car la propriété de **fuseau horaire** est définie sur le fuseau horaire est), et les valeurs d’heure ont été mis à jour pour empêcher le rendez-vous de décalage.</span><span class="sxs-lookup"><span data-stu-id="757ed-126">This is because the times are being interpreted in the Eastern time zone (because the **TimeZone** property is set to the Eastern time zone), and the time values were updated to prevent the appointment from shifting.</span></span> 
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-ews"></a><span data-ttu-id="757ed-127">Mise à jour le fuseau horaire sur un rendez-vous existant à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="757ed-127">Updating the time zone on an existing appointment by using EWS</span></span>

<span data-ttu-id="757ed-128">L’exemple de requête EWS [UpdateItem opération](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) suivant met à jour le fuseau horaire d’un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="757ed-128">The following example EWS [UpdateItem operation](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) request updates the time zone on an appointment.</span></span> <span data-ttu-id="757ed-129">Cet exemple met à jour uniquement les éléments [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) , afin que le serveur place les heures de début et de fin du rendez-vous pour qu’il conserve relative de temps zone simultanément dans le nouveau fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="757ed-129">This example only updates the [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) and [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) elements, so the server will shift the start and end times of the appointment to keep it at the same time-zone-relative time in the new time zone.</span></span> <span data-ttu-id="757ed-130">La valeur de l’élément **ItemId** est raccourcie pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="757ed-130">The value of the **ItemId** element is shortened for readability.</span></span> 
  
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
    <m:UpdateItem ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToNone">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:StartTimeZone" />
              <t:CalendarItem>
                <t:StartTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:EndTimeZone" />
              <t:CalendarItem>
                <t:EndTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="757ed-131">L’exemple de requête suivant met à jour le fuseau horaire du rendez-vous et met également à jour les heures de début et de fin en définissant explicitement les éléments de **début** et de **fin** .</span><span class="sxs-lookup"><span data-stu-id="757ed-131">The following example request updates the time zone of the appointment, and also updates the start and end times by explicitly setting the **Start** and **End** elements.</span></span> <span data-ttu-id="757ed-132">La valeur de l’élément **ItemId** est raccourcie pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="757ed-132">The value of the **ItemId** element is shortened for readability.</span></span> 
  
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
    <m:UpdateItem ConflictResolution="AlwaysOverwrite" SendMeetingInvitationsOrCancellations="SendToNone">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:StartTimeZone" />
              <t:CalendarItem>
                <t:StartTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:EndTimeZone" />
              <t:CalendarItem>
                <t:EndTimeZone Id="Central Standard Time" />
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:Start" />
              <t:CalendarItem>
                <t:Start>2014-06-20T17:00:00.000Z</t:Start>
              </t:CalendarItem>
            </t:SetItemField>
            <t:SetItemField>
              <t:FieldURI FieldURI="calendar:End" />
              <t:CalendarItem>
                <t:End>2014-06-20T18:00:00.000Z</t:End>
              </t:CalendarItem>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="757ed-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="757ed-133">See also</span></span>

- [<span data-ttu-id="757ed-134">Fuseaux horaires et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="757ed-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)   
- [<span data-ttu-id="757ed-135">Créer des rendez-vous dans un fuseau horaire spécifique à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="757ed-135">Create appointments in a specific time zone by using EWS in Exchange</span></span>](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="757ed-136">Mettre à jour vos rendez-vous et réunions à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="757ed-136">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    

