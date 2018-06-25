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
# <a name="create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange"></a>Créer des rendez-vous dans un fuseau horaire spécifique à l’aide de EWS dans Exchange

Découvrez comment créer des rendez-vous dans des fuseaux horaires spécifiques à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Création d’un rendez-vous ou une réunion dans un calendrier Exchange, le fuseau horaire permet de spécifier les heures de début et de fin est enregistré en tant que le fuseau horaire de création pour le rendez-vous. Ce fuseau horaire est également utilisé pour [interpréter les valeurs de date et heure qui n’ont pas un indication de fuseau horaire explicit](time-zones-and-ews-in-exchange.md), il est important de comprendre les options pour spécifier le fuseau horaire.
  
## <a name="creating-appointments-in-different-time-zones-by-using-the-ews-managed-api"></a>Création de rendez-vous dans différents fuseaux horaires à l’aide de l’API managée EWS

Lorsque vous créez des rendez-vous ou des réunions à l’aide de l’API managée EWS, vous disposez de trois options pour spécifier le fuseau horaire :
  
- Pour utiliser le fuseau horaire de l’ordinateur où s’exécute votre API managées, ne spécifiez pas un fuseau horaire lors de la création de l’objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) . 
    
- Pour utiliser un fuseau horaire spécifique pour toutes les propriétés de date/heure, y compris les propriétés lors de la création d’un nouveau rendez-vous ou une réunion, spécifiez un fuseau horaire dans le constructeur de l’objet **ExchangeService** . 
    
- Pour utiliser un fuseau horaire différent de celui spécifié dans la propriété [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) , utilisez les propriétés [Appointment.StartTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) et [Appointment.EndTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) . 
    
    > [!NOTE]
    > La propriété **EndTimeZone** est disponible uniquement lorsque la propriété [ExchangeService.RequestedServerVersion](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) est définie sur **Exchange2010** ou version ultérieure. S’il n’est pas disponible, définition **StartTimeZone** s’applique aux heures de début et de fin du rendez-vous. 
  
Dans l’exemple suivant, l’API managée EWS est utilisée pour créer des trois rendez-vous. Chaque rendez-vous est configuré pour démarrer à 1 h 00 deux jours à partir de maintenant, dans un fuseau horaire non spécifié et de fin, une heure plus tard. Le premier rendez-vous est créé dans le fuseau horaire de l’ordinateur client à l’aide de comportement d’API managées par défaut. Le second est créé dans le fuseau horaire Central en utilisant les propriétés **Appointment.StartTimeZone** et **Appointment.EndTimeZone** . La troisième est créée dans Paris à l’aide de la propriété **ExchangeService.TimeZone** . 
  
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

Lorsque cet exemple est exécuté sur un ordinateur client configuré dans le fuseau horaire, et il crée trois rendez-vous sont affichés à partir d’un client configuré dans le fuseau horaire, ils apparaissent à 1:00 PM, 2 h 00 et 3 h 00, respectivement.
  
## <a name="creating-appointments-in-different-time-zones-by-using-ews"></a>Création de rendez-vous dans différents fuseaux horaires à l’aide de EWS

Lorsque vous créez des rendez-vous ou des réunions à l’aide de EWS, vous disposez de trois options pour spécifier le fuseau horaire :
  
- Pour utiliser le temps universel coordonné (UTC), ne pas inclure un élément [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) , élément (Exchange 2007 uniquement), ou [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et éléments [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (Exchange 2010 et versions ultérieur) dans le [ Opération CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) demande. 
    
- Pour utiliser un fuseau horaire spécifique pour toutes les propriétés de date/heure, y compris les propriétés lors de la création d’un nouveau rendez-vous ou une réunion, spécifiez un fuseau horaire dans l’élément [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) dans la requête [d’opération CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) . 
    
- Pour utiliser un fuseau horaire différent de celui spécifié dans l’élément [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , incluez un élément [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) , élément (Exchange 2007 uniquement) ou (éléments) [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) Exchange 2010 et versions ultérieur) dans la requête [d’opération CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) . 
    
L’exemple de requête [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) suivant crée un rendez-vous à l’aide au format UTC. Notez que l’élément **TimeZoneContext** , l’élément **StartTimeZone** et l’élément **EndTimeZone** sont absents. Les valeurs d’élément **Start** et **End** sont exprimés au format UTC. 
  
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

L’exemple de requête [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) suivant utilise les éléments **StartTimeZone** et **EndTimeZone** pour spécifier le fuseau horaire Central pour le rendez-vous. Notez que l’élément **TimeZoneContext** est absent. Toutefois, s’il s’agissait il est présent, les valeurs des éléments **StartTimeZone** et **EndTimeZone** seraient remplacer sa valeur. Encore une fois, les valeurs d’élément **Start** et **End** sont exprimés au format UTC. 
  
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

L’exemple de requête [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) suivant définit l’élément **TimeZoneContext** Paris. Notez que les éléments **StartTimeZone** et **EndTimeZone** absents. Encore une fois, les valeurs d’élément **Start** et **End** sont exprimés au format UTC. 
  
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

Lorsque les trois rendez-vous créés par les demandes d’exemple EWS précédentes sont affichés à partir d’un client configuré dans le fuseau horaire, elles apparaissent à 13 h 00, 2 h 00 et 3 h 00, respectivement.
  
## 

Maintenant que vous savez comment créer un rendez-vous dans des fuseaux horaires spécifiques, vous souhaiterez [mettre à jour les fuseaux horaires dans les rendez-vous existants](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md) vers un autre. 
  
## <a name="see-also"></a>Voir aussi


- [Fuseaux horaires et EWS dans Exchange](time-zones-and-ews-in-exchange.md)
    
- [Mettre à jour le fuseau horaire pour un rendez-vous à l’aide de EWS dans Exchange](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
- [Créer des rendez-vous et réunions à l’aide de EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    

