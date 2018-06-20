---
title: Périodicités et EWS
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Découvrez les périodicités et série périodique dans Exchange.
ms.openlocfilehash: ac10e9b9a347abb5907b77f0e0e7315e4e86d97a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755070"
---
# <a name="recurrence-patterns-and-ews"></a>Périodicités et EWS

Découvrez les périodicités et série périodique dans Exchange.
  
Une série périodique est un rendez-vous ou réunion qui se répète selon un modèle défini. Une série périodique peut avoir un certain nombre d’occurrences ou pouvez répéter indéfiniment. En outre, une série périodique peut avoir les exceptions qui ne suivent pas le modèle du reste des occurrences et peuvent avoir des occurrences qui ont été supprimées du modèle. Vous pouvez utiliser les API managées EWS pour fonctionner avec une série périodique et leurs éléments de calendrier associé.
  
## <a name="recurring-calendar-items"></a>Rendez-vous périodiques

Tous les éléments de calendrier peuvent être classées dans un des quatre catégories suivantes :
  
- Éléments de calendrier non périodiques
    
- Masters périodiques
    
- Occurrences d’une série
    
- Occurrences modifiés d’une série, appelées exceptions
    
Dans cet article, nous examinerons les trois types d’éléments de calendrier qui font partie d’une série périodique.
  
Il est utile de comprendre comment périodique série sont implémentés sur le serveur Exchange. Au lieu de créer un élément distinct distinct pour chaque occurrence d’une série périodique, le serveur crée un seul élément réel dans le calendrier, appelé le contrôleur périodique. Le format d’une forme de base périodique est très similaire à un rendez-vous non périodique, avec l’ajout d’informations de modèle de périodicité. Le serveur génère puis occurrences en fonction de la périodicité en réponse aux demandes des clients pour des informations de rendez-vous, à l’aide d’un processus de développement. Ces occurrences générés ne sont pas stockés définitivement sur le serveur. Il est important de comprendre la façon dont vous recherchez des éléments de calendrier détermine quelles informations vous recevez et si le développement de cet événement se produit.
  
## <a name="recurrence-patterns"></a>Périodicités

L’information à une série périodique qui permet le développement de clé est la périodicité. La périodicité se trouve sur le contrôleur de périodique et décrit un ensemble de critères pour le calcul des occurrences en fonction de la date et l’heure de la forme de base périodique.
  
**Le tableau 1. Périodicités disponibles**

|**Classe de l’API managée EWS**|**Élément EWS**|**Exemples**|
|:-----|:-----|:-----|
|[Recurrence.DailyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[DailyRecurrence](http://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |Répéter tous les jours.  <br/> Répétez tous les jours.  <br/> |
|[Recurrence.MonthlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteMonthlyRecurrence](http://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |Répéter tous les mois le dixième jour du mois.  <br/> Répéter chaque mois sur le vingt-et-unième jour du mois.  <br/> |
|[Recurrence.RelativeMonthlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeMonthlyRecurrence](http://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |Répétez le deuxième mardi du mois.  <br/> Répétez le troisième jeudi du mois tous les trois mois.  <br/> |
|[Recurrence.RelativeYearlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeYearlyRecurrence](http://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |Répétez le premier lundi du mois d’août de chaque année.  <br/> |
|[Recurrence.WeeklyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[WeeklyRecurrence](http://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |Répétez tous les lundis.  <br/> Répétez toutes les semaines de chaque mardi et le jeudi.  <br/> |
|[Recurrence.YearlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteYearlyRecurrence](http://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |Répéter tous les ans le 1er septembre.  <br/> |
   
L’autres importante information d’une périodicité est à la fin de la périodicité. Ceci peut être exprimé sous la forme d’un nombre défini d’occurrences, comme une date de fin ou comme n’ayant aucun fin.
  
**Le tableau 2. Options pour la fin d’une série périodique**

|**Propriété de la méthode API managées**|**Élément EWS**|**Description**|
|:-----|:-----|:-----|
|[Recurrence.NumberOfOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[NumberedRecurrence](http://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |La valeur de cette propriété ou d’un élément spécifie le nombre d’occurrences.  <br/> |
|[Recurrence.EndDate](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[EndDateRecurrence](http://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |Correspond à la dernière occurrence de la série ou avant la date spécifiée par cette propriété ou d’un élément.  <br/> |
|[Recurrence.HasEnd](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [Recurrence.NeverEnds](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[NoEndRecurrence](http://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |La série ne possède aucun fin.  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a>Développé et non développé des affichages

À l’aide de la méthode **FindAppointments** dans l’API managée EWS (ou l’opération **FindItem** avec un élément **CalendarView** dans EWS) appelle le processus de développement. Cela masque les rendez-vous périodiques du jeu de résultats et présente une vue développée de cette série périodique. Occurrences d’et les exceptions à la forme de base périodique qui tombent dans les paramètres de l’affichage calendrier sont incluses dans le jeu de résultats. À l’inverse, à l’aide de la méthode **FindItems** dans l’API managée EWS (ou l’opération **FindItem** avec un élément **IndexedPageItemView** ou **FractionalPageItemView** dans EWS), n’appelle pas le processus de développement et occurrences et exceptions ne sont pas incluses. Examinons un exemple de comparaison des deux méthodes. 
  
**Le tableau 3. Méthodes et des opérations pour la recherche de rendez-vous**

|**Méthode d'API managée EWS**|**Opération EWS**|**Développe la série ?**|**Éléments inclus dans les résultats**|
|:-----|:-----|:-----|:-----|
|[ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |[Opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) avec un élément [CalendarView](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)  <br/> |Oui  <br/> |Rendez-vous non périodiques, occurrences d’une série périodique et les exceptions à la série périodique  <br/> |
|[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[Opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) avec un élément [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou un élément [FractionalPageItemView](http://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)  <br/> |Non  <br/> |Rendez-vous non périodiques et les rendez-vous périodiques  <br/> |
   
Sadie son fils pour l’équipe comprend vient de se connecter. L’équipe a pratique mercredi matin à 8 h 30, commençant à 2 juillet, la dernière étant pratique 6 août. Souhaitent ne pas oublier pratique, Sadie ajoute un rendez-vous périodique à son calendrier pour lui rappeler.
  
**Le tableau 4. Rendez-vous périodique de Sadie**

|**Champ de rendez-vous**|**Valeur**|
|:-----|:-----|
|Objet  <br/> |Nager pratique d’équipe  <br/> |
|Démarrer  <br/> |2 juillet 2014 8 h 30  <br/> |
|End  <br/> |2 juillet 2014 10:00:00  <br/> |
|Une nouvelle occurrence du  <br/> |Tous les mercredis  <br/> |
|Dernière occurrence  <br/> |6 août 2014 8 h 30  <br/> |
   
Un aperçu rapide un calendrier indique que l’équipe aura un total de six pratiques. Toutefois, il ne sont pas six éléments de rendez-vous distincts dans le calendrier. Au lieu de cela, il est un rendez-vous principal représentant la série.
  
Maintenant examinons le rendez-vous de calendrier de Sadie qui se produisent au cours du mois de juillet. L’exemple de code suivant utilise la méthode **FindItems** dans l’API managée Exchange pour générer un affichage de calendrier de Sadie non développé. 
  
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

Ce code génère la demande [d’opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) suivante avec un élément [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

La réponse du serveur inclut un seul élément, la forme de base périodique, indiquée par la valeur d’élément [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) de **RecurringMaster**. La valeur de l’élément [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) a été raccourcie pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
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

Maintenant nous allons comparer avec un affichage développé. L’exemple de code suivant utilise la méthode **FindAppointments** dans l’API managée EWS pour créer un affichage de calendrier de Sadie développé. 
  
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

Ce code entraîne la demande [d’opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) suivante avec un élément [CalendarView](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Cette fois-ci, la réponse du serveur comprend cinq occurrences, un pour chaque mercredi en juillet. Ces éléments de tous les éléments [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) ont la valeur **d’Occurrence**. Notez que le contrôleur périodique n’est pas présent dans la réponse. Les valeurs des éléments [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) ont été raccourcies pour des raisons de lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
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

Une fois que vous avez une forme de base périodique, une occurrence ou une exception, vous pouvez toujours [récupérer les autres éléments connexes](how-to-access-a-recurring-series-by-using-ews-in-exchange.md). Étant donné une occurrence ou une exception, vous pouvez récupérer la forme de base périodique et vice versa.
  
## <a name="working-with-recurring-calendar-items"></a>Utilisation d’éléments de calendrier périodique

Vous utilisez les mêmes opérations et des méthodes pour travailler avec une série périodique que vous utilisez pour travailler avec des éléments de calendrier non périodiques. La différence est que, selon l’élément que vous utilisez pour appeler les méthodes ou les opérations, les actions applicables à la série entière ou seulement une seule occurrence. [Actions effectuées sur le contrôleur de périodique](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) s’appliquent à toutes les occurrences de la série, alors que les [actions effectuées sur une seule occurrence ou une exception](how-to-update-a-recurring-series-by-using-ews.md) s’applique uniquement à cette occurrence ou une exception. 
  
## <a name="in-this-section"></a>Dans cette section

- [Accéder à une série périodique à l’aide de EWS dans Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Créer une série périodique à l’aide de EWS dans Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Supprimer un rendez-vous périodique à l’aide de EWS dans Exchange](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Mise à jour d’une série périodique à l’aide de EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Mise à jour d’une série périodique à l’aide de EWS dans Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Calendriers et EWS dans Exchange](calendars-and-ews-in-exchange.md)
    
- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Obtenir des rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

