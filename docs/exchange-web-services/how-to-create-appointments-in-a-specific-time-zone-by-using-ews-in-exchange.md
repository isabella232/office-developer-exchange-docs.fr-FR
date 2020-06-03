---
title: Créer des rendez-vous dans un fuseau horaire spécifique à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e68aaa27-250e-4170-b099-077a979c127c
description: Découvrez comment créer des rendez-vous dans des fuseaux horaires spécifiques à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 9b1160a9d62ab092d1b60265eba1ad953be0032b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456856"
---
# <a name="create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange"></a>Créer des rendez-vous dans un fuseau horaire spécifique à l’aide d’EWS dans Exchange

Découvrez comment créer des rendez-vous dans des fuseaux horaires spécifiques à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
Lorsqu’un rendez-vous ou une réunion est créé dans un calendrier Exchange, le fuseau horaire utilisé pour spécifier les heures de début et de fin est enregistré comme fuseau horaire de création pour le rendez-vous. Ce fuseau horaire est également utilisé pour [interpréter les valeurs de date et d’heure qui n’ont pas de fuseau horaire explicite spécifié](time-zones-and-ews-in-exchange.md), c’est pourquoi il est important de comprendre les options permettant de spécifier le fuseau horaire.
  
## <a name="creating-appointments-in-different-time-zones-by-using-the-ews-managed-api"></a>Création de rendez-vous dans différents fuseaux horaires à l’aide de l’API managée EWS

Lorsque vous créez des rendez-vous ou des réunions à l’aide de l’API managée EWS, vous disposez de trois options pour spécifier le fuseau horaire :
  
- Pour utiliser le fuseau horaire de l’ordinateur sur lequel votre API managée EWS est en cours d’exécution, ne spécifiez pas de fuseau horaire lors de la création de l’objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) . 
    
- Pour utiliser un fuseau horaire spécifique pour toutes les propriétés de date/heure, y compris les propriétés lors de la création d’un rendez-vous ou d’une réunion, spécifiez un fuseau horaire dans le constructeur pour l’objet **ExchangeService** . 
    
- Pour utiliser un autre fuseau horaire que celui spécifié dans la propriété [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) , utilisez les propriétés appointment. [StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) et appointment [. EndTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) . 
    
    > [!NOTE]
    > La propriété **EndTimeZone** est disponible uniquement lorsque la propriété [ExchangeService. RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) est définie sur **Exchange2010** ou une version ultérieure. Si elle n’est pas disponible, la définition de **StartTimeZone** s’applique aux heures de début et de fin du rendez-vous. 
  
Dans l’exemple suivant, l’API managée EWS est utilisée pour créer trois rendez-vous. Chaque rendez-vous est défini pour démarrer à 1:00 à partir de deux jours, dans un fuseau horaire non spécifié et se terminer une heure plus tard. Le premier rendez-vous est créé dans le fuseau horaire de l’ordinateur client en utilisant le comportement par défaut de l’API managée EWS. La deuxième est créée dans le fuseau horaire central à l’aide des propriétés appointment **. StartTimeZone** et appointment **. EndTimeZone** . Le troisième est créé dans le fuseau horaire montagnes à l’aide de la propriété **ExchangeService. TimeZone** . 
  
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

Lorsque cet exemple est exécuté sur un ordinateur client configuré dans le fuseau horaire est et que les trois rendez-vous qu’il crée sont affichés à partir d’un client configuré dans le fuseau horaire est, ils apparaissent à 1:00 PM, 2:00 PM et 3:00 PM, respectivement.
  
## <a name="creating-appointments-in-different-time-zones-by-using-ews"></a>Création de rendez-vous dans différents fuseaux horaires à l’aide d’EWS

Lorsque vous créez des rendez-vous ou des réunions à l’aide d’EWS, vous disposez de trois options pour spécifier le fuseau horaire :
  
- Pour utiliser le temps universel coordonné (UTC), n’incluez pas un élément [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , un élément [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) (Exchange 2007 uniquement) ou des éléments [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (Exchange 2010 et versions ultérieures) dans la demande d' [opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) . 
    
- Pour utiliser un fuseau horaire spécifique pour toutes les propriétés de date/heure, y compris les propriétés lors de la création d’un rendez-vous ou d’une réunion, spécifiez un fuseau horaire dans l’élément [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) de la demande de l' [opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) . 
    
- Pour utiliser un fuseau horaire différent de celui spécifié dans l’élément [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , incluez un élément [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) , un élément [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) (Exchange 2007 uniquement) ou des éléments [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (Exchange 2010 et versions ultérieures) dans la demande d' [opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) . 
    
L’exemple suivant de demande d' [opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) crée un rendez-vous à l’aide de l’UTC. Notez que l’élément **TimeZoneContext** , l’élément **StartTimeZone** et l’élément **EndTimeZone** sont absents. Les valeurs des éléments **Start** et **end** sont exprimées au format UTC. 
  
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

L’exemple suivant de demande d' [opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) utilise les éléments **StartTimeZone** et **EndTimeZone** pour spécifier le fuseau horaire central pour le rendez-vous. Notez que l’élément **TimeZoneContext** est absent. Toutefois, s’il était présent, les valeurs des éléments **StartTimeZone** et **EndTimeZone** substitueront sa valeur. Encore une fois, les valeurs des éléments **Start** et **end** sont exprimées au format UTC. 
  
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

Dans l’exemple suivant, la demande de l' [opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) définit l’élément **TimeZoneContext** sur le fuseau horaire montagnes Rocheuses. Notez que les éléments **StartTimeZone** et **EndTimeZone** sont absents. Encore une fois, les valeurs des éléments **Start** et **end** sont exprimées au format UTC. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Lorsque les trois rendez-vous créés par les requêtes d’exemple EWS précédentes sont visualisés à partir d’un client configuré dans le fuseau horaire est, ils apparaissent respectivement à 1:00 PM, 2:00 PM et 3:00 PM.
  
## 

Maintenant que vous saurez comment créer des rendez-vous dans des fuseaux horaires spécifiques, vous souhaiterez peut-être [mettre à jour les fuseaux horaires des rendez-vous existants](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md) . 
  
## <a name="see-also"></a>Voir aussi


- [Fuseaux horaires et EWS dans Exchange](time-zones-and-ews-in-exchange.md)
    
- [Mettre à jour le fuseau horaire pour un rendez-vous à l’aide d’EWS dans Exchange](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    

