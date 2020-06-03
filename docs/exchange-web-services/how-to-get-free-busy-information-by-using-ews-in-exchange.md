---
title: Obtenir des informations de disponibilité à l'aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 0e6709c0-dc3d-4280-8c53-cbec9bbdcc9e
description: Découvrez comment obtenir des informations de disponibilité et des heures de réunion suggérées à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 19f0181161b2e2dbde70f3ec7427d9d66c5bdc4d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528028"
---
# <a name="get-freebusy-information-by-using-ews-in-exchange"></a><span data-ttu-id="24b94-103">Obtenir des informations de disponibilité à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="24b94-103">Get free/busy information by using EWS in Exchange</span></span>

<span data-ttu-id="24b94-104">Découvrez comment obtenir des informations de disponibilité et des heures de réunion suggérées à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="24b94-104">Learn how to get free/busy information and suggested meeting times by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="24b94-105">L’utilisation de l’API managée EWS ou EWS pour [créer par programme une réunion](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md) et envoyer des demandes de réunion est intéressante, mais trouver un temps qui s’applique à tous vos participants est souvent un véritable défi.</span><span class="sxs-lookup"><span data-stu-id="24b94-105">Using the EWS Managed API or EWS to programmatically [create a meeting](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md) and send out meeting requests is great, but finding a time that works for all your attendees is often a challenge.</span></span> <span data-ttu-id="24b94-106">Si vous devez vérifier manuellement si tout le monde est disponible, cela ne revient pas à automatiser la tâche.</span><span class="sxs-lookup"><span data-stu-id="24b94-106">If you have to manually check to see when everyone is available, it defeats the purpose of automating the task.</span></span> <span data-ttu-id="24b94-107">Heureusement, la méthode de l’API managée EWS [ExchangeService. GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) et l’opération EWS [GetUserAvailability](https://msdn.microsoft.com/library/7906711b-80a1-42ae-8b33-26eeac036a5a%28Office.15%29.aspx) arrivent à votre secours.</span><span class="sxs-lookup"><span data-stu-id="24b94-107">Fortunately, the [ExchangeService.GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) EWS Managed API method and the [GetUserAvailability](https://msdn.microsoft.com/library/7906711b-80a1-42ae-8b33-26eeac036a5a%28Office.15%29.aspx) EWS operation come to your rescue.</span></span> <span data-ttu-id="24b94-108">Vous pouvez utiliser cette méthode ou cette opération pour interroger un serveur Exchange afin de trouver le meilleur moment pour planifier une réunion ou obtenir des informations de disponibilité pour les participants.</span><span class="sxs-lookup"><span data-stu-id="24b94-108">You can use this method or operation to query an Exchange server to find the best time to schedule a meeting or just get free/busy information for attendees.</span></span> <span data-ttu-id="24b94-109">Vous pouvez obtenir les informations de disponibilité pour une liste de participants ou faire en sorte que votre serveur Exchange trouve une heure de réunion pour vous, ou les deux.</span><span class="sxs-lookup"><span data-stu-id="24b94-109">You can get the free/busy information for a list of attendees, or have your Exchange server find a meeting time for you, or both</span></span> 
  
<span data-ttu-id="24b94-110">La figure 1 illustre le problème et la solution.</span><span class="sxs-lookup"><span data-stu-id="24b94-110">Figure 1 illustrates the problem and the solution.</span></span>
  
<span data-ttu-id="24b94-111">**Figure 1. Demande d’informations de disponibilité à partir d’un serveur Exchange**</span><span class="sxs-lookup"><span data-stu-id="24b94-111">**Figure 1. Requesting availability information from an Exchange server**</span></span>

![Image qui montre comment la méthode/l’opération GetUserAvailability résout le problème de la détermination de la disponibilité des participants en transmettant une série d’options à un serveur Exchange.](media/GetUserAvailability1.png)
  
## <a name="get-suggested-meeting-times-and-freebusy-information-by-using-the-ews-managed-api"></a><span data-ttu-id="24b94-113">Obtenir des heures de réunion et des informations de disponibilité suggérées à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="24b94-113">Get suggested meeting times and free/busy information by using the EWS Managed API</span></span>
<span data-ttu-id="24b94-114"><a name="bk_getavailewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="24b94-114"><a name="bk_getavailewsma"> </a></span></span>

<span data-ttu-id="24b94-115">Vous pouvez obtenir la liste des heures de réunion suggérées et toutes les heures d’événements planifiées pour vos participants lorsque vous utilisez une valeur d’énumération [AvailabilityData](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.availabilitydata%28v=exchg.80%29.aspx) de **FreeBusyAndSuggestions** dans votre appel de méthode [ExchangeService. GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="24b94-115">You can get both a list of suggested meeting times and all the scheduled event times for your attendees when you use an [AvailabilityData](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.availabilitydata%28v=exchg.80%29.aspx) enumeration value of **FreeBusyAndSuggestions** in your [ExchangeService.GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) method call, as shown in the following example.</span></span> 
  
<span data-ttu-id="24b94-116">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="24b94-116">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
private static void GetSuggestedMeetingTimesAndFreeBusyInfo(ExchangeService service)
{
    // Create a collection of attendees. 
    List<AttendeeInfo> attendees = new List<AttendeeInfo>(); 
 
    attendees.Add(new AttendeeInfo() 
    { 
        SmtpAddress = "mack@contoso.com", 
        AttendeeType = MeetingAttendeeType.Organizer 
    }); 
 
    attendees.Add(new AttendeeInfo() 
    { 
        SmtpAddress = "sadie@contoso.com", 
        AttendeeType = MeetingAttendeeType.Required 
    }); 
 
    // Specify options to request free/busy information and suggested meeting times.
    AvailabilityOptions availabilityOptions = new AvailabilityOptions(); 
    availabilityOptions.GoodSuggestionThreshold = 49; 
    availabilityOptions.MaximumNonWorkHoursSuggestionsPerDay = 0;
    availabilityOptions.MaximumSuggestionsPerDay = 2;
    // Note that 60 minutes is the default value for MeetingDuration, but setting it explicitly for demonstration purposes.
    availabilityOptions.MeetingDuration = 60; 
    availabilityOptions.MinimumSuggestionQuality = SuggestionQuality.Good; 
    availabilityOptions.DetailedSuggestionsWindow = new TimeWindow(DateTime.Now.AddDays(1), DateTime.Now.AddDays(2));
    availabilityOptions.RequestedFreeBusyView = FreeBusyViewType.FreeBusy;
 
    // Return free/busy information and a set of suggested meeting times. 
    // This method results in a GetUserAvailabilityRequest call to EWS.
    GetUserAvailabilityResults results = service.GetUserAvailability(attendees, 
                                                                     availabilityOptions.DetailedSuggestionsWindow, 
                                                                     AvailabilityData.FreeBusyAndSuggestions, 
                                                                     availabilityOptions); 
    // Display suggested meeting times. 
    Console.WriteLine("Availability for {0} and {1}", attendees[0].SmtpAddress, attendees[1].SmtpAddress); 
    Console.WriteLine(); 
 
    foreach (Suggestion suggestion in results.Suggestions) 
    { 
        Console.WriteLine("Suggested date: {0}\n", suggestion.Date.ToShortDateString()); 
        Console.WriteLine("Suggested meeting times:\n");
        foreach (TimeSuggestion timeSuggestion in suggestion.TimeSuggestions) 
        { 
                    Console.WriteLine("\t{0} - {1}\n", 
                                      timeSuggestion.MeetingTime.ToShortTimeString(), 
                                      timeSuggestion.MeetingTime.Add(TimeSpan.FromMinutes(availabilityOptions.MeetingDuration)).ToShortTimeString()); 
        } 
    }
            
    int i = 0;
    // Display free/busy times.
    foreach (AttendeeAvailability availability in results.AttendeesAvailability)
    {
        Console.WriteLine("Availability information for {0}:\n", attendees[i].SmtpAddress);
        foreach (CalendarEvent calEvent in availability.CalendarEvents)
        {
            Console.WriteLine("\tBusy from {0} to {1} \n", calEvent.StartTime.ToString(), calEvent.EndTime.ToString());
        }
        i++;
    }
}

```

## <a name="get-suggested-meeting-times-and-freebusy-information-by-using-ews"></a><span data-ttu-id="24b94-117">Obtenir des heures de réunion et des informations de disponibilité suggérées à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="24b94-117">Get suggested meeting times and free/busy information by using EWS</span></span>
<span data-ttu-id="24b94-118"><a name="bk_getavailews"> </a></span><span class="sxs-lookup"><span data-stu-id="24b94-118"><a name="bk_getavailews"> </a></span></span>

<span data-ttu-id="24b94-119">Vous pouvez obtenir la liste des heures de réunion suggérées et toutes les heures d’événements planifiées pour vos participants à l’aide de l’opération [GetUserAvailability](https://msdn.microsoft.com/library/7906711b-80a1-42ae-8b33-26eeac036a5a%28Office.15%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="24b94-119">You can get both a list of suggested meeting times and all the scheduled event times for your attendees by using the [GetUserAvailability](https://msdn.microsoft.com/library/7906711b-80a1-42ae-8b33-26eeac036a5a%28Office.15%29.aspx) operation, as shown in the following example.</span></span> <span data-ttu-id="24b94-120">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez l’API managée EWS pour [obtenir des heures de réunion suggérées](#bk_getavailewsma).</span><span class="sxs-lookup"><span data-stu-id="24b94-120">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get suggested meeting times](#bk_getavailewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Name="(UTC-08:00) Pacific Time (US &amp;amp; Canada)" Id="Pacific Standard Time">
        <t:Periods>
          <t:Period Bias="P0DT8H0M0.0S" Name="Standard" Id="Std" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/1" />
          <t:Period Bias="P0DT7H0M0.0S" Name="Daylight" Id="Dlt/2007" />
        </t:Periods>
        <t:TransitionsGroups>
          <t:TransitionsGroup Id="0">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/1</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>4</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>10</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>-1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
          <t:TransitionsGroup Id="1">
            <t:RecurringDayTransition>
              <t:To Kind="Period">Dlt/2007</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>3</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>2</t:Occurrence>
            </t:RecurringDayTransition>
            <t:RecurringDayTransition>
              <t:To Kind="Period">Std</t:To>
              <t:TimeOffset>P0DT2H0M0.0S</t:TimeOffset>
              <t:Month>11</t:Month>
              <t:DayOfWeek>Sunday</t:DayOfWeek>
              <t:Occurrence>1</t:Occurrence>
            </t:RecurringDayTransition>
          </t:TransitionsGroup>
        </t:TransitionsGroups>
        <t:Transitions>
          <t:Transition>
            <t:To Kind="Group">0</t:To>
          </t:Transition>
          <t:AbsoluteDateTransition>
            <t:To Kind="Group">1</t:To>
            <t:DateTime>2007-01-01T08:00:00.000Z</t:DateTime>
          </t:AbsoluteDateTransition>
        </t:Transitions>
      </t:TimeZoneDefinition>
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:GetUserAvailabilityRequest>
      <m:MailboxDataArray>
        <t:MailboxData>
          <t:Email>
            <t:Address>mack@contoso.com</t:Address>
          </t:Email>
          <t:AttendeeType>Organizer</t:AttendeeType>
          <t:ExcludeConflicts>false</t:ExcludeConflicts>
        </t:MailboxData>
        <t:MailboxData>
          <t:Email>
            <t:Address>sadie@contoso.com</t:Address>
          </t:Email>
          <t:AttendeeType>Required</t:AttendeeType>
          <t:ExcludeConflicts>false</t:ExcludeConflicts>
        </t:MailboxData>
      </m:MailboxDataArray>
      <t:FreeBusyViewOptions>
        <t:TimeWindow>
          <t:StartTime>2014-02-13T00:00:00</t:StartTime>
          <t:EndTime>2014-02-14T00:00:00</t:EndTime>
        </t:TimeWindow>
        <t:MergedFreeBusyIntervalInMinutes>30</t:MergedFreeBusyIntervalInMinutes>
        <t:RequestedView>FreeBusy</t:RequestedView>
      </t:FreeBusyViewOptions>
      <t:SuggestionsViewOptions>
        <t:GoodThreshold>49</t:GoodThreshold>
        <t:MaximumResultsByDay>2</t:MaximumResultsByDay>
        <t:MaximumNonWorkHourResultsByDay>0</t:MaximumNonWorkHourResultsByDay>
        <t:MeetingDurationInMinutes>60</t:MeetingDurationInMinutes>
        <t:MinimumSuggestionQuality>Good</t:MinimumSuggestionQuality>
        <t:DetailedSuggestionsWindow>
          <t:StartTime>2014-02-13T00:00:00</t:StartTime>
          <t:EndTime>2014-02-14T00:00:00</t:EndTime>
        </t:DetailedSuggestionsWindow>
      </t:SuggestionsViewOptions>
    </m:GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="24b94-121">Le serveur répond à la [demande GetUserAvailability](https://msdn.microsoft.com/library/7906711b-80a1-42ae-8b33-26eeac036a5a%28Office.15%29.aspx) avec un message de [réponse GetUserAvailability](https://msdn.microsoft.com/library/6999510a-d60e-43da-8964-57b5fb3e9d11%28Office.15%29.aspx) , comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="24b94-121">The server responds to the [GetUserAvailability request](https://msdn.microsoft.com/library/7906711b-80a1-42ae-8b33-26eeac036a5a%28Office.15%29.aspx) with a [GetUserAvailability response](https://msdn.microsoft.com/library/6999510a-d60e-43da-8964-57b5fb3e9d11%28Office.15%29.aspx) message, as shown in the following example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="873" MinorBuildNumber="9" Version="V2_9" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserAvailabilityResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FreeBusyResponseArray>
        <FreeBusyResponse>
          <ResponseMessage ResponseClass="Success">
            <ResponseCode>NoError</ResponseCode>
          </ResponseMessage>
          <FreeBusyView>
            <FreeBusyViewType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">FreeBusy</FreeBusyViewType>
            <CalendarEventArray xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2014-02-13T08:00:00</StartTime>
                <EndTime>2014-02-13T10:00:00</EndTime>
                <BusyType>Free</BusyType>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2014-02-13T11:00:00</StartTime>
                <EndTime>2014-02-13T12:00:00</EndTime>
                <BusyType>Busy</BusyType>
              </CalendarEvent>
            </CalendarEventArray>
            <WorkingHours xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
              <TimeZone>
                <Bias>480</Bias>
                <StandardTime>
                  <Bias>0</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>1</DayOrder>
                  <Month>11</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </StandardTime>
                <DaylightTime>
                  <Bias>-60</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>2</DayOrder>
                  <Month>3</Month>
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
            <FreeBusyViewType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">FreeBusy</FreeBusyViewType>
            <CalendarEventArray xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
              <CalendarEvent>
                <StartTime>2014-02-12T00:00:00</StartTime>
                <EndTime>2014-02-13T00:00:00</EndTime>
                <BusyType>Free</BusyType>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2014-02-13T08:00:00</StartTime>
                <EndTime>2014-02-13T10:00:00</EndTime>
                <BusyType>Free</BusyType>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2014-02-13T11:00:00</StartTime>
                <EndTime>2014-02-13T12:00:00</EndTime>
                <BusyType>Busy</BusyType>
              </CalendarEvent>
              <CalendarEvent>
                <StartTime>2014-02-13T15:00:00</StartTime>
                <EndTime>2014-02-13T16:00:00</EndTime>
                <BusyType>Tentative</BusyType>
              </CalendarEvent>
            </CalendarEventArray>
            <WorkingHours xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
              <TimeZone>
                <Bias>480</Bias>
                <StandardTime>
                  <Bias>0</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>1</DayOrder>
                  <Month>11</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </StandardTime>
                <DaylightTime>
                  <Bias>-60</Bias>
                  <Time>02:00:00</Time>
                  <DayOrder>2</DayOrder>
                  <Month>3</Month>
                  <DayOfWeek>Sunday</DayOfWeek>
                </DaylightTime>
              </TimeZone>
              <WorkingPeriodArray>
                <WorkingPeriod>
                  <DayOfWeek>Monday Tuesday Wednesday Thursday Friday</DayOfWeek>
                  <StartTimeInMinutes>540</StartTimeInMinutes>
                  <EndTimeInMinutes>1020</EndTimeInMinutes>
                </WorkingPeriod>
              </WorkingPeriodArray>
            </WorkingHours>
          </FreeBusyView>
        </FreeBusyResponse>
      </FreeBusyResponseArray>
      <SuggestionsResponse>
        <ResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
        </ResponseMessage>
        <SuggestionDayResultArray>
          <SuggestionDayResult xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <Date>2014-02-13T00:00:00</Date>
            <DayQuality>Excellent</DayQuality>
            <SuggestionArray>
              <Suggestion>
                <MeetingTime>2014-02-13T09:00:00</MeetingTime>
                <IsWorkTime>true</IsWorkTime>
                <SuggestionQuality>Excellent</SuggestionQuality>
                <AttendeeConflictDataArray>
                  <IndividualAttendeeConflictData>
                    <BusyType>Free</BusyType>
                  </IndividualAttendeeConflictData>
                  <IndividualAttendeeConflictData>
                    <BusyType>Free</BusyType>
                  </IndividualAttendeeConflictData>
                </AttendeeConflictDataArray>
              </Suggestion>
              <Suggestion>
                <MeetingTime>2014-02-13T09:30:00</MeetingTime>
                <IsWorkTime>true</IsWorkTime>
                <SuggestionQuality>Excellent</SuggestionQuality>
                <AttendeeConflictDataArray>
                  <IndividualAttendeeConflictData>
                    <BusyType>Free</BusyType>
                  </IndividualAttendeeConflictData>
                  <IndividualAttendeeConflictData>
                    <BusyType>Free</BusyType>
                  </IndividualAttendeeConflictData>
                </AttendeeConflictDataArray>
              </Suggestion>
            </SuggestionArray>
          </SuggestionDayResult>
        </SuggestionDayResultArray>
      </SuggestionsResponse>
    </GetUserAvailabilityResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="24b94-122">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="24b94-122">See also</span></span>


- [<span data-ttu-id="24b94-123">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="24b94-123">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="24b94-124">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="24b94-124">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="24b94-125">Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="24b94-125">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    

