---
title: Accéder à une série périodique à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 196a5671-2836-4696-b734-d5ecfdbf8962
description: Découvrez comment accéder aux éléments de calendrier dans une série périodique à l’aide de l’API gérée EWS ou EWS dans Exchange.
ms.openlocfilehash: 280affe532beb282bdd5cdb0c02a3dfaa62751e5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513240"
---
# <a name="access-a-recurring-series-by-using-ews-in-exchange"></a>Accéder à une série périodique à l’aide d’EWS dans Exchange

Découvrez comment accéder aux éléments de calendrier dans une série périodique à l’aide de l’API gérée EWS ou EWS dans Exchange.
  
Une série périodique de rendez-vous ou de réunions est composé d’une forme de base périodique, d’un certain nombre d’occurrences d’une série qui se répètent selon un modèle d’ensemble et, éventuellement, d’ensembles d’occurrences qui ont été modifiées et qui ont été supprimées. Vous pouvez utiliser l’API gérée EWS ou EWS pour accéder aux éléments de calendrier d’une série périodique. Cela vous permet de :
  
- Vérifiez si un élément de calendrier associé à un ID d’élément est un maître périodique, une occurrence d’une série ou une exception à une série.
    
- Recherchez des rendez-vous de récurrence dans votre dossier de calendrier.
    
- Obtenir les éléments de calendrier de récurrence associés
    
- Itérer les occurrences d’une série, les exceptions d’occurrence ou les suppressions d’occurrences.
    
## <a name="get-a-collection-of-recurring-calendar-items-by-using-the-ews-managed-api"></a>Obtenir une collection d’éléments de calendrier périodiques à l’aide de l’API gérée EWS

Si vous souhaitez récupérer une collection de rendez-vous, vous pouvez utiliser la méthode [ExchangeService.FindAppointments](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) pour récupérer tous les rendez-vous entre une date de début et de fin donnée, puis ajouter tous les éléments de calendrier dont le type de rendez-vous est **Occurrence** ou **Exception** à une collection, comme illustré dans l’exemple suivant. 
  
Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**. 
  
```cs
public static Collection<Appointment> FindRecurringCalendarItems(ExchangeService service, 
                                                                    DateTime startSearchDate, 
                                                                    DateTime endSearchDate)
{
    // Instantiate a collection to hold occurrences and exception calendar items.
    Collection<Appointment> foundAppointments = new Collection<Appointment>();
    // Create a calendar view to search the calendar folder and specify the properties to return.
    CalendarView calView = new CalendarView(startSearchDate, endSearchDate);
    calView.PropertySet = new PropertySet(BasePropertySet.IdOnly, 
                                            AppointmentSchema.Subject, 
                                            AppointmentSchema.Start, 
                                            AppointmentSchema.IsRecurring, 
                                            AppointmentSchema.AppointmentType);
    // Retrieve a collection of calendar items.
    FindItemsResults<Appointment> findResults = service.FindAppointments(WellKnownFolderName.Calendar, calView);
    // Add all calendar items in your view that are occurrences or exceptions to your collection.
    foreach (Appointment appt in findResults.Items)
    {
        if (appt.AppointmentType == AppointmentType.Occurrence || appt.AppointmentType == AppointmentType.Exception)
        {
            foundAppointments.Add(appt);
        }
        else
        {
            Console.WriteLine("Discarding calendar item of type {0}.", appt.AppointmentType);
        }
    }
    return foundAppointments;
}

```

Notez que les éléments de calendrier principal périodiques ne sont pas renvoyés dans un appel **à FindAppointments**. Si vous souhaitez récupérer des maîtres périodiques ou une approche plus générale de la récupération des éléments de calendrier, vous devez utiliser [ExchangeService.FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx). Vous pouvez ensuite utiliser un filtre de recherche pour récupérer uniquement les éléments dont la date de début est supérieure ou égale à la date que vous choisissez, et un affichage d’élément pour limiter le nombre d’éléments à renvoyer. Notez qu’un récurrable maître dont la date de début est antérieure à la date de début de votre recherche est in found, même si des occurrences se produisent dans cette plage.
  
Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**. 
  
```cs
public static Collection<Appointment> FindCalendarItemsByAppointmentType(ExchangeService service, 
                                                                         AppointmentType myAppointmentType, 
                                                                         DateTime startSearchDate)
{
    Collection<Appointment> foundAppointments = new Collection<Appointment>();
    // Create a search filter based on the start search date.
    SearchFilter.SearchFilterCollection searchFilter = new SearchFilter.SearchFilterCollection();
    searchFilter.Add(new SearchFilter.IsGreaterThanOrEqualTo(AppointmentSchema.Start, startSearchDate));
    // Create an item view to specify which properties to return.
    ItemView view = new ItemView(20);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, 
                                       AppointmentSchema.Subject, 
                                       AppointmentSchema.Start, 
                                       AppointmentSchema.AppointmentType,
                                       AppointmentSchema.IsRecurring);
    // Get the appointment items from the server with the properties we specified.
    FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Calendar, searchFilter, view);
    // Add each of the appointments of the type you want to the collection.
    foreach (Item item in findResults.Items)
    {
        Appointment appt = item as Appointment;
        if (appt.AppointmentType == myAppointmentType)
        {
            foundAppointments.Add(appt);
        }
    }
    return foundAppointments;
}

```

## <a name="get-related-recurrence-calendar-items-by-using-the-ews-managed-api"></a>Obtenir les éléments de calendrier de récurrence associés à l’aide de l’API gérée EWS

Parfois, vous avez une partie du puzzle, mais pour le résoudre, vous avez besoin du reste des pièces. Si vous avez l’ID d’élément pour un élément de calendrier de récurrence, vous pouvez obtenir les autres éléments dont vous avez besoin à l’aide de l’une des méthodes ou propriétés de l’API gérée EWS.
  
**Tableau 1. Propriété ou méthode d’API gérée EWS à utiliser pour obtenir les éléments de calendrier de récurrence associés**

|**Si vous avez l’ID d’élément pour...**|**Vous pouvez obtenir...**|**À l’aide de...**|
|:-----|:-----|:-----|
|Élément de calendrier principal périodique  <br/> | Première occurrence d’une série  <br/>  Dernière occurrence d’une série  <br/>  Les exceptions à une série  <br/>  Les rendez-vous supprimés d’une série  <br/>  Toute occurrence (en raison de son index)  <br/> |[Propriété Appointment.FirstOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx)  <br/> [Propriété Appointment.LastOccurrence](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx)  <br/> [Propriété Appointment.ModifiedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx)  <br/> [Propriété Appointment.DeletedOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx)  <br/> [Méthode Appointment.BindToOccurrence](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx)  <br/> |
|Une occurrence unique dans une série  <br/> |Le maître périodique  <br/> |[Méthode Appointment.BindToRecurringMaster](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx)  <br/> |
|Tout élément de calendrier (objet [Appointment)](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx)  <br/> |Valeur [d’éumération du type](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx) de rendez-vous  <br/> |[Propriété Appointment.AppointmentType](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx)  <br/> |
   
L’exemple de code suivant montre comment obtenir une forme de référence périodique, la première ou la dernière occurrence d’une série ou une occurrence en raison de son index.
  
Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**. 
  
```cs
public static void GetRelatedRecurrenceCalendarItems(ExchangeService service, ItemId itemId)
{
    Appointment calendarItem = Appointment.Bind(service, itemId, new PropertySet(AppointmentSchema.AppointmentType));
    Appointment recurrMaster = new Appointment(service);
    PropertySet props = new PropertySet(AppointmentSchema.AppointmentType,
                                        AppointmentSchema.Subject,
                                        AppointmentSchema.FirstOccurrence,
                                        AppointmentSchema.LastOccurrence,
                                        AppointmentSchema.ModifiedOccurrences,
                                        AppointmentSchema.DeletedOccurrences);
    // If the item ID is not for a recurring master, retrieve the recurring master for the series.
    switch (calendarItem.AppointmentType)
    {
        // Calendar item is a recurring master so use Appointment.Bind
        case AppointmentType.RecurringMaster:
            recurrMaster = Appointment.Bind(service, itemId, props);
            break;
        // The calendar item is a single instance meeting, so there are no instances to modify or delete.
        case AppointmentType.Single:
            Console.WriteLine("Item id must reference a calendar item that is part of a recurring series.");
            return;
        // The calendar item is an occurrence in the series, so use BindToRecurringMaster.
        case AppointmentType.Occurrence:
            recurrMaster = Appointment.BindToRecurringMaster(service, itemId, props);
            break;
        // The calendar item is an exception to the series, so use BindToRecurringMaster.                
        case AppointmentType.Exception:
            recurrMaster = Appointment.BindToRecurringMaster(service, itemId, props);
            break;
    }
    // View the first occurrence, last occurrence, and number of modified and deleted occurrences associated with the recurring master.
    Console.WriteLine("Information for the {0} recurring series:", recurrMaster.Subject);
    Console.WriteLine("The start time for the first appointment with id \t{0} was on \t{1}.", 
                        recurrMaster.FirstOccurrence.ItemId.ToString().Substring(144), 
                        recurrMaster.FirstOccurrence.Start.ToString());
    Console.WriteLine("The start time for the last appointment with id \t{0} will be on \t{1}.", 
                        recurrMaster.LastOccurrence.ItemId.ToString().Substring(144), 
                        recurrMaster.LastOccurrence.Start.ToString());
    Console.WriteLine("There are {0} modified occurrences and {1} deleted occurrences.", 
                        recurrMaster.ModifiedOccurrences == null ? "no" : recurrMaster.ModifiedOccurrences.Count.ToString(), 
                        recurrMaster.DeletedOccurrences == null ? "no" : recurrMaster.DeletedOccurrences.Count.ToString());
    // Bind to the first occurrence of a series by using its index.
    Appointment firstOccurrence = Appointment.BindToOccurrence(service, 
                                                                recurrMaster.Id, 
                                                                1, // Index of first item is 1, not 0.
                                                                new PropertySet(AppointmentSchema.AppointmentType,
                                                                                AppointmentSchema.Start));
    Console.WriteLine("Compare the start times for a recurring master's first occurrence " + 
                        "and the occurrence found at index 1 using the BindToOccurrence method:");
    Console.WriteLine("The appointment at index 1 has a start time of\t\t\t\t {0}\n" +
                        "Which matches that of the first occurrence on the recurring master: \t {1}",
                        firstOccurrence.Start.ToString(),
                        recurrMaster.FirstOccurrence.Start.ToString());
}

```

## <a name="access-calendar-items-in-a-recurring-series-by-using-ews"></a>Accéder aux éléments de calendrier d’une série périodique à l’aide d’EWS

L’accès aux éléments de calendrier dans une série périodique est très similaire à l’accès à des instances d’éléments de calendrier. Vous utilisez une [demande d’opération GetItem,](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) en spécifiant les propriétés que vous souhaitez, avec l’OccurrenceItemId de l’instance de rendez-vous dont vous avez besoin. [](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) [L’OccurrenceItemId contient](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) **l’ItemID** de la forme de référence périodique de l’occurrence, ainsi que sa valeur d’index dans la série. 
  
Le XML suivant montre la [requête GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) utilisée pour renvoyer une occurrence dans une série spécifiée par son index. Notez que **l’ItemID** de la master périodique a été raccourci pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
          <t:FieldURI FieldURI="calendar:Start" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:OccurrenceItemId RecurringMasterId="AAMkA" InstanceIndex="1" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **GetItem** avec un message [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) qui inclut une valeur [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NoError**, qui indique que le message a été correctement créé, et l’ItemId du message nouvellement créé. [](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 
  
## <a name="see-also"></a>Voir aussi


- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

