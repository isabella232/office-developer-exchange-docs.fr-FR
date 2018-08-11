---
title: Calendriers et EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b87b0180-f5b5-44e4-b6ac-4f23e476b03b
description: Découvrez les calendriers, les dossiers et les éléments de calendrier, les rendez-vous et les réunions dans Exchange.
ms.openlocfilehash: bb9702118ff1db66862a5788c2d8f58dd55c4d09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754760"
---
# <a name="calendars-and-ews-in-exchange"></a><span data-ttu-id="15917-103">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-103">Calendars and EWS in Exchange</span></span>

<span data-ttu-id="15917-104">Découvrez les calendriers, les dossiers et les éléments de calendrier, les rendez-vous et les réunions dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="15917-104">Learn about calendars, calendar folders and items, appointments, and meetings in Exchange.</span></span>
  
<span data-ttu-id="15917-105">Vous êtes probablement familiarisé avec de nombreuses fonctionnalités de calendrier des clients de messagerie comme Outlook, qui vous permettent d’effectuer le suivi de rendez-vous, de planifier des réunions, de vérifier la disponibilité de personnes, d’inviter des participants et de modifier ou d’annuler les réunions.</span><span class="sxs-lookup"><span data-stu-id="15917-105">You're probably familiar with many of the calendar features in email clients like Outlook, which enable you to track appointments, schedule meetings, check people's availability, invite attendees, and change or cancel meetings.</span></span>
  
<span data-ttu-id="15917-p101">Les fonctionnalités de calendrier dans Exchange sont légèrement différentes de celles que vous voyez dans un client comme Outlook. Au lieu d'afficher des informations, EWS dans Exchange vous permet d'effectuer des actions comme créer, stocker, envoyer ou modifier des informations. Pour utiliser EWS avec des calendriers, vous devez être familiarisé avec des concepts tels que le stockage d'informations, l'heure, la périodicité et le flux de messages. Plus spécifiquement, vous devez être familiarisé avec les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="15917-p101">Calendar-related features in Exchange are a little different than what you see in a client like Outlook. Instead of displaying information, EWS in Exchange enables you to do things like create, store, send, or change information. To use EWS to work with calendars, you'll need to be familiar with concepts such as information storage, time, recurrence, and message flow. More specifically, you'll need to be familiar with the following:</span></span>
  
- <span data-ttu-id="15917-110">Dossiers de calendrier, éléments de calendrier et affichages de calendrier</span><span class="sxs-lookup"><span data-stu-id="15917-110">Calendar folders, calendar items, and calendar views</span></span>
    
- <span data-ttu-id="15917-111">Demandes de réunion, réponses, planification, participants, ressources, salles et disponibilité</span><span class="sxs-lookup"><span data-stu-id="15917-111">Meeting requests, responses, scheduling, attendees, resources, rooms, and availability</span></span>
    
- <span data-ttu-id="15917-112">Durées, fuseaux horaires et heures de début et de fin des réunions et rendez-vous</span><span class="sxs-lookup"><span data-stu-id="15917-112">Time durations, time zones, and start and end times of meetings and appointments</span></span>
    
- <span data-ttu-id="15917-113">Séries périodiques, périodicités, exceptions et rendez-vous et réunions uniques</span><span class="sxs-lookup"><span data-stu-id="15917-113">Recurring series, recurrence patterns, exceptions, and single instance appointments and meetings</span></span>
    
<span data-ttu-id="15917-p102">Heureusement, EWS et l'API managée EWS fournissent un large éventail d'opérations et de méthodes qui vous permettent d'effectuer un large éventail de tâches de calendrier. Par exemple, à l'aide de l'API managée EWS, vous pouvez créer une réunion et envoyer des invitations aux participants avec simplement quelques lignes de code, comme illustré dans l'exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="15917-p102">Fortunately, EWS and the EWS Managed API provide a rich set of operations and methods that enable you to perform a wide range of calendar-related tasks. For example, using the EWS Managed API, you can create a meeting and send invitations to attendees with just a few lines of code, as shown in the following example.</span></span>
  
```cs
            Appointment meeting = new Appointment(service);
            // Set the properties on the meeting object to create the meeting.
            meeting.Subject = "Team building exercise";
            meeting.Body = "Let's learn to really work as a team and then have lunch!";
            meeting.Start = DateTime.Now.AddDays(2);
            meeting.End = meeting.Start.AddHours(2);
            meeting.Location = "Conference Room 12";
            meeting.RequiredAttendees.Add("Mack.Chaves@contoso.com");
            meeting.RequiredAttendees.Add("Sadie.Daniels@contoso.com");
            meeting.OptionalAttendees.Add("Magdalena.Kemp@contoso.com");
            meeting.ReminderMinutesBeforeStart = 60;
            // Send the meeting request
            meeting.Save(SendInvitationsMode.SendToAllAndSaveCopy);

```

## <a name="calendar-folders-and-calendar-items"></a><span data-ttu-id="15917-116">Dossiers de calendrier et éléments de calendrier</span><span class="sxs-lookup"><span data-stu-id="15917-116">Calendar folders and calendar items</span></span>
<span data-ttu-id="15917-117"><a name="bk_CalendarFolder"> </a></span><span class="sxs-lookup"><span data-stu-id="15917-117"></span></span>

<span data-ttu-id="15917-p103">Les dossiers de calendrier contiennent des éléments de calendrier. Les dossiers de calendrier ont une [classe de dossier](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) de **IPF.Appointment**, et peuvent inclure uniquement les éléments définis par la propriété de l'API managée EWS [ItemClass](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx), qui est associée à un objet de [classe de rendez-vous](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx), ou à l'élément [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="15917-p103">Calendar folders contain calendar items. Calendar folders have a [folder class](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) of **IPF.Appointment**, and can include only the items defined by the [ItemClass](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx) EWS Managed API property, which is associated with an [Appointment Class](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object, or the EWS [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="15917-120">Les éléments d’un dossier de Calendrier sont légèrement différents des éléments d’autres dossiers dans une boîte aux lettres car les occurrences d’une série périodique et les exceptions à une série périodique ne sont pas des éléments réels dans la boîte aux lettres. Elles sont plutôt stockées en interne sous forme de pièces jointes à un rendez-vous périodique important.</span><span class="sxs-lookup"><span data-stu-id="15917-120">Items in a Calendar folder are a little different from items in other folders in a mailbox because occurrences in a recurring series and exceptions to a recurring series are not actual items in the mailbox, but rather are stored internally as attachments to a recurring master. Therefore, in order to retrieve all appointments in a given date range, you need to use a calendar view. To learn more about retrieving appointments and calendar views, see How to: Get appointments and meetings by using EWS in Exchange.</span></span> <span data-ttu-id="15917-121">Par conséquent, pour récupérer tous les rendez-vous sur une plage de dates donnée, vous devez utiliser un affichage calendrier.</span><span class="sxs-lookup"><span data-stu-id="15917-121">Therefore, in order to retrieve all appointments in a given date range, you need to use a calendar view.</span></span> <span data-ttu-id="15917-122">Pour en savoir plus sur la récupération des rendez-vous et des affichages de calendrier, voir[Créer des rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md). </span><span class="sxs-lookup"><span data-stu-id="15917-122">To learn more about retrieving appointments and calendar views, see [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="meetings-and-appointments"></a><span data-ttu-id="15917-123">Réunions et rendez-vous</span><span class="sxs-lookup"><span data-stu-id="15917-123">Meetings and appointments</span></span>
<span data-ttu-id="15917-124"><a name="bk_meetings"> </a></span><span class="sxs-lookup"><span data-stu-id="15917-124"></span></span>

<span data-ttu-id="15917-p105">La principale différence entre les réunions et les rendez-vous réside dans la présence de participants aux réunions, mais pas aux rendez-vous. En interne, Exchange utilise le même objet pour les réunions et pour les rendez-vous. Pour utiliser les réunions et les rendez-vous, vous devez utiliser la [classe de rendez-vous](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) de l'API managée EWS ou l'élément [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) d'EWS.</span><span class="sxs-lookup"><span data-stu-id="15917-p105">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't. Internally, Exchange uses the same object for both meetings and appointments. You use the EWS Managed API [Appointment class](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="15917-128">Les rendez-vous et les réunions peuvent être des instances uniques ou faire partie d'une [série périodique](recurrence-patterns-and-ews.md). Cependant, les rendez-vous n'incluant ni participants, ni salles, ni ressources, ne nécessitent pas l'envoi d'un message.</span><span class="sxs-lookup"><span data-stu-id="15917-128">Both appointments and meetings can be single instances or part of a [recurring series](recurrence-patterns-and-ews.md), but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent.</span></span>
  
<span data-ttu-id="15917-p106">Étant donné que les réunions incluent l'envoi et la réponse à des demandes et des mises à jour, elles impliquent plus que le simple accès à des éléments dans un dossier de calendrier. Elles ont également un flux de travail associé. Les réunions doivent être planifiées lorsque les participants sont disponibles et peuvent également impliquer la réservation d'une salle de réunion ou de ressources comme un projecteur ou d'autres appareils.</span><span class="sxs-lookup"><span data-stu-id="15917-p106">Because meetings include sending and responding to requests and updates, they involve more than just accessing items in a Calendar folder. They also have an associated workflow. Meetings must be scheduled when attendees are available, and can also involve reserving a meeting room, or resources such as a projector or other equipment.</span></span>
  
<span data-ttu-id="15917-132">Le flux de travail d’une réunion comprend généralement les étapes suivantes :</span><span class="sxs-lookup"><span data-stu-id="15917-132">The meeting workflow typically involves the following steps:</span></span>
  
1. <span data-ttu-id="15917-133">Une réunion est créée et renseignée avec des informations telles que l’heure de début et de fin, l’emplacement et un corps de message.</span><span class="sxs-lookup"><span data-stu-id="15917-133">A meeting is created and populated with information such as start and end time, location, and a message body.</span></span>
    
2. <span data-ttu-id="15917-134">Une liste de participants, ressources et salles potentiels est créée.</span><span class="sxs-lookup"><span data-stu-id="15917-134">A list of prospective attendees, resources, and rooms is created.</span></span>
    
3. <span data-ttu-id="15917-135">Le statut de disponibilité des participants est vérifié.</span><span class="sxs-lookup"><span data-stu-id="15917-135">The availability status of attendees is checked.</span></span> 
    
4. <span data-ttu-id="15917-136">Une demande de réunion est envoyée aux participants.</span><span class="sxs-lookup"><span data-stu-id="15917-136">A meeting request is sent to attendees.</span></span>
    
5. <span data-ttu-id="15917-p107">Les participantes répondent à la réunion avec leur intention de participer ou non. Les participants peuvent également proposer une nouvelle heure pour la réunion.</span><span class="sxs-lookup"><span data-stu-id="15917-p107">Attendees reply to the meeting with their intention to attend or not. Attendees may also propose a new time for the meeting.</span></span>
    
6. <span data-ttu-id="15917-139">Les réunions peuvent être annulées ou mises à jour, ce qui déclenche généralement l’envoi de nouveaux messages aux participants.</span><span class="sxs-lookup"><span data-stu-id="15917-139">Meetings can be canceled or updated, which typically trigger new messages to be sent to attendees.</span></span>
    
## <a name="calendars-and-time"></a><span data-ttu-id="15917-140">Calendriers et heure</span><span class="sxs-lookup"><span data-stu-id="15917-140">Calendars and time</span></span>
<span data-ttu-id="15917-141"><a name="bk_Time"> </a></span><span class="sxs-lookup"><span data-stu-id="15917-141"></span></span>

<span data-ttu-id="15917-p108">Les fonctionnalités liées à l'heure font partie intégrante du calendrier. Les rendez-vous et les réunions ont des heures de début et de fin, des durées et d'autres propriétés liées à l'heure, telles que l'heure à laquelle un message est créé, envoyé et reçu. Les réunions et rendez-vous existants peuvent être récupérés à partir d'un dossier Calendrier sur la base d'une heure de début et de fin. Les séries périodiques ont des débuts et des fins. Et les réunions ont lieu dans un fuseau horaire donné, ce qui est de plus en plus important dans une économie mondiale.</span><span class="sxs-lookup"><span data-stu-id="15917-p108">Time-related functionality is integral to calendaring. Appointments and meetings have start and end times, durations, and other time-related properties, such as the time at which a message is created, sent, and received. Existing appointments and meetings can be retrieved from a Calendar folder based on a start and end time. Recurring series have beginnings and ends. And meetings occur within a given time zone, which is increasingly important in a global economy.</span></span>
  
<span data-ttu-id="15917-p109">Les heures sont stockées en interne sur un serveur Exchange en Temps universel coordonné (UTC). Exchange les convertit en heures locales en fonction des paramètres du client. Les propriétés [DateTime](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) sont limitées au fuseau horaire local de l'ordinateur.</span><span class="sxs-lookup"><span data-stu-id="15917-p109">Times are stored internally on an Exchange server in Coordinated Universal Time (UTC). Exchange converts them to local time zone based on client settings. [DateTime](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) properties are scoped to the computer's local time zone.</span></span> 
  
## <a name="recurring-series"></a><span data-ttu-id="15917-150">Séries périodiques</span><span class="sxs-lookup"><span data-stu-id="15917-150">Recurring series</span></span>
<span data-ttu-id="15917-151"><a name="bk_recurrence"> </a></span><span class="sxs-lookup"><span data-stu-id="15917-151"></span></span>

<span data-ttu-id="15917-p110">Une série périodique de réunions ou de rendez-vous est constituée d'un rendez-vous ou réunion périodique important(e), d'un ensemble d'éléments d'occurrence et, éventuellement, d'un ensemble d'éléments d'exception. Les informations de périodicité sont stockées sur l'élément de rendez-vous périodique important. L'élément EWS [RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) est associé à des occurrences et des exceptions dans une série, ou vous pouvez utiliser la méthode d'API managée EWS [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/fr-FR/library/dd635978%28v=EXCHG.80%29.aspx) pour récupérer le rendez-vous périodique important. À l'aide d'une instance d'une série, vous pouvez trouver tous les éléments et les informations associés à la série.</span><span class="sxs-lookup"><span data-stu-id="15917-p110">A recurring series of appointments or meetings is comprised of a recurring master, a set of occurrence items, and optionally, a set of exception items. Recurrence information is stored on the recurring master item. The [RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) EWS element is associated with occurrences and exceptions in a series, or you can use the [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/fr-FR/library/dd635978%28v=EXCHG.80%29.aspx) EWS Managed API method to get the recurring master. Using an instance of a series, you can find all the elements and information associated with the series.</span></span> 
  
<span data-ttu-id="15917-p111">Notez que les propriétés de périodicité existent sur tous les éléments de calendrier, mais elles sont renseignées uniquement sur les éléments de rendez-vous périodiques importants. Outre un index de toutes les occurrences d'une série, le rendez-vous périodique important a une référence à des occurrences modifiées et supprimées et à la périodicité d'une série (par exemple, quotidien, hebdomadaire, mensuel ou annuel).</span><span class="sxs-lookup"><span data-stu-id="15917-p111">Note that recurrence properties exist on all calendar items, but they are populated only on recurring master items. In addition to an index of all occurrences in a series, the recurring master has a reference to modified and deleted occurrences and the recurrence pattern of a series (for example, daily, weekly, monthly, or yearly).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="15917-158">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="15917-158">In this section</span></span>
<span data-ttu-id="15917-159"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="15917-159"></span></span>

- [<span data-ttu-id="15917-160">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="15917-160">How to: Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="15917-161">Créer des événements sur une journée entière à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-161">How to: Create all-day events by using EWS in Exchange</span></span>](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="15917-162">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-162">How to: Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="15917-163">Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-163">How to: Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="15917-164">Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-164">How to: Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="15917-165">Obtenir les listes de salle à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-165">How to: Get room lists by using EWS in Exchange</span></span>](how-to-get-room-lists-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="15917-166">Obtenir des informations de disponibilité à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-166">How to: Get free/busy information by using EWS in Exchange</span></span>](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="15917-167">Proposer une nouvelle heure de réunion à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-167">How to: Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="15917-168">Traiter les éléments de calendrier par lots dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-168">How to: Process calendar items in batches in Exchange</span></span>](how-to-process-calendar-items-in-batches-in-exchange.md)
    
- [<span data-ttu-id="15917-169">Périodicités et EWS</span><span class="sxs-lookup"><span data-stu-id="15917-169">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
## <a name="see-also"></a><span data-ttu-id="15917-170">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="15917-170">See also</span></span>


- [<span data-ttu-id="15917-171">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-171">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="15917-172">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-172">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="15917-173">Vue d'ensemble de la conception client EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="15917-173">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

