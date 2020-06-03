---
title: Supprimer des rendez-vous dans une série périodique à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Découvrez comment supprimer des rendez-vous dans une série périodique à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: 5646a30d218ed4d795044aefe5efea1399d19a79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528124"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a><span data-ttu-id="4b11f-103">Supprimer des rendez-vous dans une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b11f-103">Delete appointments in a recurring series by using EWS in Exchange</span></span>

<span data-ttu-id="4b11f-104">Découvrez comment supprimer des rendez-vous dans une série périodique à l’aide de l’API managée EWS ou d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b11f-104">Learn how to delete appointments in a recurring series by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="4b11f-105">Vous pouvez utiliser l’API managée EWS ou EWS pour supprimer une série de rendez-vous ou de réunions, ou une seule instance de la série.</span><span class="sxs-lookup"><span data-stu-id="4b11f-105">You can use the EWS Managed API or EWS to delete a series of appointments or meetings, or just one instance in the series.</span></span> <span data-ttu-id="4b11f-106">Le processus que vous utilisez pour supprimer une série entière est essentiellement le même que le processus que vous utilisez pour supprimer une seule occurrence.</span><span class="sxs-lookup"><span data-stu-id="4b11f-106">The process you use to delete an entire series is essentially the same as the process you use to delete just a single occurrence.</span></span> <span data-ttu-id="4b11f-107">Vous utilisez les mêmes méthodes d’API managée EWS ou les mêmes opérations EWS que vous utilisez pour [supprimer un rendez-vous ou une réunion unique d’instance](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4b11f-107">You use the same EWS Managed API methods or EWS operations that you use to [delete a single instance appointment or meeting](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="4b11f-108">La différence réside dans l’ID d’élément qui est inclus dans la méthode ou l’opération.</span><span class="sxs-lookup"><span data-stu-id="4b11f-108">The difference is in the item ID that is included in the method or operation.</span></span> <span data-ttu-id="4b11f-109">Commençons par examiner la manière dont les deux scénarios sont les mêmes.</span><span class="sxs-lookup"><span data-stu-id="4b11f-109">Let's start by looking at how both scenarios are the same.</span></span> 
  
<span data-ttu-id="4b11f-110">Pour supprimer une série périodique ou une occurrence unique dans une série périodique, vous devez Rechercher l’occurrence ou la série que vous souhaitez supprimer, puis appeler la méthode ou l’opération appropriée pour la supprimer.</span><span class="sxs-lookup"><span data-stu-id="4b11f-110">In order to delete a recurring series or a single occurrence in a recurring series, you need to find the occurrence or series that you want to delete, and then call the appropriate method or operation to remove it.</span></span> <span data-ttu-id="4b11f-111">Bien que vous puissiez simplement supprimer n’importe quel type de rendez-vous, nous vous recommandons de conserver les participants ou l’organisateur à jour et d’annuler les réunions que l’utilisateur a organisées et de refuser les réunions que l’utilisateur n’a pas organisé.</span><span class="sxs-lookup"><span data-stu-id="4b11f-111">While you can simply delete any type of appointment, we recommend that you keep any attendees or the organizer up to date and cancel meetings that the user has organized and decline meetings that the user did not organize.</span></span>
  
<span data-ttu-id="4b11f-112">Comment les scénarios sont-ils différents ?</span><span class="sxs-lookup"><span data-stu-id="4b11f-112">So how are the scenarios different?</span></span> <span data-ttu-id="4b11f-113">Il s’agit de l’objet de [rendez-vous](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) utilisé pour appeler la méthode (pour l’API managée EWS) ou de l’ID d’élément inclus dans la demande d’opération (pour EWS).</span><span class="sxs-lookup"><span data-stu-id="4b11f-113">It's all about the [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object used to invoke the method (for the EWS Managed API) or the item ID included in the operation request (for EWS).</span></span> <span data-ttu-id="4b11f-114">Pour supprimer une série entière, vous avez besoin de l’objet ou de l’ID d’élément de **rendez-** vous pour la forme de base périodique.</span><span class="sxs-lookup"><span data-stu-id="4b11f-114">To delete an entire series, you need the **Appointment** object or item ID for the recurring master.</span></span> <span data-ttu-id="4b11f-115">Pour supprimer une seule occurrence, vous avez besoin de l’objet ou de l’ID d’élément de **rendez-** vous pour l’occurrence.</span><span class="sxs-lookup"><span data-stu-id="4b11f-115">To delete a single occurrence, you need the **Appointment** object or item ID for the occurrence.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="4b11f-116">Supprimer un rendez-vous périodique à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="4b11f-116">Delete a recurring appointment by using the EWS Managed API</span></span>

<span data-ttu-id="4b11f-117">Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService ](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span><span class="sxs-lookup"><span data-stu-id="4b11f-117">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="4b11f-118">Le paramètre _recurringItem_ est un objet de **rendez-vous** pour le masque périodique ou une seule occurrence.</span><span class="sxs-lookup"><span data-stu-id="4b11f-118">The  _recurringItem_ parameter is an **Appointment** object for either the recurring master or a single occurrence.</span></span> <span data-ttu-id="4b11f-119">Le paramètre _deleteEntireSeries_ indique s’il faut supprimer la totalité de la série dont fait partie l' _recurringItem_ .</span><span class="sxs-lookup"><span data-stu-id="4b11f-119">The  _deleteEntireSeries_ parameter indicates whether to delete the entire series that the  _recurringItem_ is a part of.</span></span> 
  
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

<span data-ttu-id="4b11f-120">Pour utiliser cet exemple, vous devez [établir une liaison avec une occurrence ou la forme de base périodique](how-to-access-a-recurring-series-by-using-ews-in-exchange.md), et transmettre l’objet de **rendez-vous** résultant à la méthode.</span><span class="sxs-lookup"><span data-stu-id="4b11f-120">In order to use this example, you need to [bind to either an occurrence or the recurring master](how-to-access-a-recurring-series-by-using-ews-in-exchange.md), and pass the resulting **Appointment** object to the method.</span></span> <span data-ttu-id="4b11f-121">N’oubliez pas que si vous accédez à des rendez-vous à l’aide d’une classe [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) , les éléments résultants sont toutes des occurrences uniques.</span><span class="sxs-lookup"><span data-stu-id="4b11f-121">Keep in mind that if you access appointments by using a [CalendarView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) class, the resulting items are all single occurrences.</span></span> <span data-ttu-id="4b11f-122">À l’inverse, si vous utilisez la classe [objetitemview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) , les éléments résultants sont tous des masques périodiques.</span><span class="sxs-lookup"><span data-stu-id="4b11f-122">Conversely, if you use the [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) class, the resulting items are all recurring masters.</span></span> 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a><span data-ttu-id="4b11f-123">Supprimer un rendez-vous périodique à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="4b11f-123">Delete a recurring appointment by using EWS</span></span>

<span data-ttu-id="4b11f-124">La suppression d’une série périodique à l’aide d’EWS est identique à la [Suppression d’une réunion à instance unique](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4b11f-124">Deleting a recurring series by using EWS is the same as [deleting a single-instance meeting](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="4b11f-125">En fait, les demandes SOAP ont le même format.</span><span class="sxs-lookup"><span data-stu-id="4b11f-125">In fact, the SOAP requests take the same format.</span></span> <span data-ttu-id="4b11f-126">Encore une fois, la clé est l’ID de l’élément utilisé dans la demande.</span><span class="sxs-lookup"><span data-stu-id="4b11f-126">Again, the key is the item ID used in the request.</span></span> <span data-ttu-id="4b11f-127">Si l’ID d’élément correspond à la forme de base périodique, la série entière sera supprimée.</span><span class="sxs-lookup"><span data-stu-id="4b11f-127">If the item ID corresponds to the recurring master, the entire series will be deleted.</span></span> <span data-ttu-id="4b11f-128">Si l’ID d’élément correspond à une seule occurrence, seule cette occurrence sera supprimée.</span><span class="sxs-lookup"><span data-stu-id="4b11f-128">If the item ID corresponds to a single occurrence, only that occurrence will be deleted.</span></span>
  
> [!NOTE]
> <span data-ttu-id="4b11f-129">Dans les exemples de code suivants, les attributs **ItemId**, **ChangeKey**et **recurringMasterId** sont raccourcis pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="4b11f-129">In the code examples that follow, the **ItemId**, **ChangeKey**, and **RecurringMasterId** attributes are shortened for readability.</span></span> 
  
<span data-ttu-id="4b11f-130">Cet exemple utilise l' [opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) avec un élément [CancelCalendarItem](https://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) pour annuler une réunion pour laquelle l’utilisateur est l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="4b11f-130">This example uses the [CreateItem operation](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) with a [CancelCalendarItem](https://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) element to cancel a meeting for which the user is the organizer.</span></span> <span data-ttu-id="4b11f-131">La valeur de l’élément [ReferenceItemId](https://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) indique l’élément à annuler, et peut être l’ID de l’élément d’une forme de base périodique ou une seule occurrence.</span><span class="sxs-lookup"><span data-stu-id="4b11f-131">The value of the [ReferenceItemId](https://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) element indicates the item to cancel, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="4b11f-132">Cet exemple utilise l' **opération CreateItem** avec un élément [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) pour refuser une réunion pour laquelle l’utilisateur n’est pas l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="4b11f-132">This example uses the **CreateItem operation** with a [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) element to decline a meeting for which the user is not the organizer.</span></span> <span data-ttu-id="4b11f-133">Comme dans l’exemple précédent, la valeur de l’élément **ReferenceItemId** indique l’élément à refuser et peut être l’ID de l’élément d’une forme de base périodique ou une seule occurrence.</span><span class="sxs-lookup"><span data-stu-id="4b11f-133">As in the previous example, the value of the **ReferenceItemId** element indicates the item to decline, and can be the item ID of a recurring master or a single occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="4b11f-134">Cet exemple utilise l' [opération DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) pour supprimer une seule occurrence d’un rendez-vous sans participants.</span><span class="sxs-lookup"><span data-stu-id="4b11f-134">This example uses the [DeleteItem operation](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) to delete a single occurrence of an appointment with no attendees.</span></span> <span data-ttu-id="4b11f-135">L’occurrence à supprimer est spécifiée par l’élément [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) , qui est construit à partir de l’ID d’élément de la forme de base périodique et de l’index de l’occurrence.</span><span class="sxs-lookup"><span data-stu-id="4b11f-135">The occurrence to delete is specified by the [OccurrenceItemId](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) element, which is constructed from the item ID of the recurring master and the index of the occurrence.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="4b11f-136">Notez que vous pouvez obtenir le même résultat en remplaçant l’élément **OccurrenceItemId** par un élément [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) qui contient l’ID d’élément de l’occurrence, comme illustré.</span><span class="sxs-lookup"><span data-stu-id="4b11f-136">Note that you can get the same result by replacing the **OccurrenceItemId** element with an [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element that contains the item ID of the occurrence, as shown.</span></span> 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a><span data-ttu-id="4b11f-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4b11f-137">See also</span></span>


- [<span data-ttu-id="4b11f-138">Périodicités et EWS</span><span class="sxs-lookup"><span data-stu-id="4b11f-138">Recurrence patterns and EWS</span></span>](recurrence-patterns-and-ews.md)
    
- [<span data-ttu-id="4b11f-139">Accéder à une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b11f-139">Access a recurring series by using EWS in Exchange</span></span>](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="4b11f-140">Créer une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b11f-140">Create a recurring series by using EWS in Exchange</span></span>](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="4b11f-141">Mettre à jour une série périodique à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="4b11f-141">Update a recurring series by using EWS</span></span>](how-to-update-a-recurring-series-by-using-ews.md)
    
- [<span data-ttu-id="4b11f-142">Mettre à jour une série périodique à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b11f-142">Update a recurring series by using EWS in Exchange</span></span>](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="4b11f-143">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b11f-143">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="4b11f-144">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="4b11f-144">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="4b11f-145">Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b11f-145">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

