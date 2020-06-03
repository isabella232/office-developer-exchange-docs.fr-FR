---
title: Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1bae582a-8cb3-4e77-be2a-7e107fad26fe
description: Découvrez comment obtenir des rendez-vous et des réunions à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: d951bfeccdf50ae1397ecdd4887ed05548b25001
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528089"
---
# <a name="get-appointments-and-meetings-by-using-ews-in-exchange"></a><span data-ttu-id="ccec7-103">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ccec7-103">Get appointments and meetings by using EWS in Exchange</span></span>

<span data-ttu-id="ccec7-104">Découvrez comment obtenir des rendez-vous et des réunions à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="ccec7-104">Learn how to get appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="ccec7-105">Vous pouvez récupérer des rendez-vous et des réunions à partir d’un dossier de calendrier à l’aide de la méthode de l’API managée EWS [CalendarFolder. findappointmentspour](https://msdn.microsoft.com/library/dd636179%28v=exchg.80%29.aspx) ou de l’opération EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ccec7-105">You can retrieve appointments and meetings from a calendar folder by using the [CalendarFolder.FindAppointments](https://msdn.microsoft.com/library/dd636179%28v=exchg.80%29.aspx) EWS Managed API method or the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation.</span></span> 
  
## <a name="get-appointments-by-using-the-ews-managed-api"></a><span data-ttu-id="ccec7-106">Obtenir des rendez-vous à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="ccec7-106">Get appointments by using the EWS Managed API</span></span>
<span data-ttu-id="ccec7-107"><a name="bk_retrieveappsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="ccec7-107"><a name="bk_retrieveappsEWSMA"> </a></span></span>

<span data-ttu-id="ccec7-108">L’exemple de code suivant montre comment utiliser l’API managée EWS pour récupérer les rendez-vous d’un utilisateur qui se situent entre une heure de début et une heure de fin spécifiées.</span><span class="sxs-lookup"><span data-stu-id="ccec7-108">The following code example shows how to use the EWS Managed API to retrieve a user's appointments that fall between a specified start and end time.</span></span>
  
```cs
       // Initialize values for the start and end times, and the number of appointments to retrieve.
            DateTime startDate = DateTime.Now;
            DateTime endDate = startDate.AddDays(30);
            const int NUM_APPTS = 5;
            // Initialize the calendar folder object with only the folder ID. 
            CalendarFolder calendar = CalendarFolder.Bind(service, WellKnownFolderName.Calendar, new PropertySet());
            // Set the start and end time and number of appointments to retrieve.
            CalendarView cView = new CalendarView(startDate, endDate, NUM_APPTS);
            // Limit the properties returned to the appointment's subject, start time, and end time.
            cView.PropertySet = new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End);
            // Retrieve a collection of appointments by using the calendar view.
            FindItemsResults<Appointment> appointments = calendar.FindAppointments(cView);
            Console.WriteLine("\nThe first " + NUM_APPTS + " appointments on your calendar from " + startDate.Date.ToShortDateString() + 
                              " to " + endDate.Date.ToShortDateString() + " are: \n");
            
            foreach (Appointment a in appointments)
            {
                Console.Write("Subject: " + a.Subject.ToString() + " ");
                Console.Write("Start: " + a.Start.ToString() + " ");
                Console.Write("End: " + a.End.ToString());
                Console.WriteLine();
            }

```

<br/>

<span data-ttu-id="ccec7-109">Voici le résultat de l’exemple de code.</span><span class="sxs-lookup"><span data-stu-id="ccec7-109">The following is the output from the code example.</span></span>
  
```text
The first five appointments on your calendar from 8/21/2013 to 9/20/2013 are: 
  
Subject: Contoso devs team meeting Start: 8/21/2013 12:30:00 PM End: 8/21/2013 1:00:00 PM
  
Subject: Daily status meeting Start: 8/21/2013 1:00:00 PM End: 8/21/2013 2:00:00 PM
  
Subject: Lunch with sales team Start: 8/21/2013 2:30:00 PM End: 8/21/2013 3:30:00 PM
  
Subject: Tennis at the club Start: 8/22/2013 11:00:00 AM End: 8/22/2013 12:00:00 PM
  
Subject: Online training webcast: 8/22/2013 2:00:00 PM End: 8/22/2013 3:00:00 PM
```

## <a name="get-appointments-by-using-ews"></a><span data-ttu-id="ccec7-110">Obtenir des rendez-vous à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="ccec7-110">Get appointments by using EWS</span></span>
<span data-ttu-id="ccec7-111"><a name="bk_xml"> </a></span><span class="sxs-lookup"><span data-stu-id="ccec7-111"><a name="bk_xml"> </a></span></span>

<span data-ttu-id="ccec7-112">Le code XML suivant montre une demande d’opération [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) permettant de renvoyer un ID de dossier pour l’opération [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ccec7-112">The following XML shows a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request to return a folder ID for the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<br/>

<span data-ttu-id="ccec7-113">Le code XML suivant illustre la réponse **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="ccec7-113">The following XML shows the **GetFolder** response.</span></span> <span data-ttu-id="ccec7-114">Notez que les attributs **FolderId** et **ChangeKey** sont raccourcis pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ccec7-114">Note that the **FolderID** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="731" MinorBuildNumber="10" Version="V2_3" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:CalendarFolder>
              <t:FolderId Id="AAMk" ChangeKey="AgAA" />
            </t:CalendarFolder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<br/>

<span data-ttu-id="ccec7-115">Le code XML suivant montre la requête **FindItem** utilisée pour renvoyer les rendez-vous demandés.</span><span class="sxs-lookup"><span data-stu-id="ccec7-115">The following XML shows the **FindItem** request used to return the requested appointments.</span></span> <span data-ttu-id="ccec7-116">Notez que les attributs **FolderId** et **ChangeKey** sont raccourcis pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ccec7-116">Note that the **FolderID** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView MaxEntriesReturned="5" StartDate="2013-08-21T17:30:24.127Z" EndDate="2013-09-20T17:30:24.127Z" />
      <m:ParentFolderIds>
        <t:FolderId Id="AAMk" ChangeKey="AgAA" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<br/>

<span data-ttu-id="ccec7-117">Le code XML suivant illustre la réponse **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="ccec7-117">The following XML shows the **FindItem** response.</span></span> <span data-ttu-id="ccec7-118">Notez que les attributs **ItemId** et **ChangeKey** sont raccourcis pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ccec7-118">Note that the **ItemID** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="731" MinorBuildNumber="10" Version="V2_3" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="33" IncludesLastItemInRange="false">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Contoso devs team meeting</t:Subject>
                <t:Start>2013-08-21T19:30:00Z</t:Start>
                <t:End>2013-08-21T20:00:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Daily status meeting</t:Subject>
                <t:Start>2013-08-21T20:00:00Z</t:Start>
                <t:End>2013-08-21T21:00:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Lunch with sales team</t:Subject>
                <t:Start>2013-08-21T21:30:00Z</t:Start>
                <t:End>2013-08-21T22:30:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMk" ChangeKey="DwAA" />
                <t:Subject>Tennis at the club</t:Subject>
                <t:Start>2013-08-22T18:00:00Z</t:Start>
                <t:End>2013-08-22T19:00:00Z</t:End>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkA" ChangeKey="DwAA" />
                <t:Subject>Online training webcast</t:Subject>
                <t:Start>2013-08-22T21:00:00Z</t:Start>
                <t:End>2013-08-22T22:00:00Z</t:End>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="recurring-meetings-and-the-calendar-view"></a><span data-ttu-id="ccec7-119">Réunions périodiques et affichage Calendrier</span><span class="sxs-lookup"><span data-stu-id="ccec7-119">Recurring meetings and the calendar view</span></span>
<span data-ttu-id="ccec7-120"><a name="bk_recurring"> </a></span><span class="sxs-lookup"><span data-stu-id="ccec7-120"><a name="bk_recurring"> </a></span></span>

<span data-ttu-id="ccec7-121">Le dossier calendrier est légèrement différent des autres dossiers d’une boîte aux lettres, car les occurrences d’une série périodique et les exceptions à une série périodique ne sont pas des éléments réels dans la boîte aux lettres, mais sont plutôt stockées en tant que pièces jointes à une forme de base périodique.</span><span class="sxs-lookup"><span data-stu-id="ccec7-121">The calendar folder is a little different from other folders in a mailbox because occurrences in a recurring series and exceptions to a recurring series are not actual items in the mailbox, but rather are stored internally as attachments to a recurring master.</span></span> <span data-ttu-id="ccec7-122">Cela signifie que, bien que vous puissiez créer une requête EWS qui renvoie des valeurs entre un ensemble de valeurs de **début** et de **fin** à l’aide d’une des méthodes de surcharge **FindItems** de l’API managée EWS, telles que [ExchangeService. FINDITEMS](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou l’opération EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , EWS ne parcourt pas la table des pièces jointes de chaque élément de calendrier pour trouver des exceptions et des occurrences</span><span class="sxs-lookup"><span data-stu-id="ccec7-122">This means that although you can create an EWS request that returns values between a set of **start** and **end** values by using one of the EWS Managed API **FindItems** overload methods, such as [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or the EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation, EWS would not look through the attachment table of every calendar item to find exceptions and occurrences.</span></span> 
  
<span data-ttu-id="ccec7-123">Au lieu de cela, ce que vous voulez faire est une autre façon d’appliquer un *DataView* à une Union de deux tables SQL, à l’aide d’un objet [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ccec7-123">Instead, what you really want to do is something akin to applying a  *Dataview*  onto a union of two SQL tables, using a [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="ccec7-124">Pour des raisons de performances, nous vous recommandons d’utiliser la propriété [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) pour limiter la taille de la réponse en indiquant le nombre de rendez-vous ou de réunions que vous souhaitez renvoyer, ainsi que les propriétés spécifiques de votre choix.</span><span class="sxs-lookup"><span data-stu-id="ccec7-124">Note that for performance reasons, we recommend that you use the [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) property to limit the size of the response by indicating the number of appointments or meetings you want returned, as well as the specific properties you want.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ccec7-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ccec7-125">See also</span></span>
<span data-ttu-id="ccec7-126"><a name="bk_additional"> </a></span><span class="sxs-lookup"><span data-stu-id="ccec7-126"><a name="bk_additional"> </a></span></span>

- [<span data-ttu-id="ccec7-127">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ccec7-127">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)   
- [<span data-ttu-id="ccec7-128">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="ccec7-128">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)  
- [<span data-ttu-id="ccec7-129">Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ccec7-129">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="ccec7-130">Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ccec7-130">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="ccec7-131">Développer des clients de service web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ccec7-131">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

