---
title: Créer des rendez-vous dans un fuseau horaire spécifique à l’aide d’EWS Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: e68aaa27-250e-4170-b099-077a979c127c
description: Découvrez comment créer des rendez-vous dans des fuseaux horaires spécifiques à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 589c72982fdda568170468c376b8a6d9f598aa36
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521143"
---
# <a name="create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange"></a>Créer des rendez-vous dans un fuseau horaire spécifique à l’aide d’EWS Exchange

Découvrez comment créer des rendez-vous dans des fuseaux horaires spécifiques à l’aide de l’API gérée EWS ou d’EWS dans Exchange.
  
Lorsqu’un rendez-vous ou une réunion est créé sur un calendrier Exchange, le fuseau horaire utilisé pour spécifier les heures de début et de fin est enregistré en tant que fuseau horaire de création pour le rendez-vous. Ce fuseau horaire est également utilisé pour interpréter les valeurs de [date](time-zones-and-ews-in-exchange.md)et d’heure qui n’ont pas de fuseau horaire explicite spécifié. Il est donc important de comprendre vos options pour spécifier le fuseau horaire.
  
## <a name="creating-appointments-in-different-time-zones-by-using-the-ews-managed-api"></a>Création de rendez-vous dans différents fuseaux horaires à l’aide de l’API gérée EWS

Lorsque vous créez des rendez-vous ou des réunions à l’aide de l’API gérée EWS, vous avez trois options pour spécifier le fuseau horaire :
  
- Pour utiliser le fuseau horaire de l’ordinateur sur lequel votre API gérée EWS est exécutée, ne spécifiez pas de fuseau horaire lors de la création de [l’objet ExchangeService.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) 
    
- Pour utiliser un fuseau horaire spécifique pour toutes les propriétés de date/heure, y compris les propriétés lors de la création d’un rendez-vous ou d’une réunion, spécifiez un fuseau horaire dans le constructeur pour **l’objet ExchangeService.** 
    
- Pour utiliser un fuseau horaire différent de celui spécifié dans la propriété [ExchangeService.TimeZone,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) utilisez les propriétés [Appointment.StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) et [Appointment.EndTimeZone.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) 
    
    > [!NOTE]
    > La **propriété EndTimeZone** est disponible uniquement lorsque la propriété [ExchangeService.RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) est définie sur **Exchange2010** ou version ultérieure. Si elle n’est pas disponible, la définition **de StartTimeZone** s’applique aux heures de début et de fin du rendez-vous. 
  
Dans l’exemple suivant, l’API gérée EWS est utilisée pour créer trois rendez-vous. Chaque rendez-vous est fixé à 13h00 dans deux jours, dans un fuseau horaire non spécifié, et se termine une heure plus tard. Le premier rendez-vous est créé dans le fuseau horaire de l’ordinateur client à l’aide du comportement par défaut de l’API gérée EWS. Le second est créé dans le fuseau horaire central à l’aide des propriétés **Appointment.StartTimeZone** et **Appointment.EndTimeZone.** Le troisième est créé dans le fuseau horaire de mountain à l’aide de **la propriété ExchangeService.TimeZone.** 
  
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

Lorsque cet exemple est exécuté sur un ordinateur client configuré dans le fuseau horaire Est et que les trois rendez-vous créés sont consultables à partir d’un client configuré dans le fuseau horaire Est, ils apparaissent respectivement à 13 h 00, 14 h 00 et 15 h 00.
  
## <a name="creating-appointments-in-different-time-zones-by-using-ews"></a>Création de rendez-vous dans différents fuseaux horaires à l’aide d’EWS

Lorsque vous créez des rendez-vous ou des réunions à l’aide d’EWS, vous avez trois options pour spécifier le fuseau horaire :
  
- Pour utiliser le temps universel coordonné (UTC), n’incluez pas d’élément [TimeZoneContext,](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) [d’élément MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) (Exchange 2007 uniquement) ou d’éléments [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (Exchange 2010 et ultérieur) dans la demande d’opération [CreateItem.](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 
    
- Pour utiliser un fuseau horaire spécifique pour toutes les propriétés de date/heure, y compris les propriétés lors de la création d’un rendez-vous ou d’une réunion, spécifiez un fuseau horaire dans l’élément [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) dans la demande d’opération [CreateItem.](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 
    
- Pour utiliser un fuseau horaire différent de celui spécifié dans l’élément [TimeZoneContext,](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) incluez un élément [TimeZoneContext,](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) un élément [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx) (Exchange 2007 uniquement) ou des éléments [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx) et [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (Exchange 2010 et ultérieures) dans la demande d’opération [CreateItem.](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) 
    
L’exemple de [demande d’opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) suivant crée un rendez-vous à l’aide de l’UTC. Notez que **l’élément TimeZoneContext,** **l’élément StartTimeZone** et l’élément **EndTimeZone** sont absents. Les **valeurs des** éléments Start et **End** sont exprimées au UTC. 
  
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

L’exemple [de demande d’opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) suivant utilise les éléments **StartTimeZone** et **EndTimeZone** pour spécifier le fuseau horaire central du rendez-vous. Notez que **l’élément TimeZoneContext** est absent. Toutefois, si elle était présente, les valeurs des éléments **StartTimeZone** et **EndTimeZone** remplaceraient sa valeur. Là encore, les **valeurs des** éléments Start et **End** sont exprimées au UTC. 
  
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

L’exemple [de demande d’opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) suivant définit l’élément **TimeZoneContext** sur le fuseau horaire De la mountain. Notez que **les éléments StartTimeZone** et **EndTimeZone** sont absents. Là encore, les **valeurs des** éléments Start et **End** sont exprimées au UTC. 
  
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

Lorsque les trois rendez-vous créés par les exemples de demandes EWS précédents sont consultables à partir d’un client configuré dans le fuseau horaire Est, ils apparaissent respectivement à 13h00, 14h00 et 15h00.
  
## 

Maintenant que vous savez comment créer des rendez-vous dans des fuseaux horaires spécifiques, vous pouvez mettre à jour les fuseaux horaires des rendez-vous [existants](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md) vers un autre. 
  
## <a name="see-also"></a>Voir aussi


- [Fuseaux horaires et EWS dans Exchange](time-zones-and-ews-in-exchange.md)
    
- [Mettre à jour le fuseau horaire d’un rendez-vous à l’aide d’EWS Exchange](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    

