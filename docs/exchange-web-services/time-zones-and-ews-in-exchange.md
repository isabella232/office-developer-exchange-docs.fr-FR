---
title: Fuseaux horaires et EWS dans Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 0e0a666c-0541-414b-a7fb-297d94f692e6
description: Découvrez comment les fuseaux horaires fonctionnent avec l’API managée EWS et EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 8435087d7709b77e7562e2b9d50ece58377dd8db
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463747"
---
# <a name="time-zones-and-ews-in-exchange"></a>Fuseaux horaires et EWS dans Exchange

Découvrez comment les fuseaux horaires fonctionnent avec l’API managée EWS et EWS dans Exchange.
  
Les fuseaux horaires ne sont pas quelque chose que la plupart des gens considèrent. Toutefois, il s’agit d’un concept important lors de la spécification des dates et des heures à l’aide de l’API managée EWS ou EWS. La manipulation des fuseaux horaires dans une API managée EWS ou une application EWS peut produire des résultats inattendus. Le traitement correct des fuseaux horaires est facile, aussi longtemps que vous le saurez.
  
## <a name="handling-time-zones-in-the-ews-managed-api"></a>Gestion des fuseaux horaires dans l’API managée EWS

Si vous utilisez l’API managée EWS, les fuseaux horaires sont, pour l’essentiel, gérés automatiquement pour vous. Sans action explicite de votre part, l’API utilise le fuseau horaire local de l’ordinateur client et gère toutes les conversions nécessaires en arrière-plan. C’est parfait lorsqu’il s’agit de l’effet souhaité, mais vous avez d’autres options.
  
La définition de la propriété [ExchangeService. TimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) est une option. Cette propriété contrôle le fuseau horaire pour toutes les demandes exécutées par l’API managée EWS. Cette propriété est en lecture seule ; le seul moyen de le définir se fait via le constructeur de classe. Si vous utilisez le constructeur [ExchangeService (System. TimeZoneInfo)](https://msdn.microsoft.com/library/dd635875%28v=exchg.80%29.aspx) ou [ExchangeService (ExchangeVersion, System. TimeZoneInfo)](https://msdn.microsoft.com/library/dd636248%28v=exchg.80%29.aspx) , vous pouvez spécifier un fuseau horaire spécifique en tant qu’objet [System. TimeZoneInfo](https://msdn.microsoft.com/library/system.timezoneinfo%28v=vs.110%29.aspx) . Si vous utilisez l’un des autres constructeurs qui ne prennent pas d’objet **TimeZoneInfo** en tant que paramètre, la classe **ExchangeService** définit la propriété **TimeZone** sur le fuseau horaire actuel de l’ordinateur client. 
  
Que vous définiez un fuseau horaire spécifique ou que vous le laissiez comme fuseau horaire de l’ordinateur client, toutes les dates et heures sont exprimées dans le fuseau horaire représenté par la propriété **TimeZone** . L’API managée EWS expose toutes les propriétés de date/heure sous forme de structures [System. DateTime](https://msdn.microsoft.com/library/system.datetime%28v=vs.110%29.aspx) . Par conséquent, si vous définissez des propriétés de date/heure, gardez à l’esprit que l’heure que vous spécifiez est interprétée en fonction de la valeur de la propriété [DateTime. Kind](https://msdn.microsoft.com/library/system.datetime.kind%28v=vs.110%29.aspx) de l’objet **DateTime** . Si la valeur de la propriété **Kind** est définie sur **unspécifié**, la valeur de la propriété **DateTime** est interprétée comme étant dans le fuseau horaire spécifié par la propriété **TimeZone** . Si vous lisez les propriétés de date/heure, toutes les propriétés **DateTime** sont exprimées dans ce fuseau horaire. 
  
Si vous [créez des rendez-vous ou des réunions](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md) ou que vous [Mettez à jour des rendez-vous ou des réunions existants](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md), vous avez la possibilité de remplacer le fuseau horaire spécifié dans le fuseau **horaire pour les** nouveaux objets de [rendez-](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) vous. Toutefois, ce que vous pouvez remplacer exactement dépend de la [version de schéma EWS](ews-schema-versions-in-exchange.md) que vous ciblez. Pour toutes les valeurs de la propriété [ExchangeService. RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) , vous pouvez définir le [rendez-vous. StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) de sorte qu’il utilise un fuseau horaire spécifique pour ce rendez-vous ou cette réunion. Si vous utilisez une valeur pour la propriété **ExchangeService. RequestedServerVersion** supérieure à **Exchange2007_SP1**, vous pouvez également définir la propriété appointment [. EndTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) , ce qui vous permet de spécifier un fuseau horaire pour la propriété appointment [. end](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) . Toutefois, gardez à l’esprit que ces propriétés affectent uniquement l’interprétation de la date/l’heure de la demande de création. Si vous récupérez le rendez-vous, les heures de début et de fin sont toujours exprimées dans le fuseau horaire spécifié par la propriété **TimeZone** . 
  
Si vous mettez à jour des rendez-vous ou des réunions existants, vous pouvez modifier le fuseau horaire d’un objet de **rendez-** vous en définissant la propriété **StartTimeZone** et/ou la propriété **EndTimeZone** . Cette opération entraînera le changement en conséquence. Si vous avez défini le **ExchangeService. RequestedServerVersion** sur **Exchange2007_SP1**, vous ne pouvez pas définir la propriété **EndTimeZone** ; la valeur de la propriété **StartTimeZone** est utilisée à la place. 
  
**Tableau 1. Propriétés des fuseaux horaires dans l’API managée EWS**

|**Propriété de fuseau horaire**|**Version de demande serveur minimale**|**Description**|
|:-----|:-----|:-----|
|[Horaire](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |Si elle n’est pas définie via le constructeur de la classe **ExchangeService** , cette propriété est définie sur le fuseau horaire de l’ordinateur client. Toutes les propriétés **DateTime** lors de la création d’éléments et lors de la récupération d’éléments existants sont exprimées dans ce fuseau horaire. Ce fuseau horaire peut être remplacé dans créer des demandes de rendez-vous et de réunions en définissant la propriété appointment **. StartTimeZone** et/ou la propriété appointment **. EndTimeZone** . Si elle n’est pas remplacée par la propriété appointment **. StartTimeZone** , ce fuseau horaire est considéré comme le fuseau horaire de création pour les rendez-vous et les réunions.  <br/> |
|[StartTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |S’il est défini sur de nouveaux objets de **rendez-vous** , ce fuseau horaire est utilisé pour interpréter les propriétés [rendez-vous. Start](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.start%28v=exchg.80%29.aspx) et appointment [. ReminderDueBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.reminderdueby%28v=exchg.80%29.aspx) . Ce fuseau horaire est également considéré comme le fuseau horaire de création de l’objet de **rendez-vous** .  <br/> Lors de la récupération d’éléments existants, cette propriété est uniquement informatif. Les valeurs des propriétés **DateTime** sur un rendez-vous existant sont toujours exprimées dans le fuseau horaire spécifié par la propriété **ExchangeService. TimeZone** .  <br/> |
|[EndTimeZone](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2010** <br/> |S’il est défini sur de nouveaux objets de **rendez-vous** , ce fuseau horaire est utilisé pour interpréter la propriété appointment [. end](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) .  <br/> Lors de la récupération d’éléments existants, cette propriété est uniquement informatif. Les valeurs des propriétés **DateTime** sur un rendez-vous existant sont toujours exprimées dans le fuseau horaire spécifié par la propriété **ExchangeService. TimeZone** .  <br/> |
   
## <a name="handling-time-zones-in-ews"></a>Gestion des fuseaux horaires dans EWS

Si vous utilisez EWS, les fuseaux horaires ne sont pas gérés automatiquement, et les choses sont un peu plus compliquées. La manière dont les fuseaux horaires ont un impact sur les demandes et les réponses EWS dépend d’un certain nombre de facteurs :
  
- La version d’Exchange spécifiée dans l’élément [RequestServerVersion](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) 
    
- Le fuseau horaire spécifié dans l’élément [TimeZoneContext](https://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) (le cas échéant) 
    
- Le fuseau horaire spécifié dans les éléments [MeetingTimeZone](https://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx), [StartTimeZone](https://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx)ou [EndTimeZone](https://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) (s’il est présent sur les rendez-vous ou les réunions). 
    
- Le fuseau horaire spécifié dans les éléments XML **DateTime** (le cas échéant) 
    
Le fuseau horaire spécifié dans la valeur des éléments **DateTime** peut prendre trois formes. Vous pouvez lire tous les détails dans le [schéma XML part 2 : Datatypes Second Edition](http://www.w3.org/TR/xmlschema-2/#dateTime), mais à paraphrase :
  
- **Temps universel coordonné (UTC) :** Spécifié par « Z ». Par exemple,  `2014-06-06T19:00:00.000Z`.
    
- **Fuseau horaire spécifique :** Spécifié par « + » ou « - » suivi par les heures et les minutes. Par exemple,  `2014-06-06T19:00:00.000-08:00`.
    
- **Aucun fuseau horaire :** Spécifié par l’absence de fuseau horaire. Par exemple,  `2014-06-06T19:00:00.000`.
    
Si un fuseau horaire est présent dans une valeur **DateTime** (UTC ou fuseau horaire spécifique), cette valeur est toujours interprétée comme le fuseau horaire. Si aucun fuseau horaire n’est présent, l’interprétation de la valeur dépend de la combinaison spécifique des autres éléments liés au fuseau horaire. 
  
**Tableau 2. Éléments de fuseau horaire dans EWS et leurs effets**

|**RequestServerVersion**|**TimeZoneContext présent ?**|**MeetingTimeZone, StartTimeZone ou EndTimeZone présent (CalendarItem et propriété meetingrequest uniquement) ?**|**Date et heure au format UTC**|**Date et heure dans un fuseau horaire spécifique**|**dateTime sans fuseau horaire**|**Fuseau horaire de création de réunion et de rendez-vous**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|**Exchange2007_SP1** <br/> |Oui  <br/> |Oui ( **MeetingTimeZone** )  <br/> |Interprété comme UTC  <br/> |Interprété comme le fuseau horaire indiqué dans la valeur  <br/> |Les éléments au sein de l’élément [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [propriété meetingrequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) qui contient l’élément **MeetingTimeZone** sont interprétés comme le fuseau horaire de l’élément **MeetingTimeZone** , tous les autres étant interprétés comme UTC  <br/> |Fuseau horaire dans l’élément **MeetingTimeZone**  <br/> |
|**Exchange2007_SP1** <br/> |Oui  <br/> |Non  <br/> |Interprété comme UTC  <br/> |Interprété comme le fuseau horaire indiqué dans la valeur  <br/> |Interprété comme UTC  <br/> |UTC  <br/> |
|**Exchange2007_SP1** <br/> |Non  <br/> |Oui ( **MeetingTimeZone** )  <br/> |Interprété comme UTC  <br/> |Interprété comme le fuseau horaire indiqué dans la valeur  <br/> |Les éléments au sein de l’élément [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou [propriété meetingrequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) qui contient l’élément **MeetingTimeZone** sont interprétés comme le fuseau horaire de l’élément **MeetingTimeZone** , tous les autres étant interprétés comme UTC  <br/> |Fuseau horaire dans l’élément **MeetingTimeZone**  <br/> |
|**Exchange2007_SP1** <br/> |Non  <br/> |Non  <br/> |Interprété comme UTC  <br/> |Interprété comme le fuseau horaire indiqué dans la valeur  <br/> |Interprété comme UTC  <br/> |UTC  <br/> |
|**Exchange2010** et versions ultérieures  <br/> |Oui  <br/> |Oui ( **StartTimeZone** et/ou **EndTimeZone** )  <br/> |Interprété comme UTC  <br/> |Interprété comme le fuseau horaire indiqué dans la valeur  <br/> |Si l’élément **StartTimeZone** est présent, la valeur des éléments [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) et [ReminderDueBy](https://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) est interprétée comme le fuseau horaire dans l’élément **StartTimeZone** . Dans le cas contraire, la valeur de ces éléments est interprétée comme le fuseau horaire dans l’élément **TimeZoneContext** .  <br/> Si l’élément **EndTimeZone** est présent, la valeur de l’élément [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) est interprétée comme le fuseau horaire dans l’élément **EndTimeZone** . Dans le cas contraire, la valeur de l’élément **end** est interprétée comme le fuseau horaire dans l’élément **TimeZoneContext** .  <br/> Les éléments situés en dehors de [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou de [propriété meetingrequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) sont interprétés comme le fuseau horaire dans l’élément **TimeZoneContext** .  <br/> |Fuseau horaire dans l’élément **StartTimeZone** s’il est présent, fuseau horaire dans l’élément **TimeZoneContext** , si ce n’est pas le cas  <br/> |
|**Exchange2010** et versions ultérieures  <br/> |Oui  <br/> |Non  <br/> |Interprété comme UTC  <br/> |Interprété comme le fuseau horaire indiqué dans la valeur  <br/> |Interprété comme le fuseau horaire dans l’élément **TimeZoneContext**  <br/> |Fuseau horaire dans l’élément **TimeZoneContext**  <br/> |
|**Exchange2010** et versions ultérieures  <br/> |Non  <br/> |Oui ( **StartTimeZone** et/ou **EndTimeZone** )  <br/> |Interprété comme UTC  <br/> |Interprété comme le fuseau horaire indiqué dans la valeur  <br/> |Si l’élément **StartTimeZone** est présent, la valeur des éléments [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) et [ReminderDueBy](https://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) est interprétée comme le fuseau horaire dans l’élément **StartTimeZone** . Dans le cas contraire, la valeur de ces éléments est interprétée comme étant UTC.  <br/> Si l’élément **EndTimeZone** est présent, la valeur de l’élément [Start](https://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) est interprétée comme le fuseau horaire dans l’élément **EndTimeZone** . Dans le cas contraire, la valeur de l’élément **end** est interprétée comme étant UTC.  <br/> Les éléments en dehors de [CalendarItem](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) ou de [propriété meetingrequest](https://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) sont interprétés en tant que UTC.  <br/> |Fuseau horaire dans l’élément **StartTimeZone** s’il est présent, UTC s’il ne l’est pas  <br/> |
|**Exchange2010** et versions ultérieures  <br/> |Non  <br/> |Non  <br/> |Interprété comme UTC  <br/> |Interprété comme le fuseau horaire indiqué dans la valeur  <br/> |Interprété comme UTC  <br/> |UTC  <br/> |
   
Lors de l’interprétation des réponses à partir du serveur, vous devez toujours vérifier la valeur de chaque élément et interpréter la valeur en conséquence. Exchange inclut toujours un fuseau horaire (UTC ou un fuseau horaire spécifique) dans la valeur.
  
## <a name="additional-time-zone-considerations-when-creating-appointments-and-meetings"></a>Considérations supplémentaires relatives aux fuseaux horaires lors de la création de rendez-vous et de réunions

Lorsque vous créez un rendez-vous ou une réunion, le fuseau horaire qui s’applique à l’heure de début est considéré comme le fuseau horaire de création du rendez-vous. Outre le contrôle de la façon dont les dates et les heures sont interprétées lors de la création d’un rendez-vous ou d’une réunion, le fuseau horaire de création a les effets suivants sur l’élément :
  
- Si l’élément est un événement d’une journée entière, il peut s’afficher d’une manière inattendue s’il est affiché à partir d’un client qui utilise un fuseau horaire différent du fuseau horaire de création. En effet, [lorsqu’un événement d’une journée entière est créé](how-to-create-all-day-events-by-using-ews-in-exchange.md), l’heure de début et l’heure de fin des événements d’une journée entière sont ajustées à minuit du fuseau horaire de création. Cette heure s’affiche sous la forme d’une heure différente de minuit dans un autre fuseau horaire, de sorte que l’élément semble s’étendre sur des jours supplémentaires. Pour cette raison, nous vous recommandons d’utiliser le fuseau horaire configuré pour le client principal de calendrier de l’utilisateur afin de créer des événements sur une journée entière lorsque cela est possible.
    
- Si l’élément est une réunion, le fuseau horaire de création est affiché dans la barre d’informations Outlook sur les demandes de réunion reçues par les participants, si ce fuseau horaire diffère du fuseau horaire de leur client.
    
## <a name="in-this-section"></a>Dans cette section

- [Créer des rendez-vous dans un fuseau horaire spécifique à l’aide d’EWS dans Exchange](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)
    
- [Mettre à jour le fuseau horaire pour un rendez-vous à l’aide d’EWS dans Exchange](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Voir aussi


- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Versions de schéma EWS dans Exchange](ews-schema-versions-in-exchange.md)
    
- [Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Créer des événements sur une journée entière à l'aide d’EWS dans Exchange](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [Structure DateTime](https://msdn.microsoft.com/library/system.datetime%28v=vs.110%29.aspx)
    
- [Classe TimeZoneInfo](https://msdn.microsoft.com/library/system.timezoneinfo%28v=vs.110%29.aspx)
    

