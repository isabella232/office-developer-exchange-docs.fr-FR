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
# <a name="update-the-time-zone-for-an-appointment-by-using-ews-in-exchange"></a>Mettre à jour le fuseau horaire pour un rendez-vous à l’aide de EWS dans Exchange

Découvrez comment mettre à jour le fuseau horaire pour un rendez-vous ou une réunion existante à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Création d’un rendez-vous ou une réunion dans un calendrier Exchange, le fuseau horaire permet de spécifier les heures de début et de fin est enregistré en tant que le fuseau horaire de création pour le rendez-vous. Vous pouvez modifier ce fuseau horaire à l’aide de l’API managée EWS ou EWS. Toutefois, la modification du fuseau horaire d’un rendez-vous a autres effets de l’heure de début et de fin du rendez-vous.
  
Valeurs d’heure sont stockés sur le serveur Exchange en coordonner le temps universel (UTC). Par conséquent, si un rendez-vous est configuré pour démarrer à 13 h 00 (13:00) dans le fuseau horaire (UTC-05:00), que la valeur est stockée en tant que 6 h 00 (18:00) sur le serveur, en supposant que le fuseau horaire est dans sa phase d’heure standard. Lorsque ce rendez-vous est affiché dans les autres fuseaux horaires, le nombre d’heures approprié est ajouté ou soustraite de la valeur UTC pour déterminer le temps de fuseau horaire spécifique. Par exemple, si un rendez-vous a une heure de début à 1 h 00 orientale (18 h 00 UTC) et est affiché à partir d’un client dans le fuseau horaire Pacifique (UTC-08:00), heure de début du fuseau horaire spécifiques pour que le client serait 10:00:00 (18:00-08:00).
  
Lorsque vous mettez à jour le fuseau horaire du rendez-vous sans mise à jour de l’heure de début et de fin, le serveur met à jour les valeurs d’heure UTC stockés sur le serveur pour conserver l’heure de début et de fin en tant que le temps de fuseau horaire spécifiques. Par exemple, considérez le rendez-vous est 1 h 00. L’heure est stockée en tant que 18 h 00 UTC sur le serveur. Si le fuseau horaire du rendez-vous est modifié pour le fuseau horaire Pacifique, le serveur décale l’heure de début à 1 h 00 PST (21 h 00 UTC).
  
Vous pouvez modifier ce comportement en définissant explicitement les heures de début et de fin.
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-the-ews-managed-api"></a>Mise à jour le fuseau horaire sur un rendez-vous existant à l’aide de l’API managée EWS

Dans l’exemple suivant, l’API managée EWS est utilisée pour mettre à jour le fuseau horaire sur un rendez-vous existant pour le fuseau horaire Central en mettant à jour les propriétés de **Appointment.EndTimeZone** et de **Appointment.StartTimeZone** . Si le paramètre _shiftAppointnment_ est défini sur **true**, le code ne définit pas explicitement les heures de début et de fin du rendez-vous. Dans ce cas, le serveur place les heures de début et de fin pour les conserver au même moment relative du fuseau horaire dans le nouveau fuseau horaire. Si la valeur **false**, le code convertit les heures de début et de fin explicitement pour conserver le rendez-vous en même temps au format UTC. 

Cet exemple suppose que l’objet **ExchangeService** a été initialisée avec des valeurs valides dans les propriétés [d’Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) et les [informations d’identification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) . 
  
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

Lorsque l’exemple est utilisé pour mettre à jour un rendez-vous qui commence à 1 h 00 est et se termine à 2 h 00 orientale, avec le paramètre _shiftAppointment_ défini sur true et la propriété [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) définie sur le fuseau horaire est, les résultats doivent ressembler comme suit. 
  
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

Lorsque l’exemple est utilisé pour mettre à jour le même rendez-vous avec le paramètre _shiftAppointment_ défini sur false et la propriété de **fuseau horaire** à nouveau définie sur le fuseau horaire est, la sortie est légèrement différente. 
  
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

Notez que les heures de début et de fin n’a pas changé. C’est parce que les heures sont en cours interprétés dans le fuseau horaire de la zone (car la propriété de **fuseau horaire** est définie sur le fuseau horaire est), et les valeurs d’heure ont été mis à jour pour empêcher le rendez-vous de décalage. 
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-ews"></a>Mise à jour le fuseau horaire sur un rendez-vous existant à l’aide de EWS

L’exemple de requête EWS [UpdateItem opération](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) suivant met à jour le fuseau horaire d’un rendez-vous. Cet exemple met à jour uniquement les éléments [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) , afin que le serveur place les heures de début et de fin du rendez-vous pour qu’il conserve relative de temps zone simultanément dans le nouveau fuseau horaire. La valeur de l’élément **ItemId** est raccourcie pour une meilleure lisibilité. 
  
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

L’exemple de requête suivant met à jour le fuseau horaire du rendez-vous et met également à jour les heures de début et de fin en définissant explicitement les éléments de **début** et de **fin** . La valeur de l’élément **ItemId** est raccourcie pour une meilleure lisibilité. 
  
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

## <a name="see-also"></a>Voir aussi

- [Fuseaux horaires et EWS dans Exchange](time-zones-and-ews-in-exchange.md)   
- [Créer des rendez-vous dans un fuseau horaire spécifique à l’aide de EWS dans Exchange](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)   
- [Mettre à jour vos rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    

