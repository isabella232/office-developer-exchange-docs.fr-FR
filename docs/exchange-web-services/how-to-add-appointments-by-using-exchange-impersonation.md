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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754823"
---
# <a name="add-appointments-by-using-exchange-impersonation"></a><span data-ttu-id="fd039-103">Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange</span><span class="sxs-lookup"><span data-stu-id="fd039-103">Add appointments by using Exchange impersonation</span></span>

<span data-ttu-id="fd039-104">Découvrez comment utiliser l’emprunt d’identité avec les API managées EWS dans Exchange pour ajouter des rendez-vous dans les calendriers des utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="fd039-104">Learn how to use impersonation with the EWS Managed API or EWS in Exchange to add appointments to users' calendars.</span></span>
  
<span data-ttu-id="fd039-105">Vous pouvez créer une application de service qui insère des rendez-vous directement dans un calendrier Exchange à l’aide d’un compte de service dont le **AppplicationImpersonation**[rôle activé](how-to-configure-impersonation.md).</span><span class="sxs-lookup"><span data-stu-id="fd039-105">You can create a service application that inserts appointments directly into an Exchange calendar by using a service account that has the **AppplicationImpersonation**[role enabled](how-to-configure-impersonation.md).</span></span> <span data-ttu-id="fd039-106">Lorsque vous utilisez l’emprunt d’identité, l’application agit en tant que l’utilisateur ; Il est comme si l’utilisateur ajouté le rendez-vous au calendrier à l’aide d’un client comme Outlook.</span><span class="sxs-lookup"><span data-stu-id="fd039-106">When you use impersonation, the application is acting as the user; it's as if the user added the appointment to the calendar by using a client such as Outlook.</span></span> 
  
<span data-ttu-id="fd039-107">Lorsque vous utilisez l’emprunt d’identité, gardez à l’esprit les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="fd039-107">When you are using impersonation, keep in mind the following:</span></span>
  
- <span data-ttu-id="fd039-108">L’objet [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) doit être lié au compte de service.</span><span class="sxs-lookup"><span data-stu-id="fd039-108">Your [ExchangeService](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx) object must be bound to the service account.</span></span> <span data-ttu-id="fd039-109">Vous pouvez utiliser le même objet **ExchangeService** pour emprunter l’identité de plusieurs comptes en modifiant la propriété [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) pour chaque compte que vous souhaitez emprunter l’identité.</span><span class="sxs-lookup"><span data-stu-id="fd039-109">You can use the same **ExchangeService** object to impersonate multiple accounts by changing the [ImpersonatedUserId](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property for each account that you want to impersonate.</span></span> 
    
- <span data-ttu-id="fd039-110">N’importe quel élément que vous enregistrez dans un compte représenté utilisable uniquement une seule fois.</span><span class="sxs-lookup"><span data-stu-id="fd039-110">Any item that you save to an impersonated account can only be used once.</span></span> <span data-ttu-id="fd039-111">Par exemple, si vous souhaitez enregistrer le rendez-vous même dans plusieurs comptes, vous devez créer un objet de [rendez-vous](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) pour chaque compte.</span><span class="sxs-lookup"><span data-stu-id="fd039-111">If you want to save the same appointment in multiple accounts, for example, you have to create an [Appointment](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.aspx) object for each account.</span></span> 
    
## <a name="prerequisites"></a><span data-ttu-id="fd039-112">Conditions préalables</span><span class="sxs-lookup"><span data-stu-id="fd039-112">Prerequisites</span></span>

<span data-ttu-id="fd039-113">Votre application a besoin d’un compte à utiliser pour se connecter au serveur Exchange avant de pouvoir utiliser l’emprunt d’identité.</span><span class="sxs-lookup"><span data-stu-id="fd039-113">Your application needs an account to use to connect to the Exchange server before it can use impersonation.</span></span> <span data-ttu-id="fd039-114">Nous vous suggérons d’utiliser un compte de service pour l’application qui a reçu le rôle d’emprunt d’identité de l’Application pour les comptes qui y accéderont.</span><span class="sxs-lookup"><span data-stu-id="fd039-114">We suggest that you use a service account for the application that has been granted the Application Impersonation role for the accounts that it will be accessing.</span></span> <span data-ttu-id="fd039-115">Pour plus d’informations, voir [configurer l’emprunt d’identité](how-to-configure-impersonation.md)</span><span class="sxs-lookup"><span data-stu-id="fd039-115">For more information, see [Configure impersonation](how-to-configure-impersonation.md)</span></span>
  
## <a name="add-appointments-by-using-impersonation-with-the-ews-managed-api"></a><span data-ttu-id="fd039-116">Ajouter des rendez-vous à l’aide de l’emprunt d’identité avec l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="fd039-116">Add appointments by using impersonation with the EWS Managed API</span></span>

<span data-ttu-id="fd039-117">L’exemple suivant ajoute une réunion ou rendez-vous au calendrier d’un ou plusieurs comptes Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd039-117">The following example adds an appointment or meeting to the calendar of one or more Exchange accounts.</span></span> <span data-ttu-id="fd039-118">La méthode accepte trois paramètres.</span><span class="sxs-lookup"><span data-stu-id="fd039-118">The method takes three parameters.</span></span>
  
-  <span data-ttu-id="fd039-119">_service_ — un objet **ExchangeService** lié au compte de l’application de service sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd039-119">_service_ — An **ExchangeService** object bound to the service application's account on the Exchange server.</span></span> 
    
-  <span data-ttu-id="fd039-120">_emailAddresses_ , un objet [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) contenant une liste de chaînes d’adresse électronique SMTP.</span><span class="sxs-lookup"><span data-stu-id="fd039-120">_emailAddresses_ — A [System.List](http://msdn.microsoft.com/library/6sh2ey19.aspx) object containing a list of SMTP email address strings.</span></span> 
    
-  <span data-ttu-id="fd039-121">_répartiteur_ — un objet qui implémente l’interface **IAppointmentFactory** .</span><span class="sxs-lookup"><span data-stu-id="fd039-121">_factory_ — An object that implements the **IAppointmentFactory** interface.</span></span> <span data-ttu-id="fd039-122">Cette interface possède une méthode, **GetAppointment** qui prend un objet **ExchangeService** en tant que paramètre et renvoie un objet de **rendez-vous** .</span><span class="sxs-lookup"><span data-stu-id="fd039-122">This interface has one method, **GetAppointment** that takes an **ExchangeService** object as a parameter and returns an **Appointment** object.</span></span> <span data-ttu-id="fd039-123">L’interface **IAppointmentFactory** est définie par [l’interface IAppointmentFactory](#bk_IAppointmentFactory).</span><span class="sxs-lookup"><span data-stu-id="fd039-123">The **IAppointmentFactory** interface is defined [IAppointmentFactory interface](#bk_IAppointmentFactory).</span></span>
    
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

<span data-ttu-id="fd039-124">Lorsque vous enregistrez le rendez-vous, le code vérifie pour déterminer si les participants ont été ajoutés à la propriété [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fd039-124">When saving the appointment, the code checks to determine whether any attendees have been added to the [RequiredAttendees](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.requiredattendees.aspx) property.</span></span> <span data-ttu-id="fd039-125">S’ils disposent, la méthode [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) est appelée avec la valeur d’énumération [SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) afin que les participants reçoivent des demandes de réunion ; dans le cas contraire, la méthode **Appointment.Save** est appelée avec la valeur d’énumération [SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) afin que le rendez-vous est enregistré dans le calendrier de l’utilisateur avec emprunt d’identité avec la propriété [Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) la valeur **false**.</span><span class="sxs-lookup"><span data-stu-id="fd039-125">If they have, the [Appointment.Save](http://msdn.microsoft.com/library/dd635394.aspx) method is called with the [SendToAllAndSaveCopy](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the attendees receive meeting requests; otherwise, the **Appointment.Save** method is called with the [SendToNone](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.sendinvitationsmode.aspx) enumeration value so that the appointment is saved into the impersonated user's calendar with the [Appointment.IsMeeting](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.ismeeting.aspx) property set to **false**.</span></span>
  
### <a name="iappointmentfactory-interface"></a><span data-ttu-id="fd039-126">Interface IAppointmentFactory</span><span class="sxs-lookup"><span data-stu-id="fd039-126">IAppointmentFactory interface</span></span>
<span data-ttu-id="fd039-127"><a name="bk_IAppointmentFactory"> </a></span><span class="sxs-lookup"><span data-stu-id="fd039-127"></span></span>

<span data-ttu-id="fd039-128">Vous devez chaque fois que vous souhaitez enregistrer un rendez-vous dans le calendrier de l’emprunt d’identité d’un utilisateur à un nouvel objet de **rendez-vous** , l’interface **IAppointmentFactory** extrait l’objet utilisé pour remplir chaque objet **Appointment** .</span><span class="sxs-lookup"><span data-stu-id="fd039-128">Because you need a new **Appointment** object each time that you want to save an appointment on an impersonated user's calendar, the **IAppointmentFactory** interface abstracts the object used to populate each **Appointment** object.</span></span> <span data-ttu-id="fd039-129">Cette version est une interface simple qui contient une seule méthode, **GetAppointment**, qui prend un objet **ExchangeService** en tant que paramètre et renvoie un nouvel objet **rendez-vous** lié à cet objet **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="fd039-129">This version is a simple interface that contains only one method, **GetAppointment**, that takes an **ExchangeService** object as a parameter and returns a new **Appointment** object bound to that **ExchangeService** object.</span></span> 
  
```cs
interface IAppointmentFactory
{
  Appointment GetAppointment(ExchangeService service);
}
```

<span data-ttu-id="fd039-130">L’exemple de classe **AppointmentFactory** suivant illustre une implémentation de l’interface **IAppointmentFactory** qui renvoie un rendez-voius simple qui se produit trois jours à partir de maintenant.</span><span class="sxs-lookup"><span data-stu-id="fd039-130">The following **AppointmentFactory** class example shows an implementation of the **IAppointmentFactory** interface that returns a simple appointment that occurs three days from now.</span></span> <span data-ttu-id="fd039-131">Si vous supprimez le commentaire du `appointment.RequiredAttendees.Add` ligne, la méthode **GetAppointment** renverra une réunion et l’adresse de messagerie spécifiée dans cette ligne reçoit une demande de réunion avec l’emprunt d’identité utilisateur répertorié en tant que l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="fd039-131">If you uncomment the  `appointment.RequiredAttendees.Add` line, the **GetAppointment** method will return a meeting and the email address specified in that line will receive a meeting request with the impersonated user listed as the organizer.</span></span> 
  
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

## <a name="add-appointments-by-using-impersonation-with-ews"></a><span data-ttu-id="fd039-132">Ajouter des rendez-vous à l’aide de l’emprunt d’identité avec EWS</span><span class="sxs-lookup"><span data-stu-id="fd039-132">Add appointments by using impersonation with EWS</span></span>

<span data-ttu-id="fd039-133">EWS permet à votre application pour utiliser l’emprunt d’identité pour ajouter des éléments à un calendrier de la part du propriétaire du calendrier.</span><span class="sxs-lookup"><span data-stu-id="fd039-133">EWS enables you application to use impersonation to add items to a calendar on behalf the calendar's owner.</span></span> <span data-ttu-id="fd039-134">Cet exemple montre comment utiliser l’opération [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour ajouter un rendez-vous au calendrier d’un compte d’emprunt d’identité.</span><span class="sxs-lookup"><span data-stu-id="fd039-134">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to add an appointment to the calendar of an impersonated account.</span></span> 
  
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

<span data-ttu-id="fd039-135">Notez qu’autre que l’ajout de l’élément **ExchangeImpersonation** dans l’en-tête SOAP pour spécifier le compte que nous effectuons à emprunt d’identité, il s’agit de la même requête XML utilisée pour créer un rendez-vous sans l’aide de l’emprunt d’identité.</span><span class="sxs-lookup"><span data-stu-id="fd039-135">Note that other than the addition of the **ExchangeImpersonation** element in the SOAP header to specify the account that we are impersonating, this is the same XML request used to create an appointment without using impersonation.</span></span> 
  
<span data-ttu-id="fd039-136">L'exemple suivant présente le code XML de réponse renvoyé par l'opération **CreateItem**.</span><span class="sxs-lookup"><span data-stu-id="fd039-136">The following example shows the response XML that is returned by the **CreateItem** operation.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="fd039-137">Les attributs **ItemId** et **ChangeKey** sont limitent pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="fd039-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

<span data-ttu-id="fd039-138">Là encore, il s’agit du même fichier XML qui est renvoyé lorsque vous utilisez l’opération **CreateItem** sans l’aide de l’emprunt d’identité.</span><span class="sxs-lookup"><span data-stu-id="fd039-138">Again, this is the same XML that is returned when you use the **CreateItem** operation without using impersonation.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="fd039-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fd039-139">See also</span></span>


- [<span data-ttu-id="fd039-140">Emprunt d'identité et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fd039-140">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="fd039-141">Rôle ApplicationImpersonation</span><span class="sxs-lookup"><span data-stu-id="fd039-141">ApplicationImpersonation role</span></span>](http://technet.microsoft.com/fr-fr/library/dd776119%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="fd039-142">Configurer l’emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="fd039-142">Configure impersonation</span></span>](how-to-configure-impersonation.md)
    
- [<span data-ttu-id="fd039-143">Identifier le compte pour emprunter l’identité</span><span class="sxs-lookup"><span data-stu-id="fd039-143">Identify the account to impersonate</span></span>](how-to-identify-the-account-to-impersonate.md)
    
- [<span data-ttu-id="fd039-144">Créer des rendez-vous et réunions à l’aide de EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="fd039-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="fd039-145">Opération CreateItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="fd039-145">CreateItem operation (calendar item)</span></span>](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)
    
- [<span data-ttu-id="fd039-146">Propriété ExchangeService.ImpersonatedUserId</span><span class="sxs-lookup"><span data-stu-id="fd039-146">ExchangeService.ImpersonatedUserId property</span></span>](http://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx.aspx)
    

