---
title: Accéder à un calendrier en tant que délégué à l’aide d’EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Découvrez comment accéder à un calendrier en tant que délégué à l’aide de l’API managée EWS ou d’EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 20ec294ddc4ccf014f0b2148c786c8c3ef8a6069
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528292"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a>Accéder à un calendrier en tant que délégué à l’aide d’EWS dans Exchange

Découvrez comment accéder à un calendrier en tant que délégué à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
Vous pouvez utiliser l’API managée EWS ou EWS pour accorder à un utilisateur un accès délégué au dossier calendrier d’un propriétaire de boîte aux lettres. Le délégué peut ensuite créer des demandes de réunion pour le compte du propriétaire de la boîte aux lettres, créer des rendez-vous, répondre aux demandes de réunion et récupérer, mettre à jour et supprimer des réunions du dossier calendrier du propriétaire de la boîte aux lettres, en fonction de leurs autorisations.
  
En tant que délégué, vous utilisez les mêmes méthodes et opérations pour accéder au dossier de calendrier d’un propriétaire de boîte aux lettres que vous utilisez pour accéder à votre propre dossier de calendrier. La principale différence réside dans le fait que vous devez utiliser un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicit) pour rechercher ou créer un élément de calendrier ou un sous-dossier de calendrier, puis après avoir identifié l’ID d’élément ou l’ID de dossier, vous pouvez utiliser l' [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) pour obtenir, mettre à jour ou supprimer l’élément. 
  
**Tableau 1. Méthodes de l’API managée EWS et opérations EWS pour accéder à un calendrier en tant que délégué**

|**Si vous souhaitez...**|**Utilisez cette méthode d’API managée EWS...**|**Utilisez cette opération EWS...**|
|:-----|:-----|:-----|
|Créer une réunion ou un rendez-vous en tant que délégué  <br/> |[Rendez-vous. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) où le paramètre [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) fournit un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier calendrier du propriétaire de la boîte aux lettres  <br/> |[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) où l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie le [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres  <br/> |
|Créer plusieurs réunions ou rendez-vous en tant que délégué  <br/> |[ExchangeService. CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de calendrier du propriétaire de la boîte aux lettres  <br/> |[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) où l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie le [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres  <br/> |
|Rechercher ou Rechercher un rendez-vous ou une réunion en tant que délégué  <br/> |[ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) où le paramètre **FolderId** fournit un [accès explicite](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) au dossier de calendrier du propriétaire de la boîte aux lettres  <br/> |[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) où l’élément [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) spécifie le [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) du propriétaire de la boîte aux lettres  <br/> |
|Obtenir un rendez-vous ou une réunion en tant que délégué  <br/> |[Rendez-vous. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Mettre à jour un rendez-vous ou une réunion en tant que délégué  <br/> |Appointment [. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) suivi de [rendez-vous. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi de [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Supprimer un rendez-vous ou une réunion en tant que délégué  <br/> |[Rendez-vous. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) suivi de [rendez-vous.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , suivi de [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
> [!NOTE]
> Dans les exemples de code de cet article, primary@contoso.com est le propriétaire de la boîte aux lettres. 
  
## <a name="prerequisite-tasks"></a>Tâches préalables
<a name="bk_prereq"> </a>

Pour qu’un utilisateur puisse accéder au dossier calendrier d’un propriétaire de boîte aux lettres en tant que délégué, il doit être [ajouté en tant que délégué avec des autorisations](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) sur le dossier calendrier du propriétaire de la boîte aux lettres. 
  
Un délégué doit disposer d’une boîte aux lettres attachée à son compte pour mettre à jour le calendrier d’un propriétaire de boîte aux lettres.
  
Si un délégué doit travailler uniquement avec des demandes de réunion et des réponses, vous pouvez ajouter le délégué au dossier de calendrier et utiliser la valeur d’énumération de l’API managée EWS par défaut [MeetingRequestsDeliveryScope. DelegatesAndSendInformationToMe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) ou la valeur d’élément EWS [DeliverMeetingRequests](https://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) de **DelegatesAndSendInformationToMe** pour envoyer les demandes au délégué et aux messages d’information au propriétaire de la boîte aux lettres. Le délégué n’a alors pas besoin d’avoir accès au dossier boîte de réception du propriétaire de la boîte aux lettres. 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>Créer une réunion ou un rendez-vous en tant que délégué à l’aide de l’API managée EWS
<a name="bk_createewsma"> </a>

L’API managée EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué afin de créer des éléments de calendrier pour le propriétaire de la boîte aux lettres. Cet exemple montre comment utiliser la méthode [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) pour créer une réunion et envoyer des demandes de réunion aux participants. 
  
Cet exemple suppose que le **service** est un objet [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide pour le délégué et que le délégué bénéficie des autorisations appropriées pour le dossier calendrier du propriétaire de la boîte aux lettres. 
  
```cs
private static void DelegateAccessCreateMeeting(ExchangeService service)
{
    Appointment meeting = new Appointment(service);
    // Set the properties on the meeting object to create the meeting.
    meeting.Subject = "Team building exercise";
    meeting.Body = "Let's learn to really work as a team and then have lunch!";
    meeting.Start = DateTime.Now.AddDays(2);
    meeting.End = meeting.Start.AddHours(4);
    meeting.Location = "Conference Room 12";
    meeting.RequiredAttendees.Add("sadie@contoso.com");
    meeting.ReminderMinutesBeforeStart = 60;
    // Save the meeting to the Calendar folder for 
    // the mailbox owner and send the meeting request.
    // This method call results in a CreateItem call to EWS.
    meeting.Save(new FolderId(WellKnownFolderName.Calendar, 
        "primary@contoso.com"), 
        SendInvitationsMode.SendToAllAndSaveCopy);
    // Verify that the meeting was created.
    Item item = Item.Bind(service, meeting.Id, new PropertySet(ItemSchema.Subject));
    Console.WriteLine("\nMeeting created: " + item.Subject + "\n");
}
```

Notez que lorsque vous enregistrez l’élément, l’appel de la méthode [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) doit identifier le dossier calendrier du propriétaire de la boîte aux lettres. Si le dossier calendrier du propriétaire de la boîte aux lettres n’est pas spécifié, la demande de réunion est enregistrée dans le calendrier du délégué et non dans le dossier calendrier du propriétaire de la boîte aux lettres. Vous pouvez inclure le dossier calendrier du propriétaire de la boîte aux lettres dans l’appel de la méthode **Save** de deux manières. Nous vous recommandons d’instancier une nouvelle instance de l’objet [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) à l’aide de l' [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) et de l’adresse SMTP du propriétaire de la boîte aux lettres. 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

Toutefois, vous pouvez également [établir une liaison](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) avec le dossier de calendrier, puis utiliser l’ID du dossier dans l’appel de la méthode **Save** . Toutefois, sachez que cela crée un appel EWS supplémentaire. 
  
```cs
    // Identify the mailbox owner's SMTP address
    // and bind to their Calendar folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryCalendar = Folder.Bind(service, 
        new FolderId(WellKnownFolderName.Calendar, primary)); 
…
    // Save the meeting to the Calendar folder for the mailbox owner and send the meeting request.
    meeting.Save(primaryCalendar.Id, 
        SendInvitationsMode.SendToAllAndSaveCopy);
```

## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a>Créer une réunion ou un rendez-vous en tant que délégué à l’aide d’EWS
<a name="bk_createews"> </a>

EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué afin de créer des éléments de calendrier pour le propriétaire de la boîte aux lettres. Cet exemple montre comment utiliser l’opération [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) pour créer une réunion et envoyer des demandes de réunion aux participants. 
  
Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez la méthode **Save** pour [créer une réunion ou un rendez-vous en tant que délégué](#bk_createewsma).
  
L’en-tête SOAP a été supprimé de l’exemple suivant par souci de concision.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
         xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
…
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Team building exercise</t:Subject>
          <t:Body BodyType="HTML">Let's learn to really work as a 
              team and then have lunch!</t:Body>
          <t:ReminderMinutesBeforeStart>60</t:ReminderMinutesBeforeStart>
          <t:Start>2014-03-09T23:26:33.756-05:00</t:Start>
          <t:End>2014-03-10T03:26:33.756-05:00</t:End>
          <t:Location>Conference Room 12</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui inclut la valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NOERROR**, ce qui indique que la réunion a été correctement créée. La réponse contient également l’ID de l’élément de la réunion nouvellement créée.
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>Rechercher une réunion ou un rendez-vous en tant que délégué à l’aide de l’API managée EWS
<a name="bk_searchewsma"> </a>

Pour rechercher une réunion, vous devez utiliser l’une des méthodes [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) qui inclut un paramètre [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , afin que vous puissiez spécifier le dossier de calendrier du propriétaire de la boîte aux lettres. 
  
```cs
static void DelegateAccessSearchWithFilter
    (ExchangeService service, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Define the sort order.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Call FindItems to find matching calendar items. 
        // The FindItems parameters must denote the mailbox owner,
        // mailbox, and Calendar folder.
        // This method call results in a FindItem call to EWS.
        FindItemsResults<Item> results = service.FindItems(
        new FolderId(WellKnownFolderName.Calendar, 
            "primary@contoso.com"), 
            filter, 
            view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while 
            enumerating results: {0}", ex.Message);
    }
}
```

Une fois que l’appel **FindItems** renvoie une réponse avec un ID, vous pouvez obtenir, mettre à jour ou supprimer cette réunion en utilisant l’ID et l' [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) , et vous n’avez pas besoin de spécifier l’adresse SMTP du propriétaire de la boîte aux lettres. 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a>Rechercher une réunion ou un rendez-vous en tant que délégué à l’aide d’EWS
<a name="bk_searchews"> </a>

EWS vous permet d’utiliser l’objet de service pour l’utilisateur délégué afin de rechercher des rendez-vous et des réunions qui répondent à un ensemble de critères de recherche. Cet exemple montre comment utiliser l’opération [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour rechercher des réunions dans le dossier de calendrier du propriétaire de la boîte aux lettres qui contiennent le mot « Building » dans l’objet. 
  
Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez la méthode **FindItem** pour [Rechercher une réunion ou un rendez-vous en tant que délégué](#bk_searchewsma).
  
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
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:Restriction>
        <t:Contains ContainmentMode="Substring"
                    ContainmentComparison="IgnoreCase">
          <t:FieldURI FieldURI="item:Subject" />
          <t:Constant Value="building" />
        </t:Contains>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **FindItem** avec un message [FindItemResponse](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) qui inclut une valeur d’élément [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, ce qui indique que la recherche s’est terminée avec succès. La réponse contient un [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) pour les rendez-vous ou les réunions qui répondent aux critères de recherche. Dans ce cas, une seule réunion est trouvée. 
  
La valeur de l’élément [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) a été raccourcie pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1"
                        TotalItemsInView="1"
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="IJpUAAA="
                          ChangeKey="DwAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAAAIKhS" />
                <t:Subject>Team building exercise</t:Subject>
                <t:DateTimeReceived>2014-03-04T21:27:22Z</t:DateTimeReceived>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

À présent que l' **ID ItemId** de la réunion répond à vos critères, vous pouvez obtenir, mettre à jour ou supprimer cette réunion à l’aide de l' **ItemId** et de l' [accès implicite](delegate-access-and-ews-in-exchange.md#bk_implicit) , et vous n’avez pas besoin de spécifier l’adresse SMTP du propriétaire de la boîte aux lettres. 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a>Obtenir, mettre à jour ou supprimer des éléments de calendrier en tant que délégué à l’aide de l’API managée EWS
<a name="bk_geteswma"> </a>

Vous pouvez utiliser l’API managée EWS pour obtenir, mettre à jour ou supprimer une réunion ou un rendez-vous de la même façon que vous effectuez ces actions lorsque vous n’utilisez pas l’accès délégué. La seule différence réside dans le fait que l’objet de service est destiné à l’utilisateur délégué. L’ID d’élément inclus dans l’appel de méthode de **liaison** identifie de manière unique l’élément dans la Banque de boîtes aux lettres, dans le dossier de calendrier du propriétaire de la boîte aux lettres. 
  
**Tableau 2. Méthodes de l’API managée EWS pour l’utilisation de rendez-vous et de réunions en tant que délégué**

|**Tâche**|**Méthode d'API managée EWS**|**Exemple de code**|
|:-----|:-----|:-----|
|Obtenir un rendez-vous ou une réunion  <br/> |[Rattach](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[Obtention d’un élément à l’aide de l’API managée EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Mettre à jour un rendez-vous ou une réunion  <br/> |[Liaison](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) suivie par la [mise à jour](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[Mettre à jour une réunion à l’aide de l’API managée EWS](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|Supprimer un rendez-vous ou une réunion  <br/> |[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) suivi de [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[Supprimer une réunion à l’aide de l’API managée EWS](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a>Obtenir, mettre à jour ou supprimer des éléments de calendrier en tant que délégué à l’aide d’EWS
<a name="bk_getews"> </a>

Vous pouvez utiliser EWS pour obtenir, mettre à jour ou supprimer une réunion ou un rendez-vous de la même façon que vous effectuez ces actions lorsque vous n’utilisez pas l’accès délégué. La seule différence réside dans le fait que l’objet de service est destiné à l’utilisateur délégué. L’ID d’élément inclus dans l’appel de méthode [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) identifie de manière unique l’élément dans la Banque de boîtes aux lettres, dans le dossier de calendrier du propriétaire de la boîte aux lettres. 
  
**Tableau 3. Opérations EWS pour l’utilisation de rendez-vous et de réunions en tant que délégué**

|**Task**|**Opération EWS**|**Exemple de code**|
|:-----|:-----|:-----|
|Obtenir un rendez-vous ou une réunion  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Obtention d’un élément à l’aide d’EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Mettre à jour un rendez-vous ou une réunion  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) suivi de [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Mettre à jour une réunion à l’aide d’EWS](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|Supprimer un rendez-vous ou une réunion  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , suivi de [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Accès délégué et EWS dans Exchange](delegate-access-and-ews-in-exchange.md)   
- [Ajouter et supprimer des délégués à l’aide d’EWS dans Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [Définir les autorisations de dossier pour un autre utilisateur à l’aide d’EWS dans Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
    

