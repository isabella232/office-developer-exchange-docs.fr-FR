---
title: Accéder à une série périodique à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 196a5671-2836-4696-b734-d5ecfdbf8962
description: Découvrez comment accéder aux éléments de calendrier dans une série périodique à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 9f78ef5b51766a69d23fce3f36c55fbb9422fb16
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754784"
---
# <a name="access-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="7d131-103">Accéder à une série périodique à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7d131-103">Access a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="7d131-104">Découvrez comment accéder aux éléments de calendrier dans une série périodique à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d131-104">Learn how to access calendar items in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="7d131-105">Une série de rendez-vous ou réunions périodiques est composée d’une forme de base périodique, un nombre d’occurrences d’une série qui se répètent en fonction d’un modèle défini et, éventuellement, les ensembles d’occurrences qui ont été modifiées et qui ont été supprimés.</span><span class="sxs-lookup"><span data-stu-id="7d131-105">A recurring series of appointments or meetings is made up of a recurring master, a number of occurrences in a series that repeat according to a set pattern, and, optionally, sets of occurrences that were changed and that were deleted.</span></span> <span data-ttu-id="7d131-106">Vous pouvez utiliser les API managées EWS pour accéder aux éléments de calendrier dans une série périodique.</span><span class="sxs-lookup"><span data-stu-id="7d131-106">You can use the EWS Managed API or EWS to access calendar items in a recurring series.</span></span> <span data-ttu-id="7d131-107">Cela vous permet de :</span><span class="sxs-lookup"><span data-stu-id="7d131-107">This enables you to:</span></span>
  
- <span data-ttu-id="7d131-108">Vérifie si un élément de calendrier associé à un ID d’élément est une forme de base périodique, une occurrence d’une série ou d’une exception à une série.</span><span class="sxs-lookup"><span data-stu-id="7d131-108">Check to see if a calendar item associated with an item ID is a recurring master, an occurrence in a series, or an exception to a series.</span></span>
    
- <span data-ttu-id="7d131-109">Rechercher votre dossier de calendrier pour les rendez-vous de périodicité.</span><span class="sxs-lookup"><span data-stu-id="7d131-109">Search your calendar folder for recurrence appointments.</span></span>
    
- <span data-ttu-id="7d131-110">Obtenir des éléments de calendrier périodicité connexe</span><span class="sxs-lookup"><span data-stu-id="7d131-110">Get related recurrence calendar items</span></span>
    
- <span data-ttu-id="7d131-111">Itérez occurrences dans une série, exceptions occurrence ou suppressions occurrence.</span><span class="sxs-lookup"><span data-stu-id="7d131-111">Iterate through occurrences in a series, occurrence exceptions, or occurrence deletions.</span></span>
    
## <a name="get-a-collection-of-recurring-calendar-items-by-using-the-ews-managed-api"></a><span data-ttu-id="7d131-112">Obtenir une collection d’éléments de calendrier périodique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="7d131-112">Get a collection of recurring calendar items by using the EWS Managed API</span></span>

<span data-ttu-id="7d131-113">Si vous souhaitez récupérer une collection de rendez-vous, vous pouvez utiliser la méthode [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) pour extraire tous les rendez-vous entre une date de début et de fin donnée et puis ajoutez tous les éléments de calendrier avec un type de **Occurrence de rendez-vous **ou une **Exception** à une collection, comme illustré dans l’exemple suivant.</span><span class="sxs-lookup"><span data-stu-id="7d131-113">If you want to retrieve a collection of appointments, you can use the [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to retrieve all appointments between a given start and end date, and then add all calendar items with an appointment type of **Occurrence** or **Exception** to a collection, as shown in the following example.</span></span> 
  
<span data-ttu-id="7d131-114">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="7d131-114">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

<span data-ttu-id="7d131-115">Notez que les éléments de calendrier principal périodiques ne sont pas renvoyées dans un appel à **FindAppointments**.</span><span class="sxs-lookup"><span data-stu-id="7d131-115">Note that recurring master calendar items aren't returned in a call to **FindAppointments**.</span></span> <span data-ttu-id="7d131-116">Si vous souhaitez récupérer masters périodiques, ou une approche plus générale sur la récupération des éléments de calendrier, vous devez utiliser [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="7d131-116">If you want to retrieve recurring masters, or you want a more general approach to retrieving calendar items, you need to use [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="7d131-117">Vous pouvez ensuite utiliser un filtre de recherche pour récupérer uniquement les éléments avec une date de début supérieure ou égale à la date de que votre choix et un affichage de l’élément pour limiter le nombre d’éléments à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="7d131-117">You can then use a search filter to retrieve only items with a start date greater than or equal to a date you choose, and an item view to limit the number of items to return.</span></span> <span data-ttu-id="7d131-118">Notez qu’une forme de base périodique avec un démarrage date antérieures à la date de début de votre recherche ne sera pas trouvée, même si les occurrences se produisent dans cette plage.</span><span class="sxs-lookup"><span data-stu-id="7d131-118">Note that a recurring master with a start date earlier than the start date in your search will not be found, even if occurrences occur in this range.</span></span>
  
<span data-ttu-id="7d131-119">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="7d131-119">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

## <a name="get-related-recurrence-calendar-items-by-using-the-ews-managed-api"></a><span data-ttu-id="7d131-120">Obtenir des éléments de calendrier de périodicité associée à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="7d131-120">Get related recurrence calendar items by using the EWS Managed API</span></span>

<span data-ttu-id="7d131-121">Vous devez parfois une partie du puzzle, mais pour résoudre ce problème, vous devez le reste des éléments.</span><span class="sxs-lookup"><span data-stu-id="7d131-121">Sometimes you have one piece of the puzzle, but to solve it you need the rest of the pieces.</span></span> <span data-ttu-id="7d131-122">Si vous avez l’ID d’élément pour un élément de calendrier périodicité, vous pouvez obtenir les autres éléments que vous avez besoin à l’aide de plusieurs propriétés de l’API managée EWS ou méthodes.</span><span class="sxs-lookup"><span data-stu-id="7d131-122">If you have the item ID for a recurrence calendar item, you can get the other pieces you need by using one of several EWS Managed API properties or methods.</span></span>
  
<span data-ttu-id="7d131-123">**Le tableau 1. API managée EWS propriété ou méthode à utiliser pour obtenir des éléments de calendrier de périodicité connexe**</span><span class="sxs-lookup"><span data-stu-id="7d131-123">**Table 1. EWS Managed API property or method to use to get related recurrence calendar items**</span></span>

|<span data-ttu-id="7d131-124">**Si vous avez l’ID d’élément pour...**</span><span class="sxs-lookup"><span data-stu-id="7d131-124">**If you have the item ID for…**</span></span>|<span data-ttu-id="7d131-125">**Vous pouvez obtenir...**</span><span class="sxs-lookup"><span data-stu-id="7d131-125">**You can get…**</span></span>|<span data-ttu-id="7d131-126">**À l’aide de la...**</span><span class="sxs-lookup"><span data-stu-id="7d131-126">**By using the…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7d131-127">L’élément de calendrier principal périodique</span><span class="sxs-lookup"><span data-stu-id="7d131-127">The recurring master calendar item</span></span>  <br/> | <span data-ttu-id="7d131-128">La première occurrence d’une série</span><span class="sxs-lookup"><span data-stu-id="7d131-128">The first occurrence in a series</span></span>  <br/>  <span data-ttu-id="7d131-129">La dernière occurrence d’une série</span><span class="sxs-lookup"><span data-stu-id="7d131-129">The last occurrence in a series</span></span>  <br/>  <span data-ttu-id="7d131-130">Les exceptions à une série</span><span class="sxs-lookup"><span data-stu-id="7d131-130">The exceptions to a series</span></span>  <br/>  <span data-ttu-id="7d131-131">Les rendez-vous supprimés d’une série</span><span class="sxs-lookup"><span data-stu-id="7d131-131">The deleted appointments in a series</span></span>  <br/>  <span data-ttu-id="7d131-132">Toutes les occurrences (fonction de son index)</span><span class="sxs-lookup"><span data-stu-id="7d131-132">Any occurrence (given its index)</span></span>  <br/> |<span data-ttu-id="7d131-133">Propriété [Appointment.FirstOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7d131-133">[Appointment.FirstOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.firstoccurrence%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="7d131-134">Propriété [Appointment.LastOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7d131-134">[Appointment.LastOccurrence](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.lastoccurrence%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="7d131-135">Propriété [Appointment.ModifiedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7d131-135">[Appointment.ModifiedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.modifiedoccurrences%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="7d131-136">Propriété [Appointment.DeletedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7d131-136">[Appointment.DeletedOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.deletedoccurrences%28v=exchg.80%29.aspx) property</span></span>  <br/> <span data-ttu-id="7d131-137">Méthode [Appointment.BindToOccurrence](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7d131-137">[Appointment.BindToOccurrence](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtooccurrence%28v=exchg.80%29.aspx) method</span></span>  <br/> |
|<span data-ttu-id="7d131-138">Une seule occurrence d’une série</span><span class="sxs-lookup"><span data-stu-id="7d131-138">A single occurrence in a series</span></span>  <br/> |<span data-ttu-id="7d131-139">La forme de base périodique</span><span class="sxs-lookup"><span data-stu-id="7d131-139">The recurring master</span></span>  <br/> |<span data-ttu-id="7d131-140">Méthode [Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7d131-140">[Appointment.BindToRecurringMaster](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.bindtorecurringmaster%28v=exchg.80%29.aspx) method</span></span>  <br/> |
|<span data-ttu-id="7d131-141">Les éléments de calendrier (un objet [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) )</span><span class="sxs-lookup"><span data-stu-id="7d131-141">Any calendar item (an [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object)</span></span>  <br/> |<span data-ttu-id="7d131-142">La valeur d’énumération de [type de rendez-vous](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7d131-142">The [appointment type](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointmenttype%28v=exchg.80%29.aspx) enumeration value</span></span>  <br/> |<span data-ttu-id="7d131-143">Propriété [Appointment.AppointmentType](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7d131-143">[Appointment.AppointmentType](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.appointment.appointmenttype%28v=exchg.80%29.aspx) property</span></span>  <br/> |
   
<span data-ttu-id="7d131-144">L’exemple de code suivant montre comment obtenir une forme de base périodique, la première ou dernière occurrence d’une série ou d’une fonction de son index.</span><span class="sxs-lookup"><span data-stu-id="7d131-144">The following code example shows how to get a recurring master, the first or last occurrence in a series, or an occurrence given its index.</span></span>
  
<span data-ttu-id="7d131-145">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="7d131-145">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

## <a name="access-calendar-items-in-a-recurring-series-by-using-ews"></a><span data-ttu-id="7d131-146">Accéder aux éléments de calendrier dans une série périodique à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="7d131-146">Access calendar items in a recurring series by using EWS</span></span>

<span data-ttu-id="7d131-147">Accès aux éléments de calendrier dans une série périodique est très similaire à l’accès aux instances d’éléments de calendrier.</span><span class="sxs-lookup"><span data-stu-id="7d131-147">Accessing calendar items in a recurring series is very similar to accessing single instances of calendar items.</span></span> <span data-ttu-id="7d131-148">Vous utilisez une demande d’opération [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) , spécifiant les propriétés souhaitées, avec [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) de l’instance d’un rendez-vous dont vous avez besoin.</span><span class="sxs-lookup"><span data-stu-id="7d131-148">You use a [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request, specifying the properties you want, with the [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) of the appointment instance you need.</span></span> <span data-ttu-id="7d131-149">[OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) contient l' **ItemID** de master périodique de l’occurrence, ainsi que sa valeur d’index de la série.</span><span class="sxs-lookup"><span data-stu-id="7d131-149">The [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) contains the **ItemID** of the occurrence's recurring master, as well as its index value in the series.</span></span> 
  
<span data-ttu-id="7d131-150">Le code XML suivant montre la demande [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) permet de retourner une occurrence d’une série spécifiée par son index.</span><span class="sxs-lookup"><span data-stu-id="7d131-150">The following XML shows the [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) request used to return an occurrence in a series specified by its index.</span></span> <span data-ttu-id="7d131-151">Notez que l' **ItemID** du principal périodique a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="7d131-151">Note that the **ItemID** of the recurring master has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="7d131-152">Le serveur répond à la demande de **GetItem** avec un message [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que le courrier électronique a été créé avec succès et l' [ID d’élément](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de la nouvelle message créé.</span><span class="sxs-lookup"><span data-stu-id="7d131-152">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7d131-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7d131-153">See also</span></span>


- [<span data-ttu-id="7d131-154">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7d131-154">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
- [<span data-ttu-id="7d131-155">Obtenir des rendez-vous et réunions à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7d131-155">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

