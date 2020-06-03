---
title: Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: 78d5e51b-900f-4302-b9a8-fdc9aa4b65a5
description: Découvrez comment utiliser l’emprunt d’identité avec l’API managée EWS ou EWS dans Exchange pour ajouter des rendez-vous aux calendriers des utilisateurs.
localization_priority: Priority
ms.openlocfilehash: b1473d72113f8cc07d05364a4d87fedf23c7351d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455330"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a>Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange

Découvrez comment utiliser l’emprunt d’identité avec l’API managée EWS ou EWS dans Exchange pour ajouter des rendez-vous aux calendriers des utilisateurs.
  
Vous pouvez créer une application de service qui insère des rendez-vous directement dans un calendrier Exchange à l’aide d’un compte de service sur lequel le rôle **ApplicationImpersonation** est [activé](how-to-configure-impersonation.md). Lorsque vous utilisez l’emprunt d’identité, l’application agit comme l’utilisateur ; C’est comme si l’utilisateur a ajouté le rendez-vous au calendrier à l’aide d’un client tel qu’Outlook. 
  
Lorsque vous utilisez l’emprunt d’identité, gardez à l’esprit les points suivants :
  
- Votre objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) doit être lié au compte de service. Vous pouvez utiliser le même objet **ExchangeService** pour emprunter l’identité de plusieurs comptes en modifiant la propriété [ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) pour chaque compte dont vous souhaitez emprunter l’identité. 
    
- Tout élément que vous enregistrez sur un compte emprunté ne peut être utilisé qu’une seule fois. Si vous souhaitez enregistrer le même rendez-vous dans plusieurs comptes, par exemple, vous devez créer un objet de [rendez-](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) vous pour chaque compte. 
    
## <a name="prerequisites"></a>Conditions préalables

Votre application a besoin d’un compte à utiliser pour se connecter au serveur Exchange avant de pouvoir utiliser l’emprunt d’identité. Nous vous suggérons d’utiliser un compte de service pour l’application qui a reçu le rôle d’emprunt d’identité d’application pour les comptes auxquels elle accèdera. Pour plus d’informations, consultez la rubrique [configurer l’emprunt d’identité](how-to-configure-impersonation.md)
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a>Ajouter des rendez-vous à l’aide de l’emprunt d’identité avec l’API managée EWS

L’exemple suivant ajoute un rendez-vous ou une réunion au calendrier d’un ou de plusieurs comptes Exchange. La méthode utilise trois paramètres.
  
-  _service_ — objet **ExchangeService** lié au compte de l’application de service sur le serveur Exchange. 
    
-  _EmailAddresses_ : objet [System. List](https://msdn.microsoft.com/library/6sh2ey19.aspx) contenant une liste de chaînes d’adresses de messagerie SMTP. 
    
-  _Factory_ : objet qui implémente l’interface **IAppointmentFactory** . Cette interface possède une méthode, **GetAppointment** qui prend un objet **ExchangeService** comme paramètre et renvoie **un objet appointment** . L’interface **IAppointmentFactory** est définie [IAppointmentFactory interface](#bk_IAppointmentFactory).
    
```cs
private static void CreateAppointments(ExchangeService service, List<string> emailAddresses, IAppointmentFactory factory)
{
  // Loop through the list of email addresses to add the appointment.
  foreach (var emailAddress in emailAddresses)
  {
    Console.WriteLine(string.Format("  Placing appointment in calendar for {0}.", emailAddress));
    // Set the email address of the account to get the appointment.
    service.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, emailAddress);
    // Get the appointment to add.
    Appointment appointment = factory.GetAppointment(service);
    // Save the appointment.
    try
    {
      if (appointment.RequiredAttendees.Count > 0)
      {
        // The appointment has attendees so send them the meeting request.
        appointment.Save(SendInvitationsMode.SendToAllAndSaveCopy);
      }
      else
      {
        // The appointment does not have attendees, so just save to calendar.
        appointment.Save(SendInvitationsMode.SendToNone);
      }
    }
    catch (ServiceResponseException ex)
    {
      Console.WriteLine(string.Format("Could not create appointment for {0}", emailAddress));
      Console.WriteLine(ex.Message);
    }
  }
}
```

Lors de l’enregistrement du rendez-vous, le code vérifie si les participants ont été ajoutés à la propriété [RequiredAttendees](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) . Si c’est le cas, la méthode appointment [. Save](https://msdn.microsoft.com/library/dd635394.aspx) est appelée avec la valeur d’énumération [SendToAllAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) afin que les participants reçoivent des demandes de réunion ; dans le cas contraire, la méthode appointment **. Save** est appelée avec la valeur d’énumération [SendToNone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) afin que le rendez-vous soit enregistré dans le calendrier de l’utilisateur empruntés avec la propriété appointment [. IsMeeting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) définie sur **false**.
  
### <a name="iappointmentfactory-interface"></a>Interface IAppointmentFactory
<a name="bk_IAppointmentFactory"> </a>

Étant donné que vous avez besoin d’un nouvel objet de **rendez-** vous chaque fois que vous souhaitez enregistrer un rendez-vous sur le calendrier d’un utilisateur emprunté, l’interface **IAppointmentFactory** abstractionne l’objet utilisé pour remplir chaque objet de **rendez-vous** . Cette version est une interface simple qui contient une seule méthode, **GetAppointment**, qui prend un objet **ExchangeService** comme paramètre et renvoie un nouvel objet de **rendez-vous** lié à cet objet **ExchangeService** . 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

L’exemple de classe **AppointmentFactory** suivant illustre une implémentation de l’interface **IAppointmentFactory** qui renvoie un rendez-vous simple qui se produit désormais trois jours. Si vous supprimez les marques de commentaire de la `appointment.RequiredAttendees.Add` ligne, la méthode **GetAppointment** renvoie une réunion et l’adresse de messagerie spécifiée dans cette ligne reçoit une demande de réunion avec l’utilisateur représenté indiqué en tant qu’organisateur. 
  
```cs
class AppointmentFactory : IAppointmentFactory
{
  public Appointment GetAppointment(ExchangeService service)
  {
    // First create the appointment to add.
    Appointment appointment = new Appointment(service);
    // Set the properties on the appointment.
    appointment.Subject = "Tennis lesson";
    appointment.Body = "Focus on backhand this week.";
    appointment.Start = DateTime.Now.AddDays(3);
    appointment.End = appointment.Start.AddHours(1);
    appointment.Location = "Tennis club";
    // appointment.RequiredAttendees.Add(new Attendee("sonyaf@contoso1000.onmicrosoft.com"));
    return appointment;
  }
}

```

## <a name="add-appointments-by-using-impersonation-with-ews"></a>Ajouter des rendez-vous à l’aide de l’emprunt d’identité avec EWS

EWS vous permet d’utiliser l’emprunt d’identité pour ajouter des éléments à un calendrier pour le compte du propriétaire du calendrier. Cet exemple montre comment utiliser l’opération [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour ajouter un rendez-vous au calendrier d’un compte emprunté. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToNone">
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Tennis lesson</t:Subject>
          <t:Body BodyType="HTML">Focus on backhand this week.</t:Body>
          <t:ReminderDueBy>2013-09-19T14:37:10.732-07:00</t:ReminderDueBy>
          <t:Start>2013-09-21T19:00:00.000Z</t:Start>
          <t:End>2013-09-21T20:00:00.000Z</t:End>
          <t:Location>Tennis club</t:Location>
          <t:MeetingTimeZone TimeZoneName="Pacific Standard Time" />
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Notez que, à l’exception de l’ajout de l’élément **ExchangeImpersonation** dans l’en-tête SOAP, pour spécifier le compte que nous empruntons d’identité, il s’agit de la même demande XML que celle utilisée pour créer un rendez-vous sans utiliser l’emprunt d’identité. 
  
L'exemple suivant présente le code XML de réponse renvoyé par l'opération **CreateItem**. 
  
> [!NOTE]
> Les attributs **ItemId** et **ChangeKey** sont raccourcis pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

Encore une fois, il s’agit du même code XML qui est renvoyé lorsque vous utilisez l’opération **CreateItem** sans utiliser l’emprunt d’identité. 
  
## <a name="see-also"></a>Voir aussi


- [Emprunt d'identité et EWS dans Exchange](impersonation-and-ews-in-exchange.md)
    
- [Rôle ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)
    
- [Configurer l’emprunt d'identité](how-to-configure-impersonation.md)
    
- [Identifier le compte d’emprunt d’identité](how-to-identify-the-account-to-impersonate.md)
    
- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Opération CreateItem (élément de calendrier)](../web-service-reference/createitem-operation-calendar-item.md)
    
- [Propriété ExchangeService. ImpersonatedUserId](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid?view=exchange-ews-api)
    

