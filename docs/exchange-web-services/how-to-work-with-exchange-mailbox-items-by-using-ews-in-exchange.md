---
title: Travailler avec des éléments de boîte aux lettres Exchange à l’aide de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Découvrez comment créer, obtenir, mettre à jour et supprimer des éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.
ms.openlocfilehash: e70ac499da57faa60b4bcb6082648b23d1a7e791
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754966"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a>Travailler avec des éléments de boîte aux lettres Exchange à l’aide de EWS dans Exchange

Découvrez comment créer, obtenir, mettre à jour et supprimer des éléments à l’aide de l’API managée EWS ou d’EWS dans Exchange.
  
Vous pouvez utiliser les API managées EWS pour travailler avec des éléments dans une boîte aux lettres. Vous pouvez utiliser les éléments génériques : objets d’API managées, [élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) ou types EWS [élément](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) — pour effectuer certaines opérations (obtention d’un élément ou suppression d’un élément à l’aide identificateur de l’élément) ; Toutefois, la plupart du temps, que vous devrez utiliser [fortement typées élément](folders-and-items-in-ews-in-exchange.md#bk_item) pour effectuer une opération get ou mettre à jour opération car vous aurez besoin d’accéder aux propriétés qui sont spécifiques à l’élément fortement typé. 

Par exemple, vous ne pouvez pas utiliser un élément générique pour récupérer un élément qui contient un début et date de fin, vous avez besoin d’un objet d’API managées [rendez-vous](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) ou un type EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) à le faire. Et si vous utilisez l’API managée EWS, vous devrez toujours créer des éléments fortement typées, car la classe de **l’élément** générique ne dispose pas d’un constructeur. Si vous travaillez avec un élément qui n’est pas fortement typé, vous pouvez toujours utiliser la classe de **l’élément de** base pour travailler avec l’élément. 
  
**Le tableau 1. Méthodes d’API managées et opérations EWS pour l’utilisation d’éléments**

|**Pour...**|**Méthode d'API managée EWS**|**Opération EWS**|
|:-----|:-----|:-----|
|Créer un élément générique  <br/> |Aucune. Vous pouvez uniquement créer des types d’élément spécifiques à l’aide de l’API managée EWS. Vous ne pouvez pas créer d’éléments génériques.  <br/> |[CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|Obtenir un élément  <br/> |[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|Mettre à jour un élément  <br/> |[Item.Update](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Supprimer un élément  <br/> |[Item.Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
Dans cet article, vous apprendrez quand vous pouvez utiliser la classe de base générique et lorsque vous devez utiliser un élément fortement typé pour effectuer votre tâche. Les exemples de code montrent comment utiliser la classe de base et que faire lorsque vous ne pouvez pas utiliser la classe de base ou qu’il ne selon vos besoins.
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a>Création d’un élément à l’aide de l’API managée EWS
<a name="bk_createewsma"> </a>

L’API managée EWS ne dispose pas d’un constructeur publiquement disponible pour la classe [d’élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , vous devez utiliser le constructeur pour le type d’élément spécifique que vous souhaitez créer afin de créer un élément. Par exemple, utilisez le [constructeur de classe EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) pour créer un nouveau message électronique et [contactez le constructeur de classe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) pour créer un nouveau contact. De même, le serveur ne retourne jamais les objets **élément** génériques dans les réponses ; tous les éléments génériques sont renvoyés en tant qu’objets **EmailMessage** . 
  
Lorsque vous connaissez le type d’élément à créer, vous pouvez effectuer la tâche en quelques étapes seulement. Les étapes sont similaires pour tous les types d’éléments :
  
1. Initialiser une nouvelle instance d’une des classes [d’élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) avec l’objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) en tant que paramètre. 
    
2. Définissez des propriétés sur l’élément. Les schémas sont différents pour chaque type d’élément, c’est pourquoi plusieurs propriétés sont disponibles pour ces derniers.
    
3. Enregistrez l’élément, ou enregistrez et envoyez l’élément.
    
Par exemple, vous créez un objet [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) , définir des propriétés [ToRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) , le [corps](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx)et [l’objet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx)et l’envoyer puis en utilisant la méthode [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) . 
  
```cs
// Create an email message and provide it with connection 
// configuration information by using an ExchangeService object named service.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.Subject = "Company Soccer Team";
message.Body = "Are you interested in joining?";
message.ToRecipients.Add("sadie@contoso.com");
// Send the email message and save a copy.
// This method call results in a CreateItem call to EWS.
message.SendAndSaveCopy();
```

Pour savoir comment créer une réunion ou un élément de rendez-vous à l’aide de l’API managée EWS, voir [créer des rendez-vous et réunions à l’aide EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).
  
## <a name="create-an-item-by-using-ews"></a>Création d’un élément à l’aide d’EWS
<a name="bk_createews"> </a>

Vous pouvez créer un élément générique ou un élément fortement typé à l’aide d’EWS. Les étapes sont similaires pour tous les types d’éléments :
  
1. Utilisez l’opération [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) pour créer un élément dans la banque d’informations Exchange. 
    
2. Utilisez l’élément [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) pour contenir un ou plusieurs éléments à créer. 
    
3. Définissez des propriétés sur l’élément.
    
Par exemple, vous pouvez créer un message électronique et l’envoyer en utilisant le code dans l’exemple suivant. C’est également la demande XML qui envoie de l’API managée EWS lorsque vous appelez la méthode [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) . 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com </t:EmailAddress>
              </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **CreateItem** avec un message [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) qui contient une valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que le courrier électronique a été créé avec succès et l' [ID d’élément](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de la nouvelle message créé. 
  
Pour savoir comment créer une réunion ou un élément de rendez-vous à l’aide de EWS, voir [créer des rendez-vous et réunions à l’aide EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a>Obtention d’un élément à l’aide de l’API managée EWS
<a name="bk_getewsma"> </a>

Pour utiliser l’API managée EWS pour obtenir un élément si vous connaissez [Item.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à récupérer, vous appelez simplement une des méthodes [liaison](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) sur l’élément, et l’élément est récupéré. Meilleure pratique, nous vous recommandons de limiter les propriétés renvoyées uniquement à ceux qui sont requis. Cet exemple renvoie la propriété **Id** d’élément et la propriété **Subject** . 
  
Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange. variable local *itemId* est l' [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à mettre à jour. 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

Si vous recherchez un élément qui répond aux critères spécifiques, procédez comme suit :
  
1. Établissez une liaison vers le dossier qui contient les éléments à obtenir.
    
2. Instanciez un [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) ou un [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) pour filtrer les éléments à renvoyer. 
    
3. Instancier un objet [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) ou de [l’annonceAfficher le](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) pour spécifier le nombre d’éléments à renvoyer. 
    
4. Appelez la méthode [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) . 
    
Par exemple, si vous souhaitez récupérer des messages électroniques non lus dans la boîte de réception, utilisez le code dans l’exemple suivant. Cet exemple utilise un **SearchFilterCollection** pour limiter les résultats de la méthode **FindItems** aux messages non lus et limite **l’annonceAfficher le** pour limiter les résultats à un élément. Ce code fonctionne uniquement sur les objets [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) car la valeur [EmailMessageSchema.IsRead](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) fait partie de la **SearchFilter**. 
  
```cs
// Bind the Inbox folder to the service object.
Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
// The search filter to get unread email.
SearchFilter sf = new SearchFilter.SearchFilterCollection(LogicalOperator.And, new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false));
ItemView view = new ItemView(1);
// Fire the query for the unread items.
// This method call results in a FindItem call to EWS.
FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Inbox, sf, view);
```

Sinon, vous pouvez utiliser un [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) pour limiter les résultats de la recherche, comme illustré dans l’exemple de code suivant. Cet exemple utilise la méthode [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) pour récupérer jusqu'à cinq rendez-vous qui se produisent dans les 30 jours. Ce code bien sûr fonctionne uniquement sur les éléments de calendrier. 
  
```cs
// Initialize values for the start and end times, and the number of appointments to retrieve.
DateTime startDate = DateTime.Now;
DateTime endDate = startDate.AddDays(30);
const int NUM_APPTS = 5;
// Bind the Calendar folder to the service object.
// This method call results in a GetFolder call to EWS.
CalendarFolder calendar = CalendarFolder.Bind(service, WellKnownFolderName.Calendar, new PropertySet());
// Set the start and end time and number of appointments to retrieve.
CalendarView cView = new CalendarView(startDate, endDate, NUM_APPTS);
// Limit the properties returned to the appointment's subject, start time, and end time.
cView.PropertySet = new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End);
// Retrieve a collection of appointments by using the calendar view.
// This method call results in a FindAppointments call to EWS.
FindItemsResults<Appointment> appointments = calendar.FindAppointments(cView);
```

Notez que cette propriété renvoie les informations du serveur dans la réponse de la méthode **lier** est différente de celle que le serveur renvoie une réponse de méthode **FindItem** ou **FindAppointment** les informations. La méthode **Bind** peut renvoyer toutes les propriétés schématisées, tandis que les méthodes **FindItem** et **FindAppointment** ne renvoient pas toutes les propriétés schématisées. Si vous avez besoin d’un accès complet à l’élément, vous devez donc d’utiliser la méthode de **liaison** . Si vous n’avez pas l’élément **Id** de l’élément vous souhaitez récupérer, utiliser les méthodes **FindItem** ou **FindAppointment** pour récupérer l’Id, puis utilisez la méthode **Bind** pour récupérer les propriétés dont vous avez besoin. 
  
Pour savoir comment obtenir une réunion ou un élément de rendez-vous à l’aide de l’API managée EWS, voir [obtenir des rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="get-an-item-by-using-ews"></a>Obtention d’un élément à l’aide d’EWS
<a name="bk_getews"> </a>

Si vous connaissez l' [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) de l’élément à récupérer, vous pouvez obtenir l’élément à l’aide de l’opération [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) . 
  
L’exemple suivant montre la demande XML pour obtenir l' [objet](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) d’un élément avec un **ID d’élément**spécifique. C’est également la demande XML qui envoie de l’API managée EWS lors de l’appel de la méthode [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) sur un **ID d’élément**. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="GJc/NAAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

L’exemple suivant montre la réponse XML que le serveur renvoie une fois qu’il traite l’opération **GetItem** . La réponse indique que l’élément a été récupéré correctement. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="GJc/NAAA=" ChangeKey="CQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAGJd9Z"/>
              <t:Subject>Company Soccer Team</t:Subject>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

Si vous ne connaissez pas l' **ID d’élément** de l’élément que vous souhaitez récupérer, vous pouvez utiliser l’opération [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) pour rechercher l’élément. Pour pouvoir utiliser l’opération **FindItem** , vous devez d’abord identifier le dossier dans lequel vous effectuez une recherche. Vous pouvez identifier le dossier à l’aide de son **DistinguinguishedFolderName** ou à l’aide de l' [ID FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx). Vous pouvez utiliser les opérations [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) ou de [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) pour obtenir l' **ID FolderId** dont vous avez besoin. Ensuite, utilisez l’opération **FindItem** pour rechercher ce dossier pour les résultats qui correspondent au filtre de recherche. Contrairement à l’API managée EWS, EWS ne fournit pas une opération de recherche distincte pour les rendez-vous. L’opération **FindItem** récupère les éléments de tous les types. 
  
L’exemple suivant montre la requête d’opération XML **FindItem** qui est envoyée au serveur pour rechercher les rendez-vous dans le dossier de calendrier qui se produisent dans les 30 jours. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité. 
  
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
      <m:CalendarView MaxEntriesReturned="5" StartDate="2013-10-16T17:04:28.722Z" EndDate="2013-11-15T18:04:28.722Z" />
      <m:ParentFolderIds>
        <t:FolderId Id="AAAEOAAA=" ChangeKey="AgAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAAAA3" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **FindItem** avec un message [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) qui inclut la valeur de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, qui indique que l’opération s’est terminée correctement. Si les éléments de calendrier répondent aux critères de filtrage, ils sont inclus dans la réponse.
  
Notez que cette propriété renvoie les informations du serveur dans la réponse d’opération **GetItem** est différent de celui les informations sur que le serveur renvoie dans un **FindItem** ou une réponse d’opération **FindAppointment** . L’opération **GetItem** peut renvoyer toutes les propriétés schématisées, tandis que les opérations **FindItem** et **FindAppointment** ne renvoient pas toutes les propriétés schématisées. Si vous avez besoin d’un accès complet à l’élément, vous devez donc utiliser l’opération **GetItem** . Si vous n’avez pas l' **ID d’élément** de l’élément vous souhaitez récupérer, les opérations **FindItem** ou **FindAppointment** permet de récupérer l' **ID d’élément**et utiliser l’opération **GetItem** pour récupérer les éléments dont vous avez besoin. 
  
Pour savoir comment obtenir une réunion ou un élément de rendez-vous à l’aide de EWS, voir [obtenir des rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a>Mise à jour d’un élément à l’aide de l’API managée EWS
<a name="bk_updateewsma"> </a>

Les étapes pour mettre à jour un élément à l’aide de l’API managée EWS sont similaires pour tous les types d’éléments ; Toutefois, les propriétés d’élément sont différentes pour chaque type d’élément et la méthode de [mise à jour](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) possède de nombreuses méthodes surchargées à sélectionner. Pour mettre à jour un élément : 
  
1. Utilisez la méthode [lier](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) pour obtenir la dernière version de l’élément, sauf si vous disposez déjà d’elle. Pour mettre à jour les propriétés spécifiques à un élément fortement typé, vous devrez lier à ce type d’élément. Pour mettre à jour les propriétés disponibles sur le type d’élément générique, vous pouvez lier à l’objet [d’élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) . 
    
2. Mettez à jour les propriétés sur l’élément.
    
3. Appelez la méthode de **mise à jour** . 
    
Par exemple, vous pouvez mettre à jour l’objet d’un message électronique à l’aide du type d’élément générique, comme illustré dans le code de l’exemple suivant.
  
Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange. variable local *itemId* est l' [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à mettre à jour. 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Update the Subject of the email.
item.Subject = "New subject";
// Save the updated email.
// This method call results in an UpdateItem call to EWS.
item.Update(ConflictResolutionMode.AlwaysOverwrite);
```

Pour savoir comment mettre à jour une réunion ou un élément de rendez-vous à l’aide de l’API managée EWS, voir [mettre à jour vos rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="update-an-item-by-using-ews"></a>Mise à jour d’un élément à l’aide d’EWS
<a name="bk_updateews"> </a>

Pour mettre à jour un élément à l’aide d’EWS, procédez comme suit :
  
1. Utiliser l’opération de [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) pour obtenir la dernière version de l’élément, sauf si vous disposez déjà d’elle. 
    
2. L’opération [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) permet de spécifier les champs pour mettre à jour et attribuer de nouvelles valeurs à ces champs. 
    
L’exemple suivant montre la requête d’opération XML **UpdateItem** qui est envoyée au serveur pour mettre à jour la valeur de [l’objet](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) du message électronique. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAPdgr" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>New subject</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **UpdateItem** avec un message [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) qui inclut la valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que la mise à jour de l’élément a réussi.
  
Pour savoir comment mettre à jour une réunion ou un élément de rendez-vous à l’aide de EWS, voir [mettre à jour vos rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a>Suppression d’un élément à l’aide de l’API managée EWS
<a name="bk_deleteewsma"> </a>

Vous pouvez supprimer des éléments en les déplaçant vers le dossier éléments supprimés ou à la benne. Si vous connaissez l' [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à supprimer, vous devez seulement appeler la méthode [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) sur l’élément. 
  
Si vous devez rechercher l’élément avant de le supprimer, procédez comme suit :
  
1. Appelez la méthode [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) pour trouver l’élément à supprimer. 
    
1. Instancier un [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) et limitez aux propriétés à retourner ou utiliser un [SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) pour rechercher des éléments spécifiques. 
    
2. Instanciez un [annonceAfficher](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) l’ou [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) pour spécifier le nombre d’éléments à renvoyer. 
    
2. Appelez la méthode [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) . 
    
Par exemple, le code suivant indique comment déplacer un message électronique vers le dossier Éléments supprimés.
  
Cet exemple suppose que ce **service** est un objet [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) valide et que l’utilisateur a été authentifié sur un serveur Exchange. variable local *itemId* est l' [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) de l’élément à mettre à jour. 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

Pour plus d’informations sur la suppression d’éléments, voir [suppression d’éléments à l’aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md). Pour savoir comment supprimer une réunion ou un élément de rendez-vous à l’aide de l’API managée EWS, voir [Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).
  
## <a name="delete-an-item-by-using-ews"></a>Suppression d’un élément à l’aide d’EWS
<a name="bk_deleteews"> </a>

Vous pouvez supprimer un élément à l’aide de l’opération [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) . 
  
L’exemple suivant présente la demande XML qui est envoyée au serveur pour déplacer le message vers le dossier Éléments supprimés. Les valeurs de certains attributs et éléments ont été raccourcies pour des raisons de lisibilité.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems">
      <m:ItemIds>
        <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAANIFzC" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

Le serveur répond à la demande **DeleteItem** avec un message [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) qui inclut la valeur [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, ce qui indique que la suppression de l’élément a réussi.
  
Pour plus d’informations sur la suppression d’éléments, voir [suppression d’éléments à l’aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md). Pour savoir comment supprimer une réunion ou un élément de rendez-vous à l’aide de EWS, voir [Supprimer des rendez-vous et annuler des réunions à l’aide de EWS dans Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).
  
## <a name="move-or-copy-items-to-another-mailbox"></a>Déplacement ou copie d’éléments vers une autre boîte aux lettres
<a name="bk_movecopybtnmailboxes"> </a>

Vous pouvez déplacer ou copier des éléments entre les boîtes aux lettres en utilisant les opérations [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) et [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) . Pour plus d’informations, voir [exportation et importation d’éléments à l’aide de EWS dans Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Voir aussi

- [Dossiers et éléments dans EWS dans Exchange](folders-and-items-in-ews-in-exchange.md)    
- [Utilisation de dossiers à l’aide de EWS dans Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [Suppression d’éléments à l’aide de EWS dans Exchange](deleting-items-by-using-ews-in-exchange.md)
    

