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
description: Trouvez des informations sur l’opération EWS GetUserAvailability.
ms.openlocfilehash: b6d03c7da65e3f30f093b7e41448abcca2330a84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458221"
---
# <a name="getuseravailability-operation"></a><span data-ttu-id="538cc-103">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="538cc-103">GetUserAvailability operation</span></span>

<span data-ttu-id="538cc-104">Trouvez des informations sur l’opération EWS **GetUserAvailability** .</span><span class="sxs-lookup"><span data-stu-id="538cc-104">Find information about the **GetUserAvailability** EWS operation.</span></span> 
  
<span data-ttu-id="538cc-105">L’opération **GetUserAvailability** fournit des informations détaillées sur la disponibilité d’un ensemble d’utilisateurs, de salles et de ressources pendant une période spécifiée.</span><span class="sxs-lookup"><span data-stu-id="538cc-105">The **GetUserAvailability** operation provides detailed information about the availability of a set of users, rooms, and resources within a specified time period.</span></span> 
  
## <a name="using-the-getuseravailability-operation"></a><span data-ttu-id="538cc-106">Utilisation de l’opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="538cc-106">Using the GetUserAvailability operation</span></span>

<span data-ttu-id="538cc-107">L’opération **GetUserAvailability** fournit les informations de disponibilité de l’utilisateur actuel à un niveau de détail spécifié.</span><span class="sxs-lookup"><span data-stu-id="538cc-107">The **GetUserAvailability** operation provides current user availability information at a specified level of detail.</span></span> <span data-ttu-id="538cc-108">Les applications clientes telles qu’Outlook, Outlook Web Access, Outlook Mobile Access et d’autres utilisateurs utilisent des adresses SMTP pour identifier les informations utilisateur demandées.</span><span class="sxs-lookup"><span data-stu-id="538cc-108">Client applications such as Outlook, Outlook Web Access, Outlook Mobile Access, and others use SMTP addresses to identify the requested user information.</span></span> 
  
<span data-ttu-id="538cc-109">Le service de disponibilité développe les listes de distribution pour récupérer l’état de disponibilité de chaque membre de la liste, tant que le nombre de boîtes aux lettres dans la liste de distribution est inférieur à 100, ce qui correspond au nombre maximal d’identités que l’opération **GetUserAvailability** peut demander.</span><span class="sxs-lookup"><span data-stu-id="538cc-109">The Availability service expands distribution lists to retrieve the free/busy status for each member of the list, as long as the number of mailboxes in the distribution list is less than 100, which is the maximum number of identities that the **GetUserAvailability** operation can request.</span></span> <span data-ttu-id="538cc-110">Les États de disponibilité des membres de la liste de distribution sont fusionnés en un seul État de disponibilité pour l’ensemble de la liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="538cc-110">The free/busy statuses of the members of the distribution list are merged into a single free/busy status for the whole distribution list.</span></span> 
  
<span data-ttu-id="538cc-111">Demandes d’applications clientes spécifiez la période de la requête de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="538cc-111">Client application requests specify the time period of the availability query.</span></span> <span data-ttu-id="538cc-112">La période par défaut pour les informations demandées est de 42 jours.</span><span class="sxs-lookup"><span data-stu-id="538cc-112">The default time period for the requested information is 42 days.</span></span> <span data-ttu-id="538cc-113">Si le calendrier de l’utilisateur contient des rendez-vous ou des réunions à la fois à l’intérieur et à l’extérieur de la période définie pour la requête, le rendez-vous est renvoyé.</span><span class="sxs-lookup"><span data-stu-id="538cc-113">If the user's calendar contains appointments or meetings that are both within and outside the defined time period for the query, the appointment is returned.</span></span> 
  
<span data-ttu-id="538cc-114">Les heures de rendez-vous et de réunion renvoyées se situent dans le même fuseau horaire que l’application cliente qui demande la réunion.</span><span class="sxs-lookup"><span data-stu-id="538cc-114">The appointment and meeting times that are returned are in the same time zone as the client application that is requesting the meeting.</span></span>
  
<span data-ttu-id="538cc-115">Le service de disponibilité traite la demande pour chaque client.</span><span class="sxs-lookup"><span data-stu-id="538cc-115">The Availability service processes the request for each client.</span></span> <span data-ttu-id="538cc-116">Le service développe tous les rendez-vous périodiques et renvoie le nombre maximal de détails de calendrier que le client à l’origine de la demande est autorisé à recevoir.</span><span class="sxs-lookup"><span data-stu-id="538cc-116">The service expands all the recurring appointments and returns the maximum number of calendar details that the requesting client has permission to receive.</span></span>
  
> [!NOTE]
> <span data-ttu-id="538cc-117">Si la boîte aux lettres cible n’est pas disponible ou est introuvable, une exception **MailRecipientNotFoundException** est générée.</span><span class="sxs-lookup"><span data-stu-id="538cc-117">If the target mailbox is unavailable or cannot be found, a **MailRecipientNotFoundException** exception is thrown.</span></span> <span data-ttu-id="538cc-118">Le client reçoit un message d’erreur indiquant que le destinataire du message est introuvable dans le service d’annuaire Active Directory ou les services de domaine Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="538cc-118">The client receives an error message that states that the mail recipient is not found in the Active Directory directory service or Active Directory Domain Services (AD DS).</span></span> 
  
### <a name="getuseravailability-operation-soap-headers"></a><span data-ttu-id="538cc-119">En-têtes SOAP d’opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="538cc-119">GetUserAvailability operation SOAP headers</span></span>

<span data-ttu-id="538cc-120">L’opération **GetUserAvailability** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="538cc-120">The **GetUserAvailability** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="538cc-121">**Header**</span><span class="sxs-lookup"><span data-stu-id="538cc-121">**Header**</span></span>|<span data-ttu-id="538cc-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="538cc-122">**Element**</span></span>|<span data-ttu-id="538cc-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="538cc-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="538cc-124">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="538cc-124">**Impersonation**</span></span> <br/> |[<span data-ttu-id="538cc-125">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="538cc-125">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="538cc-126">Identifie l’utilisateur qui emprunte l’identité du client.</span><span class="sxs-lookup"><span data-stu-id="538cc-126">Identifies the user whom the client is impersonating.</span></span> <span data-ttu-id="538cc-127">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="538cc-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="538cc-128">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="538cc-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="538cc-129">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="538cc-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="538cc-130">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="538cc-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="538cc-131">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="538cc-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="538cc-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="538cc-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="538cc-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="538cc-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="538cc-134">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="538cc-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="538cc-135">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="538cc-135">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="538cc-136">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="538cc-136">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="538cc-137">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="538cc-137">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="538cc-138">Spécifie un en-tête SOAP qui identifie le fuseau horaire à utiliser pour toutes les réponses du serveur.</span><span class="sxs-lookup"><span data-stu-id="538cc-138">Specifies a SOAP header that identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="538cc-139">Toutes les heures qui sont retournées à partir du serveur seront converties dans le fuseau horaire spécifié.</span><span class="sxs-lookup"><span data-stu-id="538cc-139">All times that are returned from the server will be converted to the specified time zone.</span></span> <span data-ttu-id="538cc-140">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="538cc-140">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuseravailability-request-example-get-availability-information"></a><span data-ttu-id="538cc-141">Exemple de requête GetUserAvailability : obtenir des informations sur la disponibilité</span><span class="sxs-lookup"><span data-stu-id="538cc-141">GetUserAvailability request example: Get availability information</span></span>

<span data-ttu-id="538cc-142">L’exemple suivant de demande d’opération **GetUserAvailability** indique comment obtenir des informations de disponibilité détaillées pour deux utilisateurs dans le fuseau horaire Pacifique.</span><span class="sxs-lookup"><span data-stu-id="538cc-142">The following example of a **GetUserAvailability** operation request shows how to get detailed availability information for two users in the Pacific Time time zone.</span></span> 
  
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

<span data-ttu-id="538cc-143">Pour plus d’informations sur la récupération de réunions suggérées à l’aide de l’élément [SuggestionsViewOptions](suggestionsviewoptions.md) , consultez le schéma dans le répertoire virtuel EWS.</span><span class="sxs-lookup"><span data-stu-id="538cc-143">For more information about retrieving suggested meetings by using the [SuggestionsViewOptions](suggestionsviewoptions.md) element, see the schema in the EWS virtual directory.</span></span> 
  
<span data-ttu-id="538cc-144">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="538cc-144">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="538cc-145">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="538cc-145">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
    
- [<span data-ttu-id="538cc-146">TimeZone (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="538cc-146">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="538cc-147">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="538cc-147">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="538cc-148">StandardTime Element</span><span class="sxs-lookup"><span data-stu-id="538cc-148">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="538cc-149">Bias</span><span class="sxs-lookup"><span data-stu-id="538cc-149">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="538cc-150">Time</span><span class="sxs-lookup"><span data-stu-id="538cc-150">Time</span></span>](time.md)
    
- [<span data-ttu-id="538cc-151">DayOrder</span><span class="sxs-lookup"><span data-stu-id="538cc-151">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="538cc-152">Month</span><span class="sxs-lookup"><span data-stu-id="538cc-152">Month</span></span>](month.md)
    
- [<span data-ttu-id="538cc-153">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="538cc-153">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="538cc-154">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="538cc-154">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="538cc-155">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="538cc-155">MailboxDataArray</span></span>](mailboxdataarray.md)
    
- [<span data-ttu-id="538cc-156">MailboxData</span><span class="sxs-lookup"><span data-stu-id="538cc-156">MailboxData</span></span>](mailboxdata.md)
    
- [<span data-ttu-id="538cc-157">E-mail (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="538cc-157">Email (EmailAddressType)</span></span>](email-emailaddresstype.md)
    
- [<span data-ttu-id="538cc-158">Address (chaîne)</span><span class="sxs-lookup"><span data-stu-id="538cc-158">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="538cc-159">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="538cc-159">AttendeeType</span></span>](attendeetype.md)
    
- [<span data-ttu-id="538cc-160">ExcludeConflicts</span><span class="sxs-lookup"><span data-stu-id="538cc-160">ExcludeConflicts</span></span>](excludeconflicts.md)
    
- [<span data-ttu-id="538cc-161">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="538cc-161">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
    
- [<span data-ttu-id="538cc-162">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="538cc-162">TimeWindow</span></span>](timewindow.md)
    
- [<span data-ttu-id="538cc-163">StartTime</span><span class="sxs-lookup"><span data-stu-id="538cc-163">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="538cc-164">EndTime</span><span class="sxs-lookup"><span data-stu-id="538cc-164">EndTime</span></span>](endtime.md)
    
## <a name="successful-getuseravailability-operation-response"></a><span data-ttu-id="538cc-165">Réponse de l’opération GetUserAvailability réussie</span><span class="sxs-lookup"><span data-stu-id="538cc-165">Successful GetUserAvailability operation response</span></span>

<span data-ttu-id="538cc-166">L’exemple suivant montre une réponse réussie à la demande d’opération **GetUserAvailability** .</span><span class="sxs-lookup"><span data-stu-id="538cc-166">The following example shows a successful response to the **GetUserAvailability** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="538cc-167">Les identificateurs d’événements de calendrier ont été raccourcis pour conserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="538cc-167">The calendar event identifiers have been shortened to preserve readability.</span></span> 
  
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

<span data-ttu-id="538cc-168">Les informations de disponibilité de chaque utilisateur apparaissent dans un élément [FreeBusyResponse](freebusyresponse.md) unique.</span><span class="sxs-lookup"><span data-stu-id="538cc-168">The availability information for each user appears in a unique [FreeBusyResponse](freebusyresponse.md) element.</span></span> <span data-ttu-id="538cc-169">L’ordre des utilisateurs dans la demande d’opération **GetUserAvailability** détermine l’ordre des données de disponibilité pour chaque utilisateur dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="538cc-169">The order of users in the **GetUserAvailability** operation request determines the order of availability data for each user in the response.</span></span> 
  
<span data-ttu-id="538cc-170">Une erreur est renvoyée au client si le nombre de rendez-vous de la période définie dans la requête est supérieur au nombre maximal spécifié par l’administrateur.</span><span class="sxs-lookup"><span data-stu-id="538cc-170">An error will be returned to the client if the number of appointments in the time period that is defined in the query is greater than the administrator-specified maximum number.</span></span> <span data-ttu-id="538cc-171">Le nombre maximal par défaut de rendez-vous est de 10 000 instances uniques et des éléments de récurrence étendus.</span><span class="sxs-lookup"><span data-stu-id="538cc-171">The default maximum number of appointments is 10,000 single instances and expanded recurrence items.</span></span> <span data-ttu-id="538cc-172">Cette propriété ne peut être configurée que par un administrateur.</span><span class="sxs-lookup"><span data-stu-id="538cc-172">This property can be configured only by an administrator.</span></span>
  
<span data-ttu-id="538cc-173">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="538cc-173">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="538cc-174">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="538cc-174">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="538cc-175">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="538cc-175">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
    
- [<span data-ttu-id="538cc-176">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="538cc-176">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
    
- [<span data-ttu-id="538cc-177">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="538cc-177">FreeBusyResponse</span></span>](freebusyresponse.md)
    
- [<span data-ttu-id="538cc-178">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="538cc-178">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="538cc-179">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="538cc-179">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="538cc-180">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="538cc-180">FreeBusyView</span></span>](freebusyview.md)
    
- [<span data-ttu-id="538cc-181">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="538cc-181">FreeBusyViewType</span></span>](freebusyviewtype.md)
    
- [<span data-ttu-id="538cc-182">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="538cc-182">MergedFreeBusy</span></span>](mergedfreebusy.md)
    
- [<span data-ttu-id="538cc-183">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="538cc-183">CalendarEventArray</span></span>](calendareventarray.md)
    
- [<span data-ttu-id="538cc-184">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="538cc-184">CalendarEvent</span></span>](calendarevent.md)
    
- [<span data-ttu-id="538cc-185">StartTime</span><span class="sxs-lookup"><span data-stu-id="538cc-185">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="538cc-186">EndTime</span><span class="sxs-lookup"><span data-stu-id="538cc-186">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="538cc-187">BusyType</span><span class="sxs-lookup"><span data-stu-id="538cc-187">BusyType</span></span>](busytype.md)
    
- [<span data-ttu-id="538cc-188">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="538cc-188">CalendarEventDetails</span></span>](calendareventdetails.md)
    
- [<span data-ttu-id="538cc-189">ID</span><span class="sxs-lookup"><span data-stu-id="538cc-189">ID</span></span>](id.md)
    
- [<span data-ttu-id="538cc-190">Subject (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="538cc-190">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md)
    
- [<span data-ttu-id="538cc-191">Emplacement (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="538cc-191">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
    
- [<span data-ttu-id="538cc-192">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="538cc-192">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
    
- [<span data-ttu-id="538cc-193">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="538cc-193">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
    
- [<span data-ttu-id="538cc-194">IsException</span><span class="sxs-lookup"><span data-stu-id="538cc-194">IsException</span></span>](isexception.md)
    
- [<span data-ttu-id="538cc-195">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="538cc-195">IsReminderSet</span></span>](isreminderset.md)
    
- [<span data-ttu-id="538cc-196">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="538cc-196">IsPrivate</span></span>](isprivate.md)
    
- [<span data-ttu-id="538cc-197">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="538cc-197">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
    
- [<span data-ttu-id="538cc-198">TimeZone (disponibilité)</span><span class="sxs-lookup"><span data-stu-id="538cc-198">TimeZone (Availability)</span></span>](timezone-availability.md)
    
- [<span data-ttu-id="538cc-199">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="538cc-199">Bias (UTC)</span></span>](bias-utc.md)
    
- [<span data-ttu-id="538cc-200">StandardTime Element</span><span class="sxs-lookup"><span data-stu-id="538cc-200">StandardTime</span></span>](standardtime.md)
    
- [<span data-ttu-id="538cc-201">Bias</span><span class="sxs-lookup"><span data-stu-id="538cc-201">Bias</span></span>](bias.md)
    
- [<span data-ttu-id="538cc-202">Time</span><span class="sxs-lookup"><span data-stu-id="538cc-202">Time</span></span>](time.md)
    
- [<span data-ttu-id="538cc-203">DayOrder</span><span class="sxs-lookup"><span data-stu-id="538cc-203">DayOrder</span></span>](dayorder.md)
    
- [<span data-ttu-id="538cc-204">Month</span><span class="sxs-lookup"><span data-stu-id="538cc-204">Month</span></span>](month.md)
    
- [<span data-ttu-id="538cc-205">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="538cc-205">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md)
    
- [<span data-ttu-id="538cc-206">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="538cc-206">DaylightTime</span></span>](daylighttime.md)
    
- [<span data-ttu-id="538cc-207">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="538cc-207">WorkingPeriodArray</span></span>](workingperiodarray.md)
    
- [<span data-ttu-id="538cc-208">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="538cc-208">WorkingPeriod</span></span>](workingperiod.md)
    
- [<span data-ttu-id="538cc-209">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="538cc-209">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
    
- [<span data-ttu-id="538cc-210">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="538cc-210">StartTimeInMinutes</span></span>](starttimeinminutes.md)
    
- [<span data-ttu-id="538cc-211">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="538cc-211">EndTimeInMinutes</span></span>](endtimeinminutes.md)
    
## <a name="see-also"></a><span data-ttu-id="538cc-212">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="538cc-212">See also</span></span>

- [<span data-ttu-id="538cc-213">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="538cc-213">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="538cc-214">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="538cc-214">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
    

