---
title: Mettre à jour le fuseau horaire pour un rendez-vous à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: dc2240c1-5500-4d5c-97d5-09d63ffd30d5
description: Découvrez comment mettre à jour le fuseau horaire d’un rendez-vous ou d’une réunion existant à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 064f99997b7c3d1197cb8d1ee6a24f8fb874f706
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455841"
---
# <a name="update-the-time-zone-for-an-appointment-by-using-ews-in-exchange"></a><span data-ttu-id="0f512-103">Mettre à jour le fuseau horaire pour un rendez-vous à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0f512-103">Update the time zone for an appointment by using EWS in Exchange</span></span>

<span data-ttu-id="0f512-104">Découvrez comment mettre à jour le fuseau horaire d’un rendez-vous ou d’une réunion existant à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f512-104">Learn how to update the time zone for an existing appointment or meeting by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="0f512-105">Lorsqu’un rendez-vous ou une réunion est créé dans un calendrier Exchange, le fuseau horaire utilisé pour spécifier les heures de début et de fin est enregistré comme fuseau horaire de création pour le rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="0f512-105">When an appointment or meeting is created on an Exchange calendar, the time zone used to specify the start and end times is saved as the creation time zone for the appointment.</span></span> <span data-ttu-id="0f512-106">Vous pouvez modifier ce fuseau horaire à l’aide de l’API managée EWS ou d’EWS.</span><span class="sxs-lookup"><span data-stu-id="0f512-106">You can change that time zone by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="0f512-107">Toutefois, la modification du fuseau horaire sur un rendez-vous a d’autres effets sur l’heure de début et de fin du rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="0f512-107">However, changing the time zone on an appointment has other effects on the start and end time of the appointment.</span></span>
  
<span data-ttu-id="0f512-108">Les valeurs d’heure sont stockées sur le serveur Exchange en temps universel coordonné (UTC).</span><span class="sxs-lookup"><span data-stu-id="0f512-108">Time values are stored on the Exchange server in Coordinate Universal Time (UTC).</span></span> <span data-ttu-id="0f512-109">Par conséquent, si un rendez-vous est défini pour commencer à 1:00 (13:00) dans le fuseau horaire est (UTC-05:00), cette valeur est stockée en tant que 6:00 (18:00) sur le serveur, en supposant que le fuseau horaire est en phase standard.</span><span class="sxs-lookup"><span data-stu-id="0f512-109">So if an appointment is set to start at 1:00 PM (13:00) in the Eastern time zone (UTC-05:00), that value is stored as 6:00 PM (18:00) on the server, assuming that the time zone is in its standard time phase.</span></span> <span data-ttu-id="0f512-110">Lorsque ce rendez-vous est affiché dans d’autres fuseaux horaires, le nombre d’heures approprié est ajouté ou soustrait de la valeur UTC pour déterminer le temps spécifique au fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="0f512-110">When that appointment is viewed in other time zones, the appropriate number of hours is added or subtracted from the UTC value to determine the time zone-specific time.</span></span> <span data-ttu-id="0f512-111">Par exemple, si un rendez-vous a une heure de début au 1:00 PM (6:00 PM UTC) et qu’il est affiché à partir d’un client dans le fuseau horaire Pacifique (UTC-08:00), l’heure de début spécifique à la zone horaire de ce client serait de 10:00 AM (18:00-08:00).</span><span class="sxs-lookup"><span data-stu-id="0f512-111">For example, if an appointment has a start time at 1:00 PM Eastern (6:00 PM UTC), and is viewed from a client in the Pacific time zone (UTC-08:00), the time-zone specific start time for that client would be 10:00 AM (18:00 - 08:00).</span></span>
  
<span data-ttu-id="0f512-112">Lorsque vous mettez à jour le fuseau horaire du rendez-vous sans mettre à jour l’heure de début et de fin, le serveur met à jour les valeurs UTC stockées sur le serveur pour conserver l’heure de début et de fin en fonction des mêmes fuseaux horaires.</span><span class="sxs-lookup"><span data-stu-id="0f512-112">When you update the time zone of the appointment without updating the start and end time, the server updates the UTC values stored on the server to keep the start and end time as the same time zone-specific times.</span></span> <span data-ttu-id="0f512-113">Par exemple, prenons le rendez-vous 1:00 PM.</span><span class="sxs-lookup"><span data-stu-id="0f512-113">For example, consider the 1:00 PM Eastern appointment.</span></span> <span data-ttu-id="0f512-114">L’heure est stockée en tant que 18:00 UTC sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="0f512-114">The time is stored as 18:00 UTC on the server.</span></span> <span data-ttu-id="0f512-115">Si le fuseau horaire du rendez-vous est remplacé par le fuseau horaire Pacifique, le serveur passe l’heure de début au 1:00 PM (21:00 UTC).</span><span class="sxs-lookup"><span data-stu-id="0f512-115">If the time zone of the appointment is changed to the Pacific time zone, the server shifts the start time to 1:00 PM Pacific (21:00 UTC).</span></span>
  
<span data-ttu-id="0f512-116">Vous pouvez modifier ce comportement en définissant explicitement les heures de début et de fin.</span><span class="sxs-lookup"><span data-stu-id="0f512-116">You can change this behavior by explicitly setting the start and end times.</span></span>
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="0f512-117">Mise à jour du fuseau horaire sur un rendez-vous existant à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="0f512-117">Updating the time zone on an existing appointment by using the EWS Managed API</span></span>

<span data-ttu-id="0f512-118">Dans l’exemple suivant, l’API managée EWS est utilisée pour mettre à jour le fuseau horaire d’un rendez-vous existant vers le fuseau horaire central en mettant à jour les propriétés appointment **. StartTimeZone** et appointment **. EndTimeZone** .</span><span class="sxs-lookup"><span data-stu-id="0f512-118">In the following example, the EWS Managed API is used to update the time zone on an existing appointment to the Central time zone by updating the **Appointment.StartTimeZone** and **Appointment.EndTimeZone** properties.</span></span> <span data-ttu-id="0f512-119">Si le paramètre _shiftAppointnment_ est défini sur **true**, le code ne définit pas explicitement les heures de début et de fin sur le rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="0f512-119">If the  _shiftAppointnment_ parameter is set to **true**, the code does not explicitly set the start and end times on the appointment.</span></span> <span data-ttu-id="0f512-120">Dans ce cas, le serveur déplace les heures de début et de fin afin de les conserver en même temps que les heures relatives dans le nouveau fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="0f512-120">In this case, the server will shift the start and end times to keep them at the same time zone-relative times in the new time zone.</span></span> <span data-ttu-id="0f512-121">Si la valeur est **false**, le code convertit les heures de début et de fin de manière explicite afin de conserver simultanément le rendez-vous en UTC.</span><span class="sxs-lookup"><span data-stu-id="0f512-121">If set to **false**, the code converts the start and end times explicitly to keep the appointment at the same time in UTC.</span></span> 

<span data-ttu-id="0f512-122">Cet exemple part du principe que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les [informations d’identification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et les propriétés de l' [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0f512-122">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

<span data-ttu-id="0f512-123">Lorsque l’exemple est utilisé pour mettre à jour un rendez-vous qui commence à 1:00 PM et se termine à 2:00 PM est, avec le paramètre _shiftAppointment_ défini sur true et la propriété [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) définie sur le fuseau horaire est, le résultat se présente comme suit.</span><span class="sxs-lookup"><span data-stu-id="0f512-123">When the example is used to update an appointment that starts at 1:00 PM Eastern and ends at 2:00 PM Eastern, with the  _shiftAppointment_ parameter set to true, and the [ExchangeService.TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) property set to the Eastern time zone, the output looks like the following.</span></span> 
  
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

<span data-ttu-id="0f512-124">Lorsque l’exemple est utilisé pour mettre à jour le même rendez-vous avec le paramètre _shiftAppointment_ défini sur false et que la propriété **TimeZone** est de nouveau définie sur le fuseau horaire est, le résultat semble un peu différent.</span><span class="sxs-lookup"><span data-stu-id="0f512-124">When the example is used to update the same appointment with the  _shiftAppointment_ parameter set to false, and with the **TimeZone** property again set to the Eastern time zone, the output looks a little different.</span></span> 
  
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

<span data-ttu-id="0f512-125">Notez que les heures de début et de fin n’ont pas changé.</span><span class="sxs-lookup"><span data-stu-id="0f512-125">Notice that the start and end times did not change.</span></span> <span data-ttu-id="0f512-126">En effet, les heures sont interprétées dans le fuseau horaire est (car la propriété **TimeZone** est définie sur le fuseau horaire est) et les valeurs d’heure ont été mises à jour pour empêcher le changement de rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="0f512-126">This is because the times are being interpreted in the Eastern time zone (because the **TimeZone** property is set to the Eastern time zone), and the time values were updated to prevent the appointment from shifting.</span></span> 
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-ews"></a><span data-ttu-id="0f512-127">Mise à jour du fuseau horaire sur un rendez-vous existant à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="0f512-127">Updating the time zone on an existing appointment by using EWS</span></span>

<span data-ttu-id="0f512-128">L’exemple de demande d' [opération UPDATEITEM](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS met à jour le fuseau horaire sur un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="0f512-128">The following example EWS [UpdateItem operation](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) request updates the time zone on an appointment.</span></span> <span data-ttu-id="0f512-129">Cet exemple ne met pas à jour les éléments [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) , de sorte que le serveur déplace les heures de début et de fin du rendez-vous de façon à ce qu’il soit conservé en même temps dans le nouveau fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="0f512-129">This example only updates the [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) and [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) elements, so the server will shift the start and end times of the appointment to keep it at the same time-zone-relative time in the new time zone.</span></span> <span data-ttu-id="0f512-130">La valeur de l’élément **ItemId** est raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="0f512-130">The value of the **ItemId** element is shortened for readability.</span></span> 
  
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

<span data-ttu-id="0f512-131">L’exemple de requête suivant met à jour le fuseau horaire du rendez-vous et met à jour les heures de début et de fin en définissant explicitement les éléments de **début** et de **fin** .</span><span class="sxs-lookup"><span data-stu-id="0f512-131">The following example request updates the time zone of the appointment, and also updates the start and end times by explicitly setting the **Start** and **End** elements.</span></span> <span data-ttu-id="0f512-132">La valeur de l’élément **ItemId** est raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="0f512-132">The value of the **ItemId** element is shortened for readability.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="0f512-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0f512-133">See also</span></span>

- [<span data-ttu-id="0f512-134">Fuseaux horaires et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0f512-134">Time zones and EWS in Exchange</span></span>](time-zones-and-ews-in-exchange.md)   
- [<span data-ttu-id="0f512-135">Créer des rendez-vous dans un fuseau horaire spécifique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0f512-135">Create appointments in a specific time zone by using EWS in Exchange</span></span>](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="0f512-136">Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0f512-136">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    

