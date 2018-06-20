---
title: Supprimer un rendez-vous périodique à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Découvrez comment supprimer un rendez-vous périodique à l’aide de l’API managée EWS ou EWS dans Exchange.
ms.openlocfilehash: 5e4d95058808adf8db159000bdf90c1f92945338
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754844"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="7bcec-103">Supprimer un rendez-vous périodique à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7bcec-103">Delete appointments in a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="7bcec-104">Découvrez comment supprimer un rendez-vous périodique à l’aide de l’API managée EWS ou EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bcec-104">Learn how to delete appointments in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="7bcec-105">Vous pouvez utiliser les API managées EWS pour supprimer une série de rendez-vous ou réunions, ou une instance unique de la série.</span><span class="sxs-lookup"><span data-stu-id="7bcec-105">You can use the EWS Managed API or EWS to delete a series of appointments or meetings, or just one instance in the series.</span></span> <span data-ttu-id="7bcec-106">Le processus que vous permet de supprimer une série entière est pratiquement identique à la procédure pour supprimer uniquement une occurrence unique.</span><span class="sxs-lookup"><span data-stu-id="7bcec-106">The process you use to delete an entire series is essentially the same as the process you use to delete just a single occurrence.</span></span> <span data-ttu-id="7bcec-107">Vous utilisez les mêmes méthodes API managées ou opérations EWS qui vous permet de [Supprimer une réunion ou un rendez-vous unique](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="7bcec-107">You use the same EWS Managed API methods or EWS operations that you use to [delete a single instance appointment or meeting](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="7bcec-108">La différence réside dans l’ID d’élément qui est inclus dans la méthode ou l’opération.</span><span class="sxs-lookup"><span data-stu-id="7bcec-108">The difference is in the item ID that is included in the method or operation.</span></span> <span data-ttu-id="7bcec-109">Commençons par à la façon dont les deux scénarios sont les mêmes.</span><span class="sxs-lookup"><span data-stu-id="7bcec-109">Let's start by looking at how both scenarios are the same.</span></span> 
  
<span data-ttu-id="7bcec-110">Pour supprimer une série périodique, soit une seule occurrence d’une série périodique, vous devez rechercher l’occurrence ou la série que vous souhaitez supprimer, puis appelez la méthode appropriée ou l’opération à supprimer.</span><span class="sxs-lookup"><span data-stu-id="7bcec-110">In order to delete a recurring series or a single occurrence in a recurring series, you need to find the occurrence or series that you want to delete, and then call the appropriate method or operation to remove it.</span></span> <span data-ttu-id="7bcec-111">Vous pouvez simplement supprimer n’importe quel type de rendez-vous, nous vous recommandons de n’importe quel participants ou l’organisateur de la mise à jour et annuler les réunions que l’utilisateur a organisé et refuser l’utilisateur ne pas organiser les réunions.</span><span class="sxs-lookup"><span data-stu-id="7bcec-111">While you can simply delete any type of appointment, we recommend that you keep any attendees or the organizer up to date and cancel meetings that the user has organized and decline meetings that the user did not organize.</span></span>
  
<span data-ttu-id="7bcec-112">Comment sont donc les scénarios différents ?</span><span class="sxs-lookup"><span data-stu-id="7bcec-112">So how are the scenarios different?</span></span> <span data-ttu-id="7bcec-113">Il est axé sur l’objet [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) utilisé pour appeler la méthode (pour l’API managée EWS) ou l’ID d’élément inclus dans la requête d’opération (pour EWS).</span><span class="sxs-lookup"><span data-stu-id="7bcec-113">It's all about the [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object used to invoke the method (for the EWS Managed API) or the item ID included in the operation request (for EWS).</span></span> <span data-ttu-id="7bcec-114">Pour supprimer une série entière, vous devez l’ID d’objet ou d’un élément de **rendez-vous** pour le contrôleur périodique.</span><span class="sxs-lookup"><span data-stu-id="7bcec-114">To delete an entire series, you need the **Appointment** object or item ID for the recurring master.</span></span> <span data-ttu-id="7bcec-115">Pour supprimer une seule occurrence, vous devez l’ID d’objet ou d’un élément de **rendez-vous** pour l’occurrence.</span><span class="sxs-lookup"><span data-stu-id="7bcec-115">To delete a single occurrence, you need the **Appointment** object or item ID for the occurrence.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="7bcec-116">Supprimer un rendez-vous périodique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="7bcec-116">Delete a recurring appointment by using the EWS Managed API</span></span>

<span data-ttu-id="7bcec-117">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="7bcec-117">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="7bcec-118">Le paramètre _recurringItem_ est un objet de **rendez-vous** pour le contrôleur périodique ou une seule occurrence.</span><span class="sxs-lookup"><span data-stu-id="7bcec-118">The  _recurringItem_ parameter is an **Appointment** object for either the recurring master or a single occurrence.</span></span> <span data-ttu-id="7bcec-119">Le paramètre _deleteEntireSeries_ indique s’il faut supprimer la série entière faisant partie de la _recurringItem_ .</span><span class="sxs-lookup"><span data-stu-id="7bcec-119">The  _deleteEntireSeries_ parameter indicates whether to delete the entire series that the  _recurringItem_ is a part of.</span></span> 
  
```cs
public static bool DeleteRecurringItem(ExchangeService service, Appointment recurringItem, bool deleteEntireSeries)
{
    Appointment appointmentToDelete = null;
    // If the item is a single appointment, fail.
    if (recurringItem.AppointmentType == AppointmentType.Single)
    {
        Console.WriteLine("ERROR: The item to delete is not part of a recurring series.");
        return false;
    }
    // Check the Appointment that was passed. Is it
    // an occurrence or the recurring master?
    if (recurringItem.AppointmentType == AppointmentType.RecurringMaster)
    {
        if (!deleteEntireSeries)
        {
            // The item is the recurring master, so deleting it will delete
            // the entire series. The caller indicated that the entire series
            // should not be deleted, so fail.
            Console.WriteLine("ERROR: The item to delete is the recurring master of the series. Deleting it will delete the entire series.");
            return false;
        }
        else
        {
            appointmentToDelete = recurringItem;
        }
    }
    else
    {
        if (deleteEntireSeries)
        {
            // The item passed is not the recurring master, but the caller
            // wants to delete the entire series. Bind to the recurring
            // master to delete it.
            try
            {
                appointmentToDelete = Appointment.BindToRecurringMaster(service, recurringItem.Id);
            }
            catch (Exception ex)
            {
                Console.WriteLine("ERROR: {0}", ex.Message);
                return false;
            }
        }
        else
        {
            // The item passed is not the recurring master, but the caller
            // only wants to delete the occurrence, so just
            // delete the passed item.
            appointmentToDelete = recurringItem;
        }
    }
    if (appointmentToDelete != null)
    {
        // Remove the item, depending on the scenario. 
        if (appointmentToDelete.IsMeeting)
        {
            CalendarActionResults results;
            // If it's a meeting and the user is the organizer, cancel it.
            // Determine this by testing the AppointmentState bitmask for 
            // the presence of the second bit. This bit indicates that the appointment
            // was received, which means that someone sent it to the user. Therefore,
            // they're not the organizer.
            int isReceived = 2;
            if ((appointmentToDelete.AppointmentState &amp; isReceived) == 0)
            {
                results = appointmentToDelete.CancelMeeting("Cancelling this meeting.");
                return true;
            }
            // If it's a meeting and the user is not the organizer, decline it.
            else
            {
                results = appointmentToDelete.Decline(true);
                return true;
            }
        }
        else
        {
            // The item isn't a meeting, so just delete it.
            appointmentToDelete.Delete(DeleteMode.MoveToDeletedItems);
            return true;
        }
    }
    return false;
}
```

<span data-ttu-id="7bcec-120">Pour pouvoir utiliser cet exemple, vous devez [lier à une occurrence ou de la forme de base périodique](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)et passez l’objet résultant de **rendez-vous** à la méthode.</span><span class="sxs-lookup"><span data-stu-id="7bcec-120">In order to use this example, you need to [bind to either an occurrence or the recurring master](how-to-access-a-recurring-series-by-using-ews-in-exchange.md), and pass the resulting **Appointment** object to the method.</span></span> <span data-ttu-id="7bcec-121">N’oubliez pas que si vous accédez rendez-vous à l’aide d’une classe [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) , les éléments qui en résulte sont toutes les occurrences uniques.</span><span class="sxs-lookup"><span data-stu-id="7bcec-121">Keep in mind that if you access appointments by using a [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) class, the resulting items are all single occurrences.</span></span> <span data-ttu-id="7bcec-122">Inversement, si vous utilisez la classe [l’annonceAfficher le](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) , les éléments qui en résulte sont toutes les formes de base périodiques.</span><span class="sxs-lookup"><span data-stu-id="7bcec-122">Conversely, if you use the [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) class, the resulting items are all recurring masters.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a><span data-ttu-id="7bcec-123">Supprimer un rendez-vous périodique à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="7bcec-123">Delete a recurring appointment by using EWS</span></span>

<span data-ttu-id="7bcec-124">Suppression d’une série périodique à l’aide de EWS est identique à la [suppression d’une seule instance de réunion](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="7bcec-124">Deleting a recurring series by using EWS is the same as [deleting a single-instance meeting](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="7bcec-125">En fait, les demandes SOAP prennent le même format.</span><span class="sxs-lookup"><span data-stu-id="7bcec-125">In fact, the SOAP requests take the same format.</span></span> <span data-ttu-id="7bcec-126">Là encore, la clé est l’ID d’élément utilisé dans la demande.</span><span class="sxs-lookup"><span data-stu-id="7bcec-126">Again, the key is the item ID used in the request.</span></span> <span data-ttu-id="7bcec-127">Si l’ID d’élément correspond à la forme de base périodique, la série entière sera supprimée.</span><span class="sxs-lookup"><span data-stu-id="7bcec-127">If the item ID corresponds to the recurring master, the entire series will be deleted.</span></span> <span data-ttu-id="7bcec-128">Si l’ID d’élément correspond à une seule occurrence, seule cette occurrence sera supprimée.</span><span class="sxs-lookup"><span data-stu-id="7bcec-128">If the item ID corresponds to a single occurrence, only that occurrence will be deleted.</span></span>
  
> [!NOTE]
> <span data-ttu-id="7bcec-129">Dans les exemples de code qui suivent, les attributs **ItemId**, **ChangeKey**et **RecurringMasterId** sont raccourcis pour une meilleure lisibilité.</span><span class="sxs-lookup"><span data-stu-id="7bcec-129">In the code examples that follow, the **ItemId**, **ChangeKey**, and **RecurringMasterId** attributes are shortened for readability.</span></span> 
  
<span data-ttu-id="7bcec-130">Cet exemple utilise l' [opération CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) avec un élément [CancelCalendarItem](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) d’annuler une réunion pour laquelle l’utilisateur est l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="7bcec-130">This example uses the [CreateItem operation](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) with a [CancelCalendarItem](http://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) element to cancel a meeting for which the user is the organizer.</span></span> <span data-ttu-id="7bcec-131">La valeur de l’élément [ReferenceItemId](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) indique l’élément à annuler, et peut être l’ID d’élément d’une forme de base périodique ou une seule occurrence.</span><span class="sxs-lookup"><span data-stu-id="7bcec-131">The value of the [ReferenceItemId](http://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) element indicates the item to cancel, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:CancelCalendarItem>
          <t:ReferenceItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
          <t:NewBodyContent BodyType="HTML">Cancelling this meeting.</t:NewBodyContent>
        </t:CancelCalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7bcec-132">Cet exemple utilise l' **opération CreateItem** avec un élément [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) pour refuser une réunion pour laquelle l’utilisateur n’est pas l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="7bcec-132">This example uses the **CreateItem operation** with a [DeclineItem](http://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) element to decline a meeting for which the user is not the organizer.</span></span> <span data-ttu-id="7bcec-133">Comme dans l’exemple précédent, la valeur de l’élément **ReferenceItemId** indique l’élément à refuser, et peut être l’ID d’élément d’une forme de base périodique ou une seule occurrence.</span><span class="sxs-lookup"><span data-stu-id="7bcec-133">As in the previous example, the value of the **ReferenceItemId** element indicates the item to decline, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:DeclineItem>
          <t:ReferenceItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
        </t:DeclineItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7bcec-134">Cet exemple utilise l' [opération DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) pour supprimer une seule occurrence d’un rendez-vous sans participants.</span><span class="sxs-lookup"><span data-stu-id="7bcec-134">This example uses the [DeleteItem operation](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) to delete a single occurrence of an appointment with no attendees.</span></span> <span data-ttu-id="7bcec-135">L’occurrence à supprimer est spécifiée par l’élément [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) , qui est construit à partir de l’ID d’élément de la forme de base périodique et l’index de l’occurrence.</span><span class="sxs-lookup"><span data-stu-id="7bcec-135">The occurrence to delete is specified by the [OccurrenceItemId](http://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) element, which is constructed from the item ID of the recurring master and the index of the occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems" SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:OccurrenceItemId RecurringMasterId="AAMkADA8..." InstanceIndex="3" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7bcec-136">Notez que vous pouvez obtenir le même résultat en remplaçant l’élément **OccurrenceItemId** avec un élément [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) qui contient l’ID d’élément de l’occurrence, comme indiqué.</span><span class="sxs-lookup"><span data-stu-id="7bcec-136">Note that you can get the same result by replacing the **OccurrenceItemId** element with an [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element that contains the item ID of the occurrence, as shown.</span></span> 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a><span data-ttu-id="7bcec-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7bcec-137">See also</span></span>


- [<span data-ttu-id="7bcec-138">Périodicités et EWS</span><span class="sxs-lookup"><span data-stu-id="7bcec-138">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="7bcec-139">Accéder à une série périodique à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7bcec-139">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="7bcec-140">Créer une série périodique à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7bcec-140">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="7bcec-141">Mise à jour d’une série périodique à l’aide de EWS</span><span class="sxs-lookup"><span data-stu-id="7bcec-141">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="7bcec-142">Mise à jour d’une série périodique à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7bcec-142">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="7bcec-143">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7bcec-143">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="7bcec-144">Créer des rendez-vous et réunions à l’aide de EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="7bcec-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="7bcec-145">Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7bcec-145">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

