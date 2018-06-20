---
title: Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78d5e51b-900f-4302-b9a8-fdc9aa4b65a5
description: Découvrez comment utiliser l’emprunt d’identité avec les API managées EWS dans Exchange pour ajouter des rendez-vous dans les calendriers des utilisateurs.
ms.openlocfilehash: fe737658b88aca66d8b4c2860245db000888ba17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754823"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a>Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange

Découvrez comment utiliser l’emprunt d’identité avec les API managées EWS dans Exchange pour ajouter des rendez-vous dans les calendriers des utilisateurs.
  
Vous pouvez créer une application de service qui insère des rendez-vous directement dans un calendrier Exchange à l’aide d’un compte de service dont le **AppplicationImpersonation**[rôle activé](how-to-configure-impersonation.md). Lorsque vous utilisez l’emprunt d’identité, l’application agit en tant que l’utilisateur ; Il est comme si l’utilisateur ajouté le rendez-vous au calendrier à l’aide d’un client comme Outlook. 
  
Lorsque vous utilisez l’emprunt d’identité, gardez à l’esprit les éléments suivants :
  
- L’objet [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) doit être lié au compte de service. Vous pouvez utiliser le même objet **ExchangeService** pour emprunter l’identité de plusieurs comptes en modifiant la propriété [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) pour chaque compte que vous souhaitez emprunter l’identité. 
    
- N’importe quel élément que vous enregistrez dans un compte représenté utilisable uniquement une seule fois. Par exemple, si vous souhaitez enregistrer le rendez-vous même dans plusieurs comptes, vous devez créer un objet de [rendez-vous](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) pour chaque compte. 
    
## <a name="prerequisites"></a>Conditions préalables

Votre application a besoin d’un compte à utiliser pour se connecter au serveur Exchange avant de pouvoir utiliser l’emprunt d’identité. Nous vous suggérons d’utiliser un compte de service pour l’application qui a reçu le rôle d’emprunt d’identité de l’Application pour les comptes qui y accéderont. Pour plus d’informations, voir [configurer l’emprunt d’identité](how-to-configure-impersonation.md)
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a>Ajouter des rendez-vous à l’aide de l’emprunt d’identité avec l’API managée EWS

L’exemple suivant ajoute une réunion ou rendez-vous au calendrier d’un ou plusieurs comptes Exchange. La méthode accepte trois paramètres.
  
-  _service_ — un objet **ExchangeService** lié au compte de l’application de service sur le serveur Exchange. 
    
-  _emailAddresses_ , un objet [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) contenant une liste de chaînes d’adresse électronique SMTP. 
    
-  _répartiteur_ — un objet qui implémente l’interface **IAppointmentFactory** . Cette interface possède une méthode, **GetAppointment** qui prend un objet **ExchangeService** en tant que paramètre et renvoie un objet de **rendez-vous** . L’interface **IAppointmentFactory** est définie par [l’interface IAppointmentFactory](#bk_IAppointmentFactory).
    
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

Lorsque vous enregistrez le rendez-vous, le code vérifie pour déterminer si les participants ont été ajoutés à la propriété [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) . S’ils disposent, la méthode [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) est appelée avec la valeur d’énumération [SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) afin que les participants reçoivent des demandes de réunion ; dans le cas contraire, la méthode **Appointment.Save** est appelée avec la valeur d’énumération [SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) afin que le rendez-vous est enregistré dans le calendrier de l’utilisateur avec emprunt d’identité avec la propriété [Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) la valeur **false**.
  
### <a name="iappointmentfactory-interface"></a>Interface IAppointmentFactory
<a name="bk_IAppointmentFactory"> </a>

Vous devez chaque fois que vous souhaitez enregistrer un rendez-vous dans le calendrier de l’emprunt d’identité d’un utilisateur à un nouvel objet de **rendez-vous** , l’interface **IAppointmentFactory** extrait l’objet utilisé pour remplir chaque objet **Appointment** . Cette version est une interface simple qui contient une seule méthode, **GetAppointment**, qui prend un objet **ExchangeService** en tant que paramètre et renvoie un nouvel objet **rendez-vous** lié à cet objet **ExchangeService** . 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

L’exemple de classe **AppointmentFactory** suivant illustre une implémentation de l’interface **IAppointmentFactory** qui renvoie un rendez-voius simple qui se produit trois jours à partir de maintenant. Si vous supprimez le commentaire du `appointment.RequiredAttendees.Add` ligne, la méthode **GetAppointment** renverra une réunion et l’adresse de messagerie spécifiée dans cette ligne reçoit une demande de réunion avec l’emprunt d’identité utilisateur répertorié en tant que l’organisateur. 
  
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

EWS permet à votre application pour utiliser l’emprunt d’identité pour ajouter des éléments à un calendrier de la part du propriétaire du calendrier. Cet exemple montre comment utiliser l’opération [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour ajouter un rendez-vous au calendrier d’un compte d’emprunt d’identité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Notez qu’autre que l’ajout de l’élément **ExchangeImpersonation** dans l’en-tête SOAP pour spécifier le compte que nous effectuons à emprunt d’identité, il s’agit de la même requête XML utilisée pour créer un rendez-vous sans l’aide de l’emprunt d’identité. 
  
L'exemple suivant présente le code XML de réponse renvoyé par l'opération **CreateItem**. 
  
> [!NOTE]
> Les attributs **ItemId** et **ChangeKey** sont limitent pour une meilleure lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Là encore, il s’agit du même fichier XML qui est renvoyé lorsque vous utilisez l’opération **CreateItem** sans l’aide de l’emprunt d’identité. 
  
## <a name="see-also"></a>Voir aussi


- [Emprunt d'identité et EWS dans Exchange](impersonation-and-ews-in-exchange.md)
    
- [Rôle ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx)
    
- [Configurer l’emprunt d’identité](how-to-configure-impersonation.md)
    
- [Identifier le compte pour emprunter l’identité](how-to-identify-the-account-to-impersonate.md)
    
- [Créer des rendez-vous et réunions à l’aide de EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Opération CreateItem (élément de calendrier)](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)
    
- [Propriété ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx.aspx)
    

