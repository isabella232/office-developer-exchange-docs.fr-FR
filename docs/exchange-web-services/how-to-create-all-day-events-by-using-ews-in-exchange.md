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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754815"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a>Créer des événements à l’aide de EWS dans Exchange

Découvrez comment créer des événements à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Événements sur une journée entière offrent un moyen pour représenter quelque chose qui se produit pour une journée entière ou plusieurs jours, par exemple, un jour férié ou des jours de congés. Création d’événements avec les API managées EWS est un composant logiciel enfichable. Il est tout comme la [Création de rendez-vous](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md), mais avec quelques modifications mineures.
  
## <a name="setting-start-and-end-times"></a>Définition des heures de début et de fin

Par définition, les événements d’une journée démarrent à minuit sur un jour spécifique et fin 24 heures (ou un multiple de 24 heures) ultérieurement. Toutefois, les API managées EWS permettent de spécifier le temps de minuit lors de la création de tous les événements du jour. Cela peut entraîner un comportement inattendu si vous n’êtes pas au courant de la façon dont ces heures obtient traduits sur le serveur.
  
Lorsqu’une demande est reçue pour créer un nouvel événement d’une journée entière avec non minuit (dans le [fuseau horaire de la demande ou un rendez-vous](time-zones-and-ews-in-exchange.md)) début et/ou à la fin des heures, les durées ajustées à minuit dans le fuseau horaire approprié en fonction des règles suivantes :
  
- Heures de début non-minuit sont ajustées le minuit avant l’heure spécifiée. Par exemple, 1:00 PM 6 juin est réglé à 12:00 AM 6 juin.
    
- Heure de fin non-minuit est ajustées le minuit après l’heure spécifiée. Par exemple, 1:00 PM 6 juin est réglé à 12:00 AM 7 juin.
    
Afin que vous créez la journée est toujours y compris l’heure de début et de fin que vous spécifiez, mais pouvez demander davantage de temps sur l’utilisateur du calendrier en raison du travail d’équipe à minuit. Car le serveur ajuste l’heure de début et de fin à minuit, nous vous recommandons de spécifier votre heure de début et de fin à minuit pour éviter toute modification accidentelle aux fois.
  
Il est également important de prendre en compte les fuseaux horaires lors de la création d’événements sur une journée entière. Étant donné que la version d’Exchange server impose une minuit début et heure de fin dans le fuseau horaire de la demande ou d’un rendez-vous, affichage de cet événement d’une journée entière dans un client configuré pour un fuseau horaire différent peut produire des résultats inattendus. Selon le client, il peut apparaître en tant que journée avec jours supplémentaires que vous n’êtes pas à inclure ou celui-ci n’apparaîtra pas entièrement en tant qu’un événement d’une journée entière. Pour cette raison, nous vous recommandons d’utiliser fuseau horaire préféré son la mesure du possible lorsque vous créez des événements d’une journée.
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a>Créer un événement à l’aide de l’API managée EWS

L’exemple suivant montre comment utiliser l’API managée EWS pour créer un événement d’une journée entière, commençant à la date spécifiée par le paramètre _startDate_ et une durée pour le nombre de jours spécifié par le paramètre _numDays_ . Notez que le rendez-vous sera créé dans le fuseau horaire spécifié par la propriété [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) . Cet exemple suppose que l’objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) transmis dans le paramètre de _service_ a été initialisé avec les valeurs valides pour les propriétés [d’Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) et les [informations d’identification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) . 
  
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

## <a name="create-an-all-day-event-by-using-ews"></a>Créer un événement à l’aide de EWS

L’exemple suivant montre une demande EWS [opération CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) pour créer un événement d’une journée entière. Le rendez-vous est créé dans le fuseau horaire, comme indiqué par l’élément [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) . Notez que la partie heure des valeurs des éléments [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) et [End](http://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) sont les deux 04:00Z, qui convertit à minuit dans le fuseau horaire lors de l’heure d’été. 
  
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

## <a name="see-also"></a>Voir aussi


- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
    
- [Créer des rendez-vous et réunions à l’aide de EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Fuseaux horaires et EWS dans Exchange](time-zones-and-ews-in-exchange.md)
    

