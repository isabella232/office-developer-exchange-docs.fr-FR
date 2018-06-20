---
title: Fuseaux horaires et les services EWS d’Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0e0a666c-0541-414b-a7fb-297d94f692e6
description: Découvrez comment les fuseaux horaires fonctionnent avec les API managées EWS dans Exchange.
ms.openlocfilehash: fcc8b00acf2b63de04718e13b82191de95bbf2b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755079"
---
# <a name="time-zones-and-ews-in-exchange"></a>Fuseaux horaires et les services EWS d’Exchange

Découvrez comment les fuseaux horaires fonctionnent avec les API managées EWS dans Exchange.
  
Fuseaux horaires ne sont pas quelque chose que la plupart des personnes donnent beaucoup de réfléchir aux. Toutefois, elles sont un concept important lors de la spécification des dates et heures à l’aide de l’API managée EWS ou EWS. Mauvaise fuseaux horaires dans une API managées ou les EWS application peut produire des résultats inattendus. Gestion des fuseaux horaires correctement est facile, dans la mesure où vous savez comment.
  
## <a name="handling-time-zones-in-the-ews-managed-api"></a>Gestion des fuseaux horaires dans l’API managée EWS

Si vous utilisez l’API managée EWS, fuseaux horaires sont, pour l’essentiel, gérés automatiquement. Sans aucune action explicite de votre part, l’API utilise le fuseau horaire local de l’ordinateur client et gère toutes les conversions nécessaires en arrière-plan. Il s’agit très lorsque l’effet de votre choix, mais vous disposez d’autres options.
  
Une seule option consiste à définir la propriété [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) . Cette propriété contrôle le fuseau horaire pour toutes les demandes exécutées par l’API managée EWS. Cette propriété est en lecture seule ; le seul moyen qu’elle est via le constructeur de classe. Si vous utilisez le constructeur [ExchangeService (ExchangeVersion, System.TimeZoneInfo)](http://msdn.microsoft.com/en-us/library/dd636248%28v=exchg.80%29.aspx) ou [ExchangeService(System.TimeZoneInfo)](http://msdn.microsoft.com/en-us/library/dd635875%28v=exchg.80%29.aspx) , vous pouvez spécifier un fuseau horaire spécifique en tant qu’objet [System.TimeZoneInfo](http://msdn.microsoft.com/en-us/library/system.timezoneinfo%28v=vs.110%29.aspx) . Si vous utilisez un des constructeurs qui ne prennent pas un objet **TimeZoneInfo** en tant que paramètre, la classe **ExchangeService** définit la propriété de **fuseau horaire** pour le fuseau horaire actuel de l’ordinateur client. 
  
Si vous définissez un fuseau horaire spécifique ou conservez le fuseau horaire du client ordinateur, toutes les dates et heures sont exprimées dans le fuseau horaire représenté par la propriété de **fuseau horaire** . L’API managée EWS expose toutes les propriétés de date/heure en tant que structures [System.DateTime](http://msdn.microsoft.com/en-us/library/system.datetime%28v=vs.110%29.aspx) . Si vous définissez les propriétés de date/heure, donc ayant à l’esprit que l’heure spécifiée est interprété en fonction de la valeur de la propriété [DateTime.Kind](http://msdn.microsoft.com/en-us/library/system.datetime.kind%28v=vs.110%29.aspx) sur l’objet **DateTime** . Si la valeur de la propriété **type** est définie sur **non spécifié**, la valeur de **DateTime** est interprétée comme étant dans le fuseau horaire spécifié par la propriété de **fuseau horaire** . Si vous avez lu les propriétés de date/heure, toutes les propriétés de **DateTime** sont exprimées dans ce fuseau horaire. 
  
Si vous êtes [Création de rendez-vous ou réunions](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md) ou [mise à jour des rendez-vous ou réunions existant](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md), vous avez la possibilité de remplacer le fuseau horaire spécifié dans le **fuseau horaire** pour les nouveaux objets de [rendez-vous](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) . Toutefois, exactement ce que vous pouvez substituer dépend de la [version du schéma EWS](ews-schema-versions-in-exchange.md) vous ciblez. Toutes les valeurs de la propriété [ExchangeService.RequestedServerVersion](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) , vous pouvez définir [Appointment.StartTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) à utiliser un fuseau horaire spécifique pour cette réunion ou de rendez-vous. Si vous utilisez une valeur de la propriété **ExchangeService.RequestedServerVersion** supérieure à **Exchange2007_SP1**, vous pouvez également définir la propriété [Appointment.EndTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) , qui vous permet de spécifier un fuseau horaire pour le [ Appointment.End](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) propriété. Toutefois, l’esprit que ces propriétés n’affectent l’interprétation de la date/heure de la demande de création. Si vous récupérez le rendez-vous, les heures de début et de fin sont toujours exprimées dans le fuseau horaire spécifié par la propriété de **fuseau horaire** . 
  
Si vous mettez à jour des rendez-vous ou réunions existant, vous pouvez modifier le fuseau horaire pour un objet de **rendez-vous** en définissant la propriété **StartTimeZone** et/ou la propriété **EndTimeZone** . Sinon, les heures applicables doivent être décalées en conséquence. Si vous avez défini **ExchangeService.RequestedServerVersion** à **Exchange2007_SP1**, vous ne pouvez pas définir la propriété **EndTimeZone** ; la valeur de la propriété **StartTimeZone** servira à sa place. 
  
**Le tableau 1. Propriétés de fuseau horaire dans l’API managée EWS**

|**Propriété de fuseau horaire**|**Version de requête minimale du serveur**|**Description**|
|:-----|:-----|:-----|
|[Fuseau horaire](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |Si sa valeur via le constructeur de la classe **ExchangeService** , cette propriété est définie sur le fuseau horaire de l’ordinateur client. Toutes les propriétés de **DateTime** lors de la création d’éléments et lorsque les éléments de récupération existants sont exprimées dans ce fuseau horaire. Cette fois-ci zone peut être remplacée dans créer des demandes de rendez-vous et réunions en définissant **Appointment.StartTimeZone** et/ou la propriété **Appointment.EndTimeZone** . Si ne pas remplacée par la propriété **Appointment.StartTimeZone** , ce fuseau horaire est considéré comme le fuseau horaire de création pour les rendez-vous et réunions.  <br/> |
|[StartTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |Si défini sur les nouveaux objets de **rendez-vous** , ce fuseau horaire est utilisé pour interpréter les propriétés [Appointment.Start](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.start%28v=exchg.80%29.aspx) et [Appointment.ReminderDueBy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.reminderdueby%28v=exchg.80%29.aspx) . Ce fuseau horaire est également considéré comme le fuseau horaire de la création de l’objet du **rendez-vous** .  <br/> Lors de la récupération d’éléments existants, cette propriété est d’information uniquement. Les valeurs des propriétés de **DateTime** sur rendez-vous existant sont toujours exprimés dans le fuseau horaire spécifié par la propriété **ExchangeService.TimeZone** .  <br/> |
|[EndTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2010** <br/> |Si défini sur les nouveaux objets de **rendez-vous** , ce fuseau horaire est utilisé pour interpréter la propriété [Appointment.End](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) .  <br/> Lors de la récupération d’éléments existants, cette propriété est d’information uniquement. Les valeurs des propriétés de **DateTime** sur rendez-vous existant sont toujours exprimés dans le fuseau horaire spécifié par la propriété **ExchangeService.TimeZone** .  <br/> |
   
## <a name="handling-time-zones-in-ews"></a>Gestion des fuseaux horaires dans EWS

Si vous utilisez EWS, fuseaux horaires ne sont pas gérés automatiquement, et les choses sont un peu plus complexes. Impact des fuseaux horaires EWS demandes et réponses dépend de plusieurs facteurs :
  
- La version Exchange spécifiée dans l’élément [RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) 
    
- Le fuseau horaire spécifié dans l’élément [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) (le cas échéant) 
    
- Le fuseau horaire spécifié dans les éléments [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx), [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx)ou [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (le cas échéant rendez-vous ou réunions) 
    
- Le fuseau horaire spécifié dans les éléments de **dateTime** XML (le cas échéant) 
    
Le fuseau horaire spécifié dans la valeur de **dateTime** éléments peut prendre trois formes. Vous pouvez lire tous les détails dans [XML Schema Part 2 : types de données deuxième édition](http://www.w3.org/TR/xmlschema-2/#dateTime), mais de paraphraser :
  
- **Coordinated Universal Time (UTC) :** Spécifié par « Z ». Par exemple,`2014-06-06T19:00:00.000Z`
    
- **Fuseau horaire spécifique :** Spécifié par « + » ou «- » suivi des heures et minutes. Par exemple,`2014-06-06T19:00:00.000-08:00`
    
- **Aucun fuseau horaire :** Spécifié par l’absence d’un fuseau horaire. Par exemple,`2014-06-06T19:00:00.000`
    
Si un fuseau horaire est présent dans une valeur **dateTime** (UTC ou un fuseau horaire spécifique), cette valeur est toujours interprétée comme ce fuseau horaire. Si aucun fuseau horaire n’est présent, l’interprétation de la valeur dépend de la combinaison de ces autres éléments connexes fuseau horaire spécifique. 
  
**Le tableau 2. Éléments de fuseau horaire dans EWS et leurs effets**

|**RequestServerVersion**|**TimeZoneContext présent ?**|**EndTimeZone, StartTimeZone ou MeetingTimeZone présenter (CalendarItem et uniquement MeetingRequest) ?**|**dateTime au format UTC**|**dateTime dans le fuseau horaire spécifique**|**dateTime sans fuseau horaire**|**Rendez-vous et réunion fuseau horaire de création**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|**Exchange2007_SP1** <br/> |Oui  <br/> |Oui ( **MeetingTimeZone** )  <br/> |Interprété comme UTC  <br/> |Interprété comme indiqué dans la valeur de fuseau horaire  <br/> |Éléments dans l’élément [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) qui contient l’élément **MeetingTimeZone** sont considérés comme le fuseau horaire dans l’élément **MeetingTimeZone** , tous les autres interprétée comme UTC  <br/> |Fuseau horaire dans l’élément **MeetingTimeZone**  <br/> |
|**Exchange2007_SP1** <br/> |Oui  <br/> |Non  <br/> |Interprété comme UTC  <br/> |Interprété comme indiqué dans la valeur de fuseau horaire  <br/> |Interprété comme UTC  <br/> |UTC  <br/> |
|**Exchange2007_SP1** <br/> |Non  <br/> |Oui ( **MeetingTimeZone** )  <br/> |Interprété comme UTC  <br/> |Interprété comme indiqué dans la valeur de fuseau horaire  <br/> |Éléments dans l’élément [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) qui contient l’élément **MeetingTimeZone** sont considérés comme le fuseau horaire dans l’élément **MeetingTimeZone** , tous les autres interprétée comme UTC  <br/> |Fuseau horaire dans l’élément **MeetingTimeZone**  <br/> |
|**Exchange2007_SP1** <br/> |Non  <br/> |Non  <br/> |Interprété comme UTC  <br/> |Interprété comme indiqué dans la valeur de fuseau horaire  <br/> |Interprété comme UTC  <br/> |UTC  <br/> |
|**Exchange2010** et versions ultérieures  <br/> |Oui  <br/> |Oui ( **StartTimeZone** et/ou **EndTimeZone** )  <br/> |Interprété comme UTC  <br/> |Interprété comme indiqué dans la valeur de fuseau horaire  <br/> |Si l’élément **StartTimeZone** est présent, la valeur du [démarrage](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) et des éléments [ReminderDueBy](http://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) sont interprétées en tant que le fuseau horaire dans l’élément **StartTimeZone** . Sinon, la valeur de ces éléments sont interprétées en tant que le fuseau horaire dans l’élément **TimeZoneContext** .  <br/> Si l’élément **EndTimeZone** est présent, la valeur de l’élément de [démarrage](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) est interprétée comme le fuseau horaire dans l’élément **EndTimeZone** . Dans le cas contraire, la valeur de l’élément de **fin** est interprétée comme le fuseau horaire dans l’élément **TimeZoneContext** .  <br/> Éléments à l’extérieur du [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) sont considérés comme le fuseau horaire dans l’élément **TimeZoneContext** .  <br/> |Fuseau horaire dans l’élément **StartTimeZone** , le cas échéant, fuseau horaire dans l’élément **TimeZoneContext** dans le cas contraire  <br/> |
|**Exchange2010** et versions ultérieures  <br/> |Oui  <br/> |Non  <br/> |Interprété comme UTC  <br/> |Interprété comme indiqué dans la valeur de fuseau horaire  <br/> |Interprété comme le fuseau horaire dans l’élément **TimeZoneContext**  <br/> |Fuseau horaire dans l’élément **TimeZoneContext**  <br/> |
|**Exchange2010** et versions ultérieures  <br/> |Non  <br/> |Oui ( **StartTimeZone** et/ou **EndTimeZone** )  <br/> |Interprété comme UTC  <br/> |Interprété comme indiqué dans la valeur de fuseau horaire  <br/> |Si l’élément **StartTimeZone** est présent, la valeur du [démarrage](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) et des éléments [ReminderDueBy](http://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) sont interprétées en tant que le fuseau horaire dans l’élément **StartTimeZone** . Dans le cas contraire, la valeur de ces éléments sont interprétée comme UTC.  <br/> Si l’élément **EndTimeZone** est présent, la valeur de l’élément de [démarrage](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) est interprétée comme le fuseau horaire dans l’élément **EndTimeZone** . Dans le cas contraire, la valeur de l’élément de **fin** est interprétée comme UTC.  <br/> Éléments à l’extérieur du [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) sont considérés comme UTC.  <br/> |Fuseau horaire dans l’élément **StartTimeZone** , le cas échéant, UTC si pas  <br/> |
|**Exchange2010** et versions ultérieures  <br/> |Non  <br/> |Non  <br/> |Interprété comme UTC  <br/> |Interprété comme indiqué dans la valeur de fuseau horaire  <br/> |Interprété comme UTC  <br/> |UTC  <br/> |
   
Lors de l’interprétation des réponses à partir du serveur, vous devez toujours vérifier la valeur de chaque élément et interpréter la valeur en conséquence. Exchange inclut toujours un fuseau horaire (UTC ou un fuseau horaire spécifique) dans la valeur.
  
## <a name="additional-time-zone-considerations-when-creating-appointments-and-meetings"></a>Considérations supplémentaires fuseau horaire lors de la création de rendez-vous et réunions

Lorsque vous créez un rendez-vous ou une réunion, le fuseau horaire qui s’applique à l’heure de début est considéré comme le fuseau horaire de création pour le rendez-vous. En plus de contrôle de l’interprétation de la date/times lors de la création d’un rendez-vous ou une réunion, le fuseau horaire de création a les conséquences suivantes sur l’élément :
  
- Si l’élément est un événement d’une journée entière, il peut afficher de manière inattendue si affichés à partir d’un client qui utilise un fuseau horaire différent du fuseau horaire de création. Il s’agit de temps [lors de la création d’une journée entière](how-to-create-all-day-events-by-using-ews-in-exchange.md), le début et de fin des événements d’une journée entière sont ajustées à minuit le fuseau horaire de création. Ce temps s’affichera comme une heure que minuit dans un autre fuseau horaire, l’élément s’affiche couvrir jours supplémentaires. Pour cette raison, nous vous recommandons d’utiliser le fuseau horaire configuré pour le client de l’utilisateur principal du calendrier pour créer des événements sur une journée entière lorsque cela est possible.
    
- Si l’élément est une réunion, le fuseau horaire de création s’affichera dans la barre d’informations sur les demandes de réunion reçue par les participants, Outlook si ce fuseau horaire diffère du fuseau horaire du client.
    
## <a name="in-this-section"></a>Dans cette section

- [Créer des rendez-vous dans un fuseau horaire spécifique à l’aide de EWS dans Exchange](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)
    
- [Mettre à jour le fuseau horaire pour un rendez-vous à l’aide de EWS dans Exchange](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Versions de schéma EWS dans Exchange](ews-schema-versions-in-exchange.md)
    
- [Créer des rendez-vous et réunions à l’aide de EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Mettre à jour vos rendez-vous et réunions à l’aide de EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Créer des événements à l’aide de EWS dans Exchange](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [DateTime, Structure](http://msdn.microsoft.com/en-us/library/system.datetime%28v=vs.110%29.aspx)
    
- [Classe TimeZoneInfo](http://msdn.microsoft.com/en-us/library/system.timezoneinfo%28v=vs.110%29.aspx)
    

