---
title: Supprimer des rendez-vous dans une série périodique à l’aide d’EWS Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: a9d5244a-bc4a-4e9c-9c6c-ff361e04cbf8
description: Découvrez comment supprimer des rendez-vous dans une série périodique à l’aide de l’API gérée EWS ou EWS dans Exchange.
ms.openlocfilehash: 8a68b6655c98f290d569a14dc0ac518c5d875cbe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513191"
---
# <a name="delete-appointments-in-a-recurring-series-by-using-ews-in-exchange"></a>Supprimer des rendez-vous dans une série périodique à l’aide d’EWS Exchange

Découvrez comment supprimer des rendez-vous dans une série périodique à l’aide de l’API gérée EWS ou EWS dans Exchange.
  
Vous pouvez utiliser l’API gérée EWS ou EWS pour supprimer une série de rendez-vous ou de réunions, ou une seule instance de la série. Le processus que vous utilisez pour supprimer une série entière est essentiellement le même que celui que vous utilisez pour supprimer une seule occurrence. Vous utilisez les mêmes méthodes d’API gérées EWS ou opérations EWS que vous utilisez pour supprimer un rendez-vous ou [une réunion d’instance unique.](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md) La différence est l’ID d’élément inclus dans la méthode ou l’opération. Commençons par voir comment les deux scénarios sont identiques. 
  
Pour supprimer une série périodique ou une occurrence unique d’une série périodique, vous devez rechercher l’occurrence ou la série à supprimer, puis appeler la méthode ou l’opération appropriée pour la supprimer. Bien que vous pouvez simplement supprimer n’importe quel type de rendez-vous, nous vous recommandons de tenir à jour tous les participants ou l’organisateur et d’annuler les réunions que l’utilisateur a organisées et de refuser les réunions qu’il n’a pas organisées.
  
En quoi les scénarios sont-ils différents ? Il s’agit de l’objet [Appointment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) utilisé pour appeler la méthode (pour l’API gérée EWS) ou l’ID d’élément inclus dans la demande d’opération (pour EWS). Pour supprimer une série entière, vous avez besoin de l’objet **Appointment** ou de l’ID d’élément pour le récurrent. Pour supprimer une occurrence unique, vous avez besoin de l’objet **Appointment** ou de l’ID d’élément pour l’occurrence. 
  
## <a name="delete-a-recurring-appointment-by-using-the-ews-managed-api"></a>Supprimer un rendez-vous périodique à l’aide de l’API gérée EWS

Cet exemple suppose que vous ont été authentifiés auprès d'un serveur Exchange et que vous avez acquis un [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**. Le  _paramètre recurringItem_ est un objet **Appointment** pour la récurrable maître ou une occurrence unique. Le  _paramètre deleteEntireSeries_ indique s’il faut supprimer la série entière dont l’élément  _recurringItem_ fait partie. 
  
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

Pour utiliser cet exemple, vous devez lier une occurrence ou la récurration [principale](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)et transmettre l’objet **Appointment** résultant à la méthode. N’oubliez pas que si vous accédez à des rendez-vous à l’aide d’une [classe CalendarView,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) les éléments résultants sont tous des occurrences simples. À l’inverse, si vous utilisez la [classe ItemView,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) les éléments résultants sont tous des maîtres périodiques. 
  
## <a name="delete-a-recurring-appointment-by-using-ews"></a>Supprimer un rendez-vous périodique à l’aide d’EWS

La suppression d’une série périodique à l’aide d’EWS est identique à la suppression [d’une réunion à instance unique.](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md) En fait, les requêtes SOAP prennent le même format. Là encore, la clé est l’ID d’élément utilisé dans la demande. Si l’ID d’élément correspond au maître périodique, la série entière est supprimée. Si l’ID d’élément correspond à une occurrence unique, seule cette occurrence sera supprimée.
  
> [!NOTE]
> Dans les exemples de code qui suivent, les attributs **ItemId,** **ChangeKey** et **RecurringMasterId** sont raccourcis pour des raisons de lisibilité. 
  
Cet exemple utilise [l’opération CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) avec un [élément CancelCalendarItem](https://msdn.microsoft.com/library/a2046402-a176-44d5-b4b3-adb696581935%28Office.15%29.aspx) pour annuler une réunion dont l’utilisateur est l’organisateur. La valeur de [l’élément ReferenceItemId](https://msdn.microsoft.com/library/8fd4bb12-a94b-43f5-be3b-f435684e311d%28Office.15%29.aspx) indique l’élément à annuler et peut être l’ID d’un élément principal périodique ou une occurrence unique. 
  
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

Cet exemple utilise **l’opération CreateItem** avec un [élément DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) pour refuser une réunion dont l’utilisateur n’est pas l’organisateur. Comme dans l’exemple précédent, la valeur de l’élément **ReferenceItemId** indique l’élément à refuser et peut être l’ID d’élément d’une récurration principale ou d’une occurrence unique. 
  
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

Cet exemple utilise [l’opération DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) pour supprimer une occurrence unique d’un rendez-vous sans participants. L’occurrence à supprimer est spécifiée par [l’élément OccurrenceItemId,](https://msdn.microsoft.com/library/4a15bbc3-5b93-4193-b9ec-da32f0a9a552%28Office.15%29.aspx) qui est construit à partir de l’ID d’élément de la référence périodique et de l’index de l’occurrence. 
  
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

Notez que vous pouvez obtenir le même résultat en remplaçant l’élément **OccurrenceItemId** par un [élément ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) qui contient l’ID d’élément de l’occurrence, comme illustré. 
  
```XML
<m:ItemIds>
  <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
</m:ItemIds>

```

## <a name="see-also"></a>Voir aussi


- [Périodicités et EWS](recurrence-patterns-and-ews.md)
    
- [Accéder à une série périodique à l’aide d’EWS dans Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Créer une série périodique à l’aide d’EWS dans Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Mettre à jour une série périodique à l’aide d’EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Mettre à jour une série périodique à l’aide d’EWS Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
    
- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

