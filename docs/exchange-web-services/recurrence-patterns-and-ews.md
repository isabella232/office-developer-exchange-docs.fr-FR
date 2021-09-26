---
title: Périodicités et EWS
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Découvrez les modèles de récurrence et les séries périodiques dans Exchange.
ms.openlocfilehash: fcd6cf847efedd3bc48a26ad7866a0221de59371
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541587"
---
# <a name="recurrence-patterns-and-ews"></a>Périodicités et EWS

Découvrez les modèles de récurrence et les séries périodiques dans Exchange.
  
Une série périodique est un rendez-vous ou une réunion qui se répète selon un modèle défini. Une série périodique peut avoir un nombre spécifique d’occurrences ou se répéter indéfiniment. En outre, une série périodique peut avoir des exceptions qui ne suivent pas le modèle du reste des occurrences et peut avoir des occurrences qui ont été supprimées du modèle. Vous pouvez utiliser l’API gérée EWS et EWS pour travailler avec des séries périodiques et leurs éléments de calendrier associés.
  
## <a name="recurring-calendar-items"></a>Éléments de calendrier périodiques

Tous les éléments de calendrier se classent dans l’une des quatre catégories suivantes :
  
- Éléments de calendrier non périodiques
    
- Récurrons les maîtres
    
- Occurrences d’une série
    
- Occurrences modifiées dans une série, appelées exceptions
    
Dans cet article, nous allons examiner les trois types d’éléments de calendrier qui font partie d’une série périodique.
  
Il est utile de comprendre comment les séries périodiques sont implémentées sur Exchange serveur. Au lieu de créer un élément distinct distinct pour chaque occurrence d’une série périodique, le serveur crée un seul élément réel dans le calendrier, appelé maître périodique. Le format d’une forme de maître périodique est très similaire à un rendez-vous non périodique, avec l’ajout d’informations de modèle de récurrence. Le serveur génère ensuite des occurrences basées sur la fréquence de récurrence en réponse aux demandes des clients d’informations de rendez-vous, à l’aide d’un processus appelé expansion. Ces occurrences générées ne sont pas stockées définitivement sur le serveur. Il est important de comprendre cela, car la façon dont vous recherchez des éléments de calendrier détermine les informations que vous recevez et si l’expansion se produit.
  
## <a name="recurrence-patterns"></a>Périodicités

L’élément clé d’une série périodique qui rend l’expansion possible est la récurrence. La récurrence se trouve sur la forme de base périodique et décrit un ensemble de critères pour le calcul des occurrences en fonction de la date et de l’heure de la forme de base périodique.
  
**Tableau 1. Modèles de récurrence disponibles**

|**Classe API gérée EWS**|**Élément EWS**|**Exemples**|
|:-----|:-----|:-----|
|[Recurrence.DailyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[DailyRecurrence](https://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |Répétez l’étape tous les jours.  <br/> Répétez l’étape tous les deux jours.  <br/> |
|[Recurrence.MonthlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteMonthlyRecurrence](https://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |Répéter tous les mois le dixième jour du mois.  <br/> Répétez l’étape tous les deux mois le 21 du mois.  <br/> |
|[Recurrence.RelativeMonthlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeMonthlyRecurrence](https://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |Répétez l’étape le deuxième mardi de chaque mois.  <br/> Répétez l’étape le troisième jeudi du mois tous les trois mois.  <br/> |
|[Recurrence.RelativeYearlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeYearlyRecurrence](https://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |Répétez l’étape le premier lundi d’août chaque année.  <br/> |
|[Recurrence.WeeklyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[WeeklyRecurrence](https://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |Répétez l’étape tous les lundis.  <br/> Répéter tous les mardis et jeudis toutes les deux semaines.  <br/> |
|[Recurrence.YearlyPattern](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteYearlyRecurrence](https://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |Répétez l’étape le 1er septembre chaque année.  <br/> |
   
L’autre information importante pour une récurrence est la fin de la récurrence. Cela peut être exprimé sous la mesure d’un nombre d’occurrences donné, d’une date de fin ou d’une absence de fin.
  
**Tableau 2. Options de fin d’une série périodique**

|**Méthode/propriété de l’API gérée EWS**|**Élément EWS**|**Description**|
|:-----|:-----|:-----|
|[Recurrence.NumberOfOccurrences](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[NumberedRecurrence](https://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |La valeur de cette propriété ou élément spécifie le nombre d’occurrences.  <br/> |
|[Recurrence.EndDate](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[EndDateRecurrence](https://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |La dernière occurrence de la série se produit à la date spécifiée par cette propriété ou cet élément ou avant celle-ci.  <br/> |
|[Recurrence.HasEnd](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [Recurrence.NeverEnds](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[NoEndRecurrence](https://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |La série n’a pas de fin.  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a>Vues étendues et non étendues

L’utilisation de la méthode **FindAppointments** dans l’API gérée EWS (ou l’opération **FindItem** avec un élément **CalendarView** dans EWS) appelle le processus d’expansion. Cela masque les rendez-vous maîtres périodiques du jeu de résultats et présente à la place une vue étendue de cette série périodique. Les occurrences et les exceptions à la maître périodique qui se trouve dans les paramètres de l’affichage Calendrier sont incluses dans le jeu de résultats. À l’inverse, l’utilisation de la méthode **FindItems** dans l’API gérée EWS (ou l’opération **FindItem** avec un **élément IndexedPageItemView** ou **FractionalPageItemView** dans EWS) n’appelle pas le processus d’expansion et les occurrences et les exceptions ne sont pas incluses. Examinons un exemple comparant les deux méthodes. 
  
**Tableau 3. Méthodes et opérations pour la recherche de rendez-vous**

|**Méthode d'API managée EWS**|**Opération EWS**|**Développe une série ?**|**Éléments inclus dans les résultats**|
|:-----|:-----|:-----|:-----|
|[ExchangeService.FindAppointments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |[Opération FindItem avec](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) un [élément CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)  <br/> |Oui  <br/> |Rendez-vous non périodiques, occurrences individuelles de séries périodiques et exceptions aux séries périodiques  <br/> |
|[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[Opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) avec un [élément IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou [FractionalPageItemView](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)  <br/> |Non  <br/> |Rendez-vous non périodiques et rendez-vous maîtres périodiques  <br/> |
   
Sadie vient d’signer son fils pour l’équipe de formation. L’équipe s’entraîne tous les mercredis matin à 8 h 30, à partir du 2 juillet, la dernière pratique étant le 6 août. Ne souhaitant pas oublier la pratique, Sadie ajoute un rendez-vous périodique à son calendrier pour lui le rappeler.
  
**Tableau 4. Rendez-vous périodique de Sadie**

|**Champ Rendez-vous**|**Valeur**|
|:-----|:-----|
|Sujet  <br/> |Pratique de l’équipe de formation  <br/> |
|Début  <br/> |2 juillet 2014 08:30  <br/> |
|End  <br/> |2 juillet 2014 10:00  <br/> |
|Récurseurs  <br/> |Tous les mercredis  <br/> |
|Dernière occurrence  <br/> |6 août 2014 8:30  <br/> |
   
Un aperçu rapide d’un calendrier montre que l’équipe aura un total de six pratiques. Toutefois, il n’y a pas six éléments de rendez-vous distincts dans le calendrier. Au lieu de cela, il n’existe qu’un seul rendez-vous maître périodique représentant la série.
  
Examinons maintenant la recherche de rendez-vous dans le calendrier de Sadie qui se produisent au cours du mois de juillet. L’exemple de code suivant utilise la méthode **FindItems** dans l’API Exchange Managed pour produire une vue non étendue du calendrier de Sadie. 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
#region FindItems + ItemView method
ItemView itemView = new ItemView(100);
itemView.PropertySet = propSet;
List<SearchFilter> filterList = new List<SearchFilter>();
// Find appointments that start after midnight on July 1, 2014.
SearchFilter.IsGreaterThan startFilter = new SearchFilter.IsGreaterThan(AppointmentSchema.Start,
    new DateTime(2014, 7, 1));
// Find appointments that end before midnight on July 31, 2014
SearchFilter.IsLessThan endFilter = new SearchFilter.IsLessThan(AppointmentSchema.End,
    new DateTime(2014, 7, 31));
filterList.Add(startFilter);
filterList.Add(endFilter);
SearchFilter.SearchFilterCollection calendarFilter = new SearchFilter.SearchFilterCollection(LogicalOperator.And, filterList);
// This results in a call to EWS.
FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Calendar, calendarFilter, itemView);
foreach(Item appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

Ce code entraîne la demande [d’opération FindItem suivante](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) avec un [élément IndexedPageItemView.](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="100" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:IsGreaterThan>
            <t:FieldURI FieldURI="calendar:Start" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-01T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsGreaterThan>
          <t:IsLessThan>
            <t:FieldURI FieldURI="calendar:End" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-31T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsLessThan>
        </t:And>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

La réponse du serveur inclut un seul élément, le maître périodique, indiqué par la valeur de l’élément [CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) **de RecurringMaster**. La valeur de [l’élément ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) a été raccourcie pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
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
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

Maintenant, nous allons comparer avec une vue étendue. L’exemple de code suivant utilise **la méthode FindAppointments** dans l’API gérée EWS pour créer une vue étendue du calendrier de Sadie. 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
CalendarView calView = new CalendarView(new DateTime(2014, 7, 1),
    new DateTime(2014, 7, 31));
calView.PropertySet = propSet;
FindItemsResults<Appointment> results = service.FindAppointments(WellKnownFolderName.Calendar, calView);
foreach(Appointment appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

Ce code entraîne la demande [d’opération FindItem suivante](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) avec un [élément CalendarView.](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView StartDate="2014-07-01T07:00:00.000Z" EndDate="2014-07-31T07:00:00.000Z" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Cette fois, la réponse du serveur inclut cinq occurrences, une pour chaque mercredi de juillet. Les [éléments CalendarItemType](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) de ces éléments ont tous la valeur **Occurrence**. Notez que la forme de maître périodique n’est pas présente dans la réponse. Les valeurs des éléments [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) ont été raccourcies pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
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
          <m:RootFolder TotalItemsInView="5" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-09T15:30:00Z</t:Start>
                <t:End>2014-07-09T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA8..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-16T15:30:00Z</t:Start>
                <t:End>2014-07-16T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA9..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-23T15:30:00Z</t:Start>
                <t:End>2014-07-23T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADAA..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-30T15:30:00Z</t:Start>
                <t:End>2014-07-30T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

Une fois que vous avez une forme de maître périodique, une occurrence ou une exception, vous pouvez toujours récupérer [les autres éléments associés.](how-to-access-a-recurring-series-by-using-ews-in-exchange.md) En cas d’occurrence ou d’exception, vous pouvez récupérer la maître périodique, et vice versa.
  
## <a name="working-with-recurring-calendar-items"></a>Travailler avec des éléments de calendrier périodiques

Vous utilisez les mêmes méthodes et opérations pour travailler avec des séries périodiques que pour travailler avec des éléments de calendrier non périodiques. La différence est que, en fonction de l’élément que vous utilisez pour appeler ces méthodes ou opérations, les actions que vous prenez peuvent s’appliquer à l’ensemble de la série ou à une seule occurrence. [Les actions entreprises sur le](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) maître périodique s’appliquent à toutes les occurrences de la série, tandis que les actions entreprises sur une occurrence ou une [exception](how-to-update-a-recurring-series-by-using-ews.md) ne s’appliquent qu’à cette occurrence ou exception. 
  
## <a name="in-this-section"></a>Dans cette section

- [Accéder à une série périodique à l’aide d’EWS dans Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Créer une série périodique à l’aide d’EWS dans Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Supprimer des rendez-vous dans une série périodique à l’aide d’EWS Exchange](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Mettre à jour une série périodique à l’aide d’EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Mettre à jour une série périodique à l’aide d’EWS Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
    
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

