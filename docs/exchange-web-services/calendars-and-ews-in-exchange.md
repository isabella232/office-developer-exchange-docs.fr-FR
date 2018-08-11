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
# <a name="calendars-and-ews-in-exchange"></a>Calendriers et EWS dans Exchange

Découvrez les calendriers, les dossiers et les éléments de calendrier, les rendez-vous et les réunions dans Exchange.
  
Vous êtes probablement familiarisé avec de nombreuses fonctionnalités de calendrier des clients de messagerie comme Outlook, qui vous permettent d’effectuer le suivi de rendez-vous, de planifier des réunions, de vérifier la disponibilité de personnes, d’inviter des participants et de modifier ou d’annuler les réunions.
  
Les fonctionnalités de calendrier dans Exchange sont légèrement différentes de celles que vous voyez dans un client comme Outlook. Au lieu d'afficher des informations, EWS dans Exchange vous permet d'effectuer des actions comme créer, stocker, envoyer ou modifier des informations. Pour utiliser EWS avec des calendriers, vous devez être familiarisé avec des concepts tels que le stockage d'informations, l'heure, la périodicité et le flux de messages. Plus spécifiquement, vous devez être familiarisé avec les éléments suivants :
  
- Dossiers de calendrier, éléments de calendrier et affichages de calendrier
    
- Demandes de réunion, réponses, planification, participants, ressources, salles et disponibilité
    
- Durées, fuseaux horaires et heures de début et de fin des réunions et rendez-vous
    
- Séries périodiques, périodicités, exceptions et rendez-vous et réunions uniques
    
Heureusement, EWS et l'API managée EWS fournissent un large éventail d'opérations et de méthodes qui vous permettent d'effectuer un large éventail de tâches de calendrier. Par exemple, à l'aide de l'API managée EWS, vous pouvez créer une réunion et envoyer des invitations aux participants avec simplement quelques lignes de code, comme illustré dans l'exemple suivant.
  
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

## <a name="calendar-folders-and-calendar-items"></a>Dossiers de calendrier et éléments de calendrier
<a name="bk_CalendarFolder"> </a>

Les dossiers de calendrier contiennent des éléments de calendrier. Les dossiers de calendrier ont une [classe de dossier](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) de **IPF.Appointment**, et peuvent inclure uniquement les éléments définis par la propriété de l'API managée EWS [ItemClass](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.item.itemclass%28v=exchg.80%29.aspx), qui est associée à un objet de [classe de rendez-vous](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx), ou à l'élément [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) EWS. 
  
Les éléments d’un dossier de Calendrier sont légèrement différents des éléments d’autres dossiers dans une boîte aux lettres car les occurrences d’une série périodique et les exceptions à une série périodique ne sont pas des éléments réels dans la boîte aux lettres. Elles sont plutôt stockées en interne sous forme de pièces jointes à un rendez-vous périodique important. Par conséquent, pour récupérer tous les rendez-vous sur une plage de dates donnée, vous devez utiliser un affichage calendrier. Pour en savoir plus sur la récupération des rendez-vous et des affichages de calendrier, voir[Créer des rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md). 
  
## <a name="meetings-and-appointments"></a>Réunions et rendez-vous
<a name="bk_meetings"> </a>

La principale différence entre les réunions et les rendez-vous réside dans la présence de participants aux réunions, mais pas aux rendez-vous. En interne, Exchange utilise le même objet pour les réunions et pour les rendez-vous. Pour utiliser les réunions et les rendez-vous, vous devez utiliser la [classe de rendez-vous](http://msdn.microsoft.com/fr-FR/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) de l'API managée EWS ou l'élément [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) d'EWS. 
  
Les rendez-vous et les réunions peuvent être des instances uniques ou faire partie d'une [série périodique](recurrence-patterns-and-ews.md). Cependant, les rendez-vous n'incluant ni participants, ni salles, ni ressources, ne nécessitent pas l'envoi d'un message.
  
Étant donné que les réunions incluent l'envoi et la réponse à des demandes et des mises à jour, elles impliquent plus que le simple accès à des éléments dans un dossier de calendrier. Elles ont également un flux de travail associé. Les réunions doivent être planifiées lorsque les participants sont disponibles et peuvent également impliquer la réservation d'une salle de réunion ou de ressources comme un projecteur ou d'autres appareils.
  
Le flux de travail d’une réunion comprend généralement les étapes suivantes :
  
1. Une réunion est créée et renseignée avec des informations telles que l’heure de début et de fin, l’emplacement et un corps de message.
    
2. Une liste de participants, ressources et salles potentiels est créée.
    
3. Le statut de disponibilité des participants est vérifié. 
    
4. Une demande de réunion est envoyée aux participants.
    
5. Les participantes répondent à la réunion avec leur intention de participer ou non. Les participants peuvent également proposer une nouvelle heure pour la réunion.
    
6. Les réunions peuvent être annulées ou mises à jour, ce qui déclenche généralement l’envoi de nouveaux messages aux participants.
    
## <a name="calendars-and-time"></a>Calendriers et heure
<a name="bk_Time"> </a>

Les fonctionnalités liées à l'heure font partie intégrante du calendrier. Les rendez-vous et les réunions ont des heures de début et de fin, des durées et d'autres propriétés liées à l'heure, telles que l'heure à laquelle un message est créé, envoyé et reçu. Les réunions et rendez-vous existants peuvent être récupérés à partir d'un dossier Calendrier sur la base d'une heure de début et de fin. Les séries périodiques ont des débuts et des fins. Et les réunions ont lieu dans un fuseau horaire donné, ce qui est de plus en plus important dans une économie mondiale.
  
Les heures sont stockées en interne sur un serveur Exchange en Temps universel coordonné (UTC). Exchange les convertit en heures locales en fonction des paramètres du client. Les propriétés [DateTime](http://msdn.microsoft.com/library/9c6ecd4c-779c-4fa5-8082-dd2bc0a751f4%28Office.15%29.aspx) sont limitées au fuseau horaire local de l'ordinateur. 
  
## <a name="recurring-series"></a>Séries périodiques
<a name="bk_recurrence"> </a>

Une série périodique de réunions ou de rendez-vous est constituée d'un rendez-vous ou réunion périodique important(e), d'un ensemble d'éléments d'occurrence et, éventuellement, d'un ensemble d'éléments d'exception. Les informations de périodicité sont stockées sur l'élément de rendez-vous périodique important. L'élément EWS [RecurringMasterItemId](http://msdn.microsoft.com/library/5800b58c-f3d7-4d8f-acc0-d13e02f4e258%28Office.15%29.aspx) est associé à des occurrences et des exceptions dans une série, ou vous pouvez utiliser la méthode d'API managée EWS [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/fr-FR/library/dd635978%28v=EXCHG.80%29.aspx) pour récupérer le rendez-vous périodique important. À l'aide d'une instance d'une série, vous pouvez trouver tous les éléments et les informations associés à la série. 
  
Notez que les propriétés de périodicité existent sur tous les éléments de calendrier, mais elles sont renseignées uniquement sur les éléments de rendez-vous périodiques importants. Outre un index de toutes les occurrences d'une série, le rendez-vous périodique important a une référence à des occurrences modifiées et supprimées et à la périodicité d'une série (par exemple, quotidien, hebdomadaire, mensuel ou annuel).
  
## <a name="in-this-section"></a>Dans cette section
<a name="bk_inthissection"> </a>

- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Créer des événements sur une journée entière à l'aide d’EWS dans Exchange](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [Obtenir les listes de salle à l'aide d’EWS dans Exchange](how-to-get-room-lists-by-using-ews-in-exchange.md)
    
- [Obtenir des informations de disponibilité à l'aide d’EWS dans Exchange](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [Proposer une nouvelle heure de réunion à l'aide d’EWS dans Exchange](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    
- [Traiter les éléments de calendrier par lots dans Exchange](how-to-process-calendar-items-in-batches-in-exchange.md)
    
- [Périodicités et EWS](recurrence-patterns-and-ews.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Commencer à utiliser les services web dans Exchange](start-using-web-services-in-exchange.md)
    
- [Vue d'ensemble de la conception client EWS pour Exchange](ews-client-design-overview-for-exchange.md)
    

