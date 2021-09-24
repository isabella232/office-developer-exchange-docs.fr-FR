---
title: Créer des événements sur une journée entière à l'aide d’EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 0fcb484b-4ffc-41a5-aeed-8c797766b70c
description: Découvrez comment créer des événements d’une journée à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 8769999907df46f519355a36fdf409f9ad347330
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521220"
---
# <a name="create-all-day-events-by-using-ews-in-exchange"></a>Créer des événements sur une journée entière à l'aide d’EWS dans Exchange

Découvrez comment créer des événements d’une journée à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
  
Les événements d’une journée entière permettent de représenter un événement qui se produit pendant une journée entière ou plusieurs jours( par exemple, des jours fériés ou des jours de vacances). La création d’événements d’une journée avec l’API gérée EWS ou EWS est un logiciel en un clin d’œil. C’est comme créer [des rendez-vous,](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)mais avec quelques petites modifications.
  
## <a name="setting-start-and-end-times"></a>Définition des heures de début et de fin

Par définition, les événements d’une journée commencent à minuit un jour spécifique et se terminent 24 heures (ou un multiple de 24 heures) plus tard. Toutefois, l’API gérée EWS et EWS vous permettent de spécifier des heures autres que minuit lors de la création d’événements d’une journée. Cela peut entraîner un comportement inattendu si vous ne savez pas comment ces heures sont traduites sur le serveur.
  
Lorsqu’une demande est reçue pour créer un événement d’une journée avec des heures de début et/ou de fin non-minuit (dans le fuseau horaire de la demande ou du rendez-vous), ces heures sont ajustées à minuit dans le fuseau horaire approprié en fonction des règles suivantes : [](time-zones-and-ews-in-exchange.md)
  
- Les heures de début autres que minuit sont ajustées à minuit avant l’heure spécifiée. Par exemple, 13h00 le 6 juin est ajusté à 00h00 le 6 juin.
    
- Les heures de fin autres que minuit sont ajustées à minuit après l’heure spécifiée. Par exemple, 13h00 le 6 juin est ajusté à 00h00 le 7 juin.
    
Ainsi, l’événement d’une journée que vous créez est toujours inclus entre l’heure de début et l’heure de fin que vous spécifiez, mais peut revendiquer du temps supplémentaire sur le calendrier de l’utilisateur en raison du passage à minuit. Étant donné que le serveur ajustera l’heure de début et de fin à minuit, nous vous recommandons de spécifier vos heures de début et de fin à minuit afin d’éviter toute modification inattendue des heures.
  
Il est également important de prendre en compte les fuseaux horaires lors de la création d’événements d’une journée. Étant donné que le serveur Exchange applique une heure de début et de fin à minuit dans le fuseau horaire de la demande ou du rendez-vous, l’affichage de cet événement sur une journée entière dans un client configuré pour un autre fuseau horaire peut produire des résultats inattendus. Selon le client, il peut apparaître comme un événement d’une journée entière avec des jours supplémentaires que vous n’avez pas l’intention d’inclure, ou il peut ne pas apparaître comme un événement d’une journée entière. Pour cette raison, nous vous recommandons d’utiliser le fuseau horaire préféré de l’utilisateur chaque fois que possible lorsque vous créez des événements d’une journée.
  
## <a name="create-an-all-day-event-by-using-the-ews-managed-api"></a>Créer un événement d’une journée à l’aide de l’API gérée EWS

L’exemple suivant montre comment utiliser l’API gérée EWS pour créer un événement d’une journée, en commençant à la date spécifiée par le paramètre _startDate_ et pendant le nombre de jours spécifié par le paramètre _numDays._ Notez que le rendez-vous sera créé dans le fuseau horaire spécifié par la [propriété ExchangeService.TimeZone.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) Cet exemple suppose que l’objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) transmis dans le paramètre _de service_ a été initialisé avec des valeurs valides pour les [propriétés Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) et [Url.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) 
  
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

## <a name="create-an-all-day-event-by-using-ews"></a>Créer un événement d’une journée à l’aide d’EWS

L’exemple suivant illustre une demande d’opération [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS pour créer un événement d’une journée. Le rendez-vous est créé dans le fuseau horaire Est, comme indiqué par [l’élément TimeZoneContext.](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) Notez que la partie heure des [](https://msdn.microsoft.com/library/72329821-32ff-495d-b6e5-fdc011003c2e%28Office.15%29.aspx) valeurs des éléments [Début](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) et Fin est 04:00Z, qui se convertit en minuit dans le fuseau horaire Est pendant l’heure d’été. 
  
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

## <a name="see-also"></a>Voir aussi


- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
    
- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Fuseaux horaires et EWS dans Exchange](time-zones-and-ews-in-exchange.md)
    

