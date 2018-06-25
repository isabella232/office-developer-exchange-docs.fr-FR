---
title: Obtenir des rendez-vous et réunions à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bae582a-8cb3-4e77-be2a-7e107fad26fe
description: Découvrez comment obtenir des rendez-vous et réunions à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 0f5eb135142e807f30f48f01d7948fbdbf147ac2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754834"
---
# <a name="get-appointments-and-meetings-by-using-ews-in-exchange"></a>Obtenir des rendez-vous et réunions à l’aide de EWS dans Exchange

Découvrez comment obtenir des rendez-vous et réunions à l’aide de l’API managée EWS ou EWS dans Exchange.
  
Vous pouvez récupérer des rendez-vous et réunions à partir d’un dossier de calendrier à l’aide de la méthode d’API managées [CalendarFolder.FindAppointments](http://msdn.microsoft.com/en-us/library/dd636179%28v=exchg.80%29.aspx) ou l’opération EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) . 
  
## <a name="get-appointments-by-using-the-ews-managed-api"></a>Obtenir des rendez-vous à l’aide de l’API managée EWS
<a name="bk_retrieveappsEWSMA"> </a>

L’exemple de code suivant montre comment utiliser l’API managée EWS pour récupérer des rendez-vous d’un utilisateur entre un début spécifiée et l’heure de fin.
  
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

Voici la sortie de l’exemple de code.
  
Les cinq premiers rendez-vous dans votre calendrier à partir de 21/8/2013 à 9/20/2013 sont les suivants : 
  
Objet : Réunion début de l’équipe Contoso développements : 21/8/2013 12:30:00 PM fin : 21/8/2013 1:00:00 PM
  
Objet : Quotidienne réunion démarrer : 21/8/2013 1:00:00 PM fin : 21/8/2013 2:00:00 PM
  
Objet : Déjeuner avec l’équipe commerciale démarrer : 21/8/2013 2:30:00 PM fin : 21/8/2013 3:30:00 PM
  
Objet : Tennis au début club : 22/8/2013 11:00:00 AM fin : 22/8/2013 12:00:00 PM
  
Sujet : Présentation technique en ligne formation en ligne : 22/8/2013 2:00:00 PM fin : 22/8/2013 3:00:00 PM
## <a name="get-appointments-by-using-ews"></a>Obtenir des rendez-vous à l’aide de EWS
<a name="bk_xml"> </a>

Le code XML suivant montre une demande d’opération [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) pour renvoyer un ID de dossier pour l’opération [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Le code XML suivant montre la réponse **GetFolder** . Notez que les attributs **FolderID** et **ChangeKey** sont raccourcis pour améliorer la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="731" MinorBuildNumber="10" Version="V2_3" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Le code XML suivant montre la demande **FindItem** permet de retourner les rendez-vous demandés. Notez que les attributs **FolderID** et **ChangeKey** sont raccourcis pour améliorer la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
       xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
       xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Le code XML suivant montre la réponse **FindItem** . Notez que les attributs **ItemID** et **ChangeKey** sont raccourcis pour améliorer la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="731" MinorBuildNumber="10" Version="V2_3" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="recurring-meetings-and-the-calendar-view"></a>Les réunions périodiques et l’affichage Calendrier
<a name="bk_recurring"> </a>

Le dossier calendrier est légèrement différent des autres dossiers dans une boîte aux lettres, car les occurrences dans une série périodique et les exceptions à une série périodique ne sont pas des éléments réels dans la boîte aux lettres, mais plutôt sont stockées en tant que pièces jointes à un masque périodique interne. Cela signifie que, bien que vous pouvez créer une demande EWS qui renvoie des valeurs entre un ensemble de **Démarrer** et valeurs de **fin** à l’aide d’une de l' API managée EWS **FindItems** surcharger des méthodes, telles que [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou le [EWS FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) opération EWS se présente pas par le biais de la table des pièces jointes de chaque élément de calendrier pour rechercher les exceptions et les occurrences. 
  
Au lieu de cela, vous souhaitez vraiment faire est quelque chose à appliquer un *Dataview* sur union de deux tables SQL, à l’aide d’un objet [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) . Notez que pour des raisons de performances, nous vous recommandons d’utiliser la propriété [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) pour limiter la taille de la réponse en indiquant le nombre de rendez-vous ou réunions à retourner, ainsi que les propriétés spécifiques que vous souhaitez. 
  
## <a name="see-also"></a>Voir aussi
<a name="bk_additional"> </a>

- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
    
- [Créer des rendez-vous et réunions à l’aide de EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Mettre à jour vos rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    

