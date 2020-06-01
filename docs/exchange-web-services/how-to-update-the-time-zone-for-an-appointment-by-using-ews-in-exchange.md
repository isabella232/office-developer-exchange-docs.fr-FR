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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455841"
---
# <a name="update-the-time-zone-for-an-appointment-by-using-ews-in-exchange"></a>Mettre à jour le fuseau horaire pour un rendez-vous à l’aide d’EWS dans Exchange

Découvrez comment mettre à jour le fuseau horaire d’un rendez-vous ou d’une réunion existant à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
Lorsqu’un rendez-vous ou une réunion est créé dans un calendrier Exchange, le fuseau horaire utilisé pour spécifier les heures de début et de fin est enregistré comme fuseau horaire de création pour le rendez-vous. Vous pouvez modifier ce fuseau horaire à l’aide de l’API managée EWS ou d’EWS. Toutefois, la modification du fuseau horaire sur un rendez-vous a d’autres effets sur l’heure de début et de fin du rendez-vous.
  
Les valeurs d’heure sont stockées sur le serveur Exchange en temps universel coordonné (UTC). Par conséquent, si un rendez-vous est défini pour commencer à 1:00 (13:00) dans le fuseau horaire est (UTC-05:00), cette valeur est stockée en tant que 6:00 (18:00) sur le serveur, en supposant que le fuseau horaire est en phase standard. Lorsque ce rendez-vous est affiché dans d’autres fuseaux horaires, le nombre d’heures approprié est ajouté ou soustrait de la valeur UTC pour déterminer le temps spécifique au fuseau horaire. Par exemple, si un rendez-vous a une heure de début au 1:00 PM (6:00 PM UTC) et qu’il est affiché à partir d’un client dans le fuseau horaire Pacifique (UTC-08:00), l’heure de début spécifique à la zone horaire de ce client serait de 10:00 AM (18:00-08:00).
  
Lorsque vous mettez à jour le fuseau horaire du rendez-vous sans mettre à jour l’heure de début et de fin, le serveur met à jour les valeurs UTC stockées sur le serveur pour conserver l’heure de début et de fin en fonction des mêmes fuseaux horaires. Par exemple, prenons le rendez-vous 1:00 PM. L’heure est stockée en tant que 18:00 UTC sur le serveur. Si le fuseau horaire du rendez-vous est remplacé par le fuseau horaire Pacifique, le serveur passe l’heure de début au 1:00 PM (21:00 UTC).
  
Vous pouvez modifier ce comportement en définissant explicitement les heures de début et de fin.
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-the-ews-managed-api"></a>Mise à jour du fuseau horaire sur un rendez-vous existant à l’aide de l’API managée EWS

Dans l’exemple suivant, l’API managée EWS est utilisée pour mettre à jour le fuseau horaire d’un rendez-vous existant vers le fuseau horaire central en mettant à jour les propriétés appointment **. StartTimeZone** et appointment **. EndTimeZone** . Si le paramètre _shiftAppointnment_ est défini sur **true**, le code ne définit pas explicitement les heures de début et de fin sur le rendez-vous. Dans ce cas, le serveur déplace les heures de début et de fin afin de les conserver en même temps que les heures relatives dans le nouveau fuseau horaire. Si la valeur est **false**, le code convertit les heures de début et de fin de manière explicite afin de conserver simultanément le rendez-vous en UTC. 

Cet exemple part du principe que l’objet **ExchangeService** a été initialisé avec des valeurs valides dans les [informations d’identification](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et les propriétés de l' [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . 
  
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

Lorsque l’exemple est utilisé pour mettre à jour un rendez-vous qui commence à 1:00 PM et se termine à 2:00 PM est, avec le paramètre _shiftAppointment_ défini sur true et la propriété [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) définie sur le fuseau horaire est, le résultat se présente comme suit. 
  
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

Lorsque l’exemple est utilisé pour mettre à jour le même rendez-vous avec le paramètre _shiftAppointment_ défini sur false et que la propriété **TimeZone** est de nouveau définie sur le fuseau horaire est, le résultat semble un peu différent. 
  
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

Notez que les heures de début et de fin n’ont pas changé. En effet, les heures sont interprétées dans le fuseau horaire est (car la propriété **TimeZone** est définie sur le fuseau horaire est) et les valeurs d’heure ont été mises à jour pour empêcher le changement de rendez-vous. 
  
## <a name="updating-the-time-zone-on-an-existing-appointment-by-using-ews"></a>Mise à jour du fuseau horaire sur un rendez-vous existant à l’aide d’EWS

L’exemple de demande d' [opération UPDATEITEM](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS met à jour le fuseau horaire sur un rendez-vous. Cet exemple ne met pas à jour les éléments [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) , de sorte que le serveur déplace les heures de début et de fin du rendez-vous de façon à ce qu’il soit conservé en même temps dans le nouveau fuseau horaire. La valeur de l’élément **ItemId** est raccourcie pour des raisons de lisibilité. 
  
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

L’exemple de requête suivant met à jour le fuseau horaire du rendez-vous et met à jour les heures de début et de fin en définissant explicitement les éléments de **début** et de **fin** . La valeur de l’élément **ItemId** est raccourcie pour des raisons de lisibilité. 
  
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

## <a name="see-also"></a>Voir aussi

- [Fuseaux horaires et EWS dans Exchange](time-zones-and-ews-in-exchange.md)   
- [Créer des rendez-vous dans un fuseau horaire spécifique à l’aide d’EWS dans Exchange](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)   
- [Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    

