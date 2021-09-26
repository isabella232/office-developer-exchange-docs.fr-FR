---
title: Opération GetUserAvailability
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetUserAvailability
api_type:
- schema
ms.assetid: 8da17226-5d3a-4525-9ffa-d83730f47bb1
description: Trouvez des informations sur l’opération GetUserAvailability EWS.
ms.openlocfilehash: fcd222dfc98df3c12bdd6035e585f620e0a6d9f5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547503"
---
# <a name="getuseravailability-operation"></a>Opération GetUserAvailability

Trouvez des informations sur **l’opération GetUserAvailability** EWS. 
  
**L’opération GetUserAvailability** fournit des informations détaillées sur la disponibilité d’un ensemble d’utilisateurs, de salles et de ressources sur une période spécifiée. 
  
## <a name="using-the-getuseravailability-operation"></a>Utilisation de l’opération GetUserAvailability

**L’opération GetUserAvailability** fournit les informations de disponibilité utilisateur actuelles à un niveau de détail spécifié. Les applications clientes telles que Outlook, Outlook Web Access, Outlook Mobile Access et d’autres utilisent des adresses SMTP pour identifier les informations utilisateur demandées. 
  
Le service de disponibilité développe les listes de distribution pour récupérer l’état de disponibilité de chaque membre de la liste, tant que le nombre de boîtes aux lettres dans la liste de distribution est inférieur à 100, ce qui est le nombre maximal d’identités que l’opération **GetUserAvailability** peut demander. Les statuts de libre/occupé des membres de la liste de distribution sont fusionnés en un seul statut de libre/occupé pour l’ensemble de la liste de distribution. 
  
Les demandes d’application client spécifient la période de la requête de disponibilité. La période par défaut pour les informations demandées est de 42 jours. Si le calendrier de l’utilisateur contient des rendez-vous ou des réunions qui sont à la fois au sein de la période définie et en dehors de la période définie pour la requête, le rendez-vous est renvoyé. 
  
Les heures de rendez-vous et de réunion renvoyées sont dans le même fuseau horaire que l’application cliente qui demande la réunion.
  
Le service de disponibilité traite la demande pour chaque client. Le service développe tous les rendez-vous périodiques et renvoie le nombre maximal de détails de calendrier que le client demandeur est autorisé à recevoir.
  
> [!NOTE]
> Si la boîte aux lettres cible est indisponible ou est introuvable, une exception **MailRecipientNotFoundException** est envoyée. Le client reçoit un message d’erreur qui indique que le destinataire du message est in trouvé dans le service d’annuaire Active Directory ou les services de domaine Active Directory (AD DS). 
  
### <a name="getuseravailability-operation-soap-headers"></a>En-têtes SOAP de l’opération GetUserAvailability

**L’opération GetUserAvailability** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur dont le client usurpe l’identité. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Spécifie un en-tête SOAP qui identifie le fuseau horaire à utiliser pour toutes les réponses du serveur. Toutes les heures renvoyées par le serveur sont converties en fuseau horaire spécifié. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a>Exemple de requête GetUserAvailability : obtenir des informations de disponibilité

L’exemple suivant d’une demande d’opération **GetUserAvailability** montre comment obtenir des informations de disponibilité détaillées pour deux utilisateurs dans le fuseau horaire Pacifique. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <t:TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

Pour plus d’informations sur la récupération de réunions suggérées à l’aide de l’élément [SuggestionsViewOptions,](suggestionsviewoptions.md) voir le schéma dans le répertoire virtuel EWS. 
  
Le corps SOAP de la requête contient les éléments suivants :
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
    
- [TimeZone (Availability)](timezone-availability.md)
    
- [Bias (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Bias](bias.md)
    
- [Time](time.md)
    
- [DayOrder](dayorder.md)
    
- [Month](month.md)
    
- [DayOfWeek (TimeZone)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [MailboxDataArray](mailboxdataarray.md)
    
- [MailboxData](mailboxdata.md)
    
- [Email (EmailAddressType)](email-emailaddresstype.md)
    
- [Address (String)](address-string.md)
    
- [AttendeeType](attendeetype.md)
    
- [ExcludeConflicts](excludeconflicts.md)
    
- [FreeBusyViewOptions](freebusyviewoptions.md)
    
- [TimeWindow](timewindow.md)
    
- [StartTime](starttime.md)
    
- [EndTime](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a>Réponse réussie de l’opération GetUserAvailability

L’exemple suivant montre une réponse réussie à la demande d’opération **GetUserAvailability.** 
  
> [!NOTE]
> Les identificateurs d’événements de calendrier ont été raccourcis pour préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="665" MinorBuildNumber="7" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserAvailabilityResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FreeBusyResponseArray>
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">DetailedMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="https://schemas.microsoft.com/exchange/services/2006/types">000002220220000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <WorkingHours xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <FreeBusyViewType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">FreeBusyMerged</FreeBusyViewType>
            <MergedFreeBusy xmlns="https://schemas.microsoft.com/exchange/services/2006/types">000000001100000000000000</MergedFreeBusy>
            <CalendarEventArray xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2006-10-16T09:00:00-07:00</StartTime>
                <EndTime>2006-10-16T10:00:00-07:00</EndTime>
                <BusyType>Tentative</BusyType>
              </CalendarEvent>
            </CalendarEventArray>
            <WorkingHours xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

Les informations de disponibilité de chaque utilisateur apparaissent dans un [élément FreeBusyResponse](freebusyresponse.md) unique. L’ordre des utilisateurs dans la **demande d’opération GetUserAvailability** détermine l’ordre des données de disponibilité pour chaque utilisateur dans la réponse. 
  
Une erreur est renvoyée au client si le nombre de rendez-vous dans la période définie dans la requête est supérieur au nombre maximal spécifié par l’administrateur. Le nombre maximal de rendez-vous par défaut est de 10 000 instances et d’éléments de récurrence étendus. Cette propriété ne peut être configurée que par un administrateur.
  
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
    
- [StartTime](starttime.md)
    
- [EndTime](endtime.md)
    
- [BusyType](busytype.md)
    
- [CalendarEventDetails](calendareventdetails.md)
    
- [ID](id.md)
    
- [Subject (CalendarEventDetails)](subject-calendareventdetails.md)
    
- [Location (CalendarEventDetails)](location-calendareventdetails.md)
    
- [IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md)
    
- [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md)
    
- [IsException](isexception.md)
    
- [IsReminderSet](isreminderset.md)
    
- [IsPrivate](isprivate.md)
    
- [WorkingHours](workinghours-ex15websvcsotherref.md)
    
- [TimeZone (Availability)](timezone-availability.md)
    
- [Bias (UTC)](bias-utc.md)
    
- [StandardTime](standardtime.md)
    
- [Bias](bias.md)
    
- [Time](time.md)
    
- [DayOrder](dayorder.md)
    
- [Month](month.md)
    
- [DayOfWeek (TimeZone)](dayofweek-timezone.md)
    
- [DaylightTime](daylighttime.md)
    
- [WorkingPeriodArray](workingperiodarray.md)
    
- [WorkingPeriod](workingperiod.md)
    
- [DayOfWeek (WorkingPeriod)](dayofweek-workingperiod.md)
    
- [StartTimeInMinutes](starttimeinminutes.md)
    
- [EndTimeInMinutes](endtimeinminutes.md)
    
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    

