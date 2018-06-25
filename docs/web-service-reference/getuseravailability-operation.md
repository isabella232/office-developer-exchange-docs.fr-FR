---
title: Opération GetUserAvailability
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailability
api_type:
- schema
ms.assetid: 8da17226-5d3a-4525-9ffa-d83730f47bb1
description: Opération de recherche plus d’informations sur la GetUserAvailability EWS.
ms.openlocfilehash: 41246fe22bfb7444cd4aa7b1d4651d475dd9231c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827686"
---
# <a name="getuseravailability-operation"></a>Opération GetUserAvailability

Trouvez des informations sur l’opération EWS **GetUserAvailability** . 
  
L’opération **GetUserAvailability** fournit des informations détaillées sur la disponibilité d’un ensemble d’utilisateurs, les salles et les ressources dans une période spécifiée. 
  
## <a name="using-the-getuseravailability-operation"></a>Utilisation de l’opération GetUserAvailability

L’opération **GetUserAvailability** fournit des informations de disponibilité utilisateur actif à un niveau de détail spécifié. Applications clientes comme Outlook, Outlook Web Access, Outlook Mobile Access et d’autres personnes les adresses SMTP permet d’identifier les informations de l’utilisateur demandé. 
  
Le service de disponibilité développe les listes de distribution pour récupérer l’état de disponibilité de chaque membre de la liste, dans la mesure où le nombre de boîtes aux lettres dans la liste de distribution est inférieur à 100, qui est le nombre maximal d’identités qui le **GetUserAvailability **opération peut demander. Les statuts et de disponibilité des membres de la liste de distribution sont fusionnés dans un état libre/occupé unique pour la liste de distribution entière. 
  
Demandes des applications clientes spécifient la période de temps de la requête de disponibilité. Période de temps pour les informations demandées par défaut est de 42 jours. Si le calendrier de l’utilisateur contient des rendez-vous ou réunions qui se trouvent au sein et en dehors de la période définie pour la requête, le rendez-vous est renvoyé. 
  
Les heures de rendez-vous et de réunion qui sont retournés sont dans le même fuseau horaire en tant que l’application cliente qui demande la réunion.
  
Le service de disponibilité traite la demande pour chaque client. Le service développe tous les rendez-vous périodiques et renvoie le nombre maximal de détails du calendrier qui le client demande est autorisé à recevoir.
  
> [!NOTE]
> Si la boîte aux lettres cible n’est pas disponible ou est introuvable, une exception **MailRecipientNotFoundException** est levée. Le client reçoit un message d’erreur indiquant que le destinataire est introuvable dans le service d’annuaire Active Directory ou les Services de domaine Active Directory (AD DS). 
  
### <a name="getuseravailability-operation-soap-headers"></a>En-têtes SOAP d’opération GetUserAvailability

L’opération **GetUserAvailability** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur auquel le client est l’emprunt d’identité. Cet en-tête est applicable à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Spécifie un en-tête SOAP qui identifie le fuseau horaire à utiliser pour toutes les réponses à partir du serveur. Toutes les heures qui sont renvoyés à partir du serveur seront convertis dans le fuseau horaire spécifié. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a>Exemple de requête GetUserAvailability : obtenir des informations de disponibilité

Une demande d’opération **GetUserAvailability** l’exemple suivant montre comment obtenir des informations de disponibilité détaillées pour les deux utilisateurs dans le fuseau horaire Pacifique. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <t:TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Bias>480</Bias>
        <StandardTime>
          <Bias>0</Bias>
          <Time>02:00:00</Time>
          <DayOrder>5</DayOrder>
          <Month>10</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </StandardTime>
        <DaylightTime>
          <Bias>-60</Bias>
          <Time>02:00:00</Time>
          <DayOrder>1</DayOrder>
          <Month>4</Month>
          <DayOfWeek>Sunday</DayOfWeek>
        </DaylightTime>
      </t:TimeZone>
      <MailboxDataArray>
        <t:MailboxData>
          <t:Email>
            <t:Address>user1@example.com</t:Address>
          </t:Email>
          <t:AttendeeType>Required</t:AttendeeType>
          <t:ExcludeConflicts>false</t:ExcludeConflicts>
        </t:MailboxData>
        <t:MailboxData>
          <t:Email>
            <t:Address>user2@example.com</t:Address>
          </t:Email>
          <t:AttendeeType>Required</t:AttendeeType>
          <t:ExcludeConflicts>false</t:ExcludeConflicts>
        </t:MailboxData>
      </MailboxDataArray>
      <t:FreeBusyViewOptions>
        <t:TimeWindow>
          <t:StartTime>2006-10-16T00:00:00</t:StartTime>
          <t:EndTime>2006-10-16T23:59:59</t:EndTime>
        </t:TimeWindow>
        <t:MergedFreeBusyIntervalInMinutes>60</t:MergedFreeBusyIntervalInMinutes>
        <t:RequestedView>DetailedMerged</t:RequestedView>
      </t:FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

Pour plus d’informations sur la récupération des réunions proposées à l’aide de l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) , voir le schéma dans le répertoire virtuel EWS. 
  
La demande SOAP body contient les éléments suivants :
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
    
- [Fuseau horaire (disponibilité)](timezone-availability.md)
    
- [Bias (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Bias](bias.md)
    
- [Heure](time.md)
    
- [DayOrder](dayorder.md)
    
- [Mois](month.md)
    
- [DayOfWeek (fuseau horaire)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [MailboxDataArray](mailboxdataarray.md)
    
- [MailboxData](mailboxdata.md)
    
- [Courrier électronique (EmailAddressType)](email-emailaddresstype.md)
    
- [Adresse (chaîne)](address-string.md)
    
- [AttendeeType](attendeetype.md)
    
- [ExcludeConflicts](excludeconflicts.md)
    
- [FreeBusyViewOptions](freebusyviewoptions.md)
    
- [Durée](timewindow.md)
    
- [Heure de début](starttime.md)
    
- [Heure de fin](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a>Réponse d’opération GetUserAvailability réussie

L’exemple suivant montre une réponse positive à la requête d’opération **GetUserAvailability** . 
  
> [!NOTE]
> Les identificateurs d’événements de calendrier ont été réduits afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="665" MinorBuildNumber="7" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserAvailabilityResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FreeBusyResponseArray>
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">DetailedMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="http://schemas.microsoft.com/exchange/services/2006/types">000002220220000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2006-10-16T06:00:00-07:00</StartTime>
                <EndTime>2006-10-16T06:30:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>14B6414B0</ID>
                  <Subject>Meet with Contoso Account Executives</Subject>
                  <Location />
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
                </CalendarEventDetails>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2006-10-16T07:00:00-07:00</StartTime>
                <EndTime>2006-10-16T08:00:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>E14B6414B0B</ID>
                  <Subject>Pick up my groceries</Subject>
                  <Location />
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
                </CalendarEventDetails>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2006-10-16T09:40:00-07:00</StartTime>
                <EndTime>2006-10-16T10:10:00-07:00</EndTime>
                <BusyType>Busy</BusyType>
                <CalendarEventDetails>
                  <ID>14B6414B0B1</ID>
                  <Subject>Meet with doctor</Subject>
                  <Location>Kirkland</Location>
                  <IsMeeting>false</IsMeeting>
                  <IsRecurring>false</IsRecurring>
                  <IsException>false</IsException>
                  <IsReminderSet>false</IsReminderSet>
                  <IsPrivate>false</IsPrivate>
                </CalendarEventDetails>
              </CalendarEvent>
            </CalendarEventArray>
            <WorkingHours xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
              <TimeZone>
                <Bias>480</Bias>
                <StandardTime>
                  <Bias>0</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>5</DayOrder>
                  <Month>10</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </StandardTime>
                <DaylightTime>
                  <Bias>-60</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>1</DayOrder>
                  <Month>4</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </DaylightTime>
              </TimeZone>
              <WorkingPeriodArray>
                <WorkingPeriod>
                  <DayOfWeek>Monday Tuesday Wednesday Thursday Friday</DayOfWeek>
                  <StartTimeInMinutes>480</StartTimeInMinutes>
                  <EndTimeInMinutes>1020</EndTimeInMinutes>
                </WorkingPeriod>
              </WorkingPeriodArray>
            </WorkingHours>
          </FreeBusyView>
        </FreeBusyResponse>
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">FreeBusyMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="http://schemas.microsoft.com/exchange/services/2006/types">000000001100000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2006-10-16T09:00:00-07:00</StartTime>
                <EndTime>2006-10-16T10:00:00-07:00</EndTime>
                <BusyType>Tentative</BusyType>
              </CalendarEvent>
            </CalendarEventArray>
            <WorkingHours xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
              <TimeZone>
                <Bias>480</Bias>
                <StandardTime>
                  <Bias>0</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>5</DayOrder>
                  <Month>10</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </StandardTime>
                <DaylightTime>
                  <Bias>-60</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>1</DayOrder>
                  <Month>4</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </DaylightTime>
              </TimeZone>
              <WorkingPeriodArray>
                <WorkingPeriod>
                  <DayOfWeek>Monday Tuesday Wednesday Thursday Friday</DayOfWeek>
                  <StartTimeInMinutes>480</StartTimeInMinutes>
                  <EndTimeInMinutes>1020</EndTimeInMinutes>
                </WorkingPeriod>
              </WorkingPeriodArray>
            </WorkingHours>
          </FreeBusyView>
        </FreeBusyResponse>
      </FreeBusyResponseArray>
    </GetUserAvailabilityResponse>
  </soap:Body>
</soap:Envelope>
```

Les informations de disponibilité de chaque utilisateur s’affiche dans un élément [FreeBusyResponse](freebusyresponse.md) unique. L’ordre des utilisateurs dans la requête d’opération **GetUserAvailability** détermine l’ordre des données de disponibilité pour chaque utilisateur dans la réponse. 
  
Une erreur est renvoyée au client si le nombre de rendez-vous dans la période définie dans la requête est supérieur au nombre maximal spécifié par l’administrateur. Le nombre maximal par défaut de rendez-vous est de 10 000 instances uniques et développé des éléments de périodicité. Cette propriété peut être configurée uniquement par un administrateur.
  
Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
    
- [FreeBusyResponseArray](freebusyresponsearray.md)
    
- [FreeBusyResponse](freebusyresponse.md)
    
- [ResponseMessage](responsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [FreeBusyView](freebusyview.md)
    
- [FreeBusyViewType](freebusyviewtype.md)
    
- [MergedFreeBusy](mergedfreebusy.md)
    
- [CalendarEventArray](calendareventarray.md)
    
- [CalendarEvent](calendarevent.md)
    
- [Heure de début](starttime.md)
    
- [Heure de fin](endtime.md)
    
- [BusyType](busytype.md)
    
- [CalendarEventDetails](calendareventdetails.md)
    
- [ID](id.md)
    
- [Sujet (CalendarEventDetails)](subject-calendareventdetails.md)
    
- [Emplacement (CalendarEventDetails)](location-calendareventdetails.md)
    
- [IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md)
    
- [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md)
    
- [IsException](isexception.md)
    
- [IsReminderSet](isreminderset.md)
    
- [IsPrivate](isprivate.md)
    
- [WorkingHours](workinghours-ex15websvcsotherref.md)
    
- [Fuseau horaire (disponibilité)](timezone-availability.md)
    
- [Bias (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Bias](bias.md)
    
- [Heure](time.md)
    
- [DayOrder](dayorder.md)
    
- [Mois](month.md)
    
- [DayOfWeek (fuseau horaire)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [WorkingPeriodArray](workingperiodarray.md)
    
- [WorkingPeriod](workingperiod.md)
    
- [DayOfWeek (WorkingPeriod)](dayofweek-workingperiod.md)
    
- [StartTimeInMinutes](starttimeinminutes.md)
    
- [EndTimeInMinutes](endtimeinminutes.md)
    
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Obtention de disponibilité de l’utilisateur](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    

