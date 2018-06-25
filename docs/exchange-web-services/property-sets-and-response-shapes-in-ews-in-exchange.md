---
title: Jeux de propriétés et de réponse des formes dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 04a29804-6067-48e7-9f5c-534e253a230e
description: Apprenez à gérer les formes de réponse et jeux de propriétés qui sont renvoyées par la EWS gérés API et EWS dans Exchange.
ms.openlocfilehash: d9fd6c155438dfd03cfc9536397316cf3faa2287
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755083"
---
# <a name="property-sets-and-response-shapes-in-ews-in-exchange"></a>Jeux de propriétés et de réponse des formes dans EWS dans Exchange

Apprenez à gérer les formes de réponse et jeux de propriétés qui sont renvoyées par la EWS gérés API et EWS dans Exchange.
  
Le magasin de données Exchange fournit une solution de stockage flexible qui vous permet de stocker différents éléments, tels que des contacts et des entrées de calendrier, dans le même dossier. Toutefois, elle peut rendre difficile à gérer les données qui sont renvoyées à partir d’un appel à une opération EWS ou une méthode de l’API managée.
  
Pour le rendre plus facile de gérer les données qui sont retournées par Exchange Online, Exchange Online dans le cadre d’Office 365, ou la version de Excahange commençant par Exchange 2013, l’API managée EWS utilise des jeux de propriétés et EWS formes de réponse. Il s’agit de collections prédéfinies qui fournissent les propriétés d’un élément de magasin les plus courants. Le jeu de propriétés renvoyé est déterminé par le type d’élément. Cela signifie que lorsque vous liez un élément à l’aide de la méthode de l' API managée Exchange [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) , vous obtenez un ensemble différent de propriétés en fonction du type d’élément auquel lier. Liaison à un élément de calendrier renvoie un ensemble différent de propriétés de liaison à un élément de contact. De même, si vous utilisez EWS, l' [opération GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) renvoie un ensemble différent de propriétés en fonction du type d’élément qui est renvoyé. 
  
Liaison à un dossier avec la méthode [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) ou à l’aide de l' [opération GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) retourne également différentes propriétés basées sur le dossier que vous demander. 
  
**Le tableau 1. Formes de réponse prédéfinie**

|**Forme de réponse**|**Équivalent de l’API managée EWS**|**Description**|
|:-----|:-----|:-----|
|ID uniquement  <br/> |[BasePropertySet.IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Renvoie uniquement l’identificateur de l’élément ou d’un dossier. La plupart des applications, utilisez cette forme de réponse et spécifier des propriétés supplémentaires qui sont requises.  <br/> |
|Default (Défaut)  <br/> |S/O  <br/> |Renvoie un ensemble prédéfini des propriétés par défaut pour l’élément ou d’un dossier (EWS uniquement).  <br/> |
|Toutes les propriétés  <br/> |[BasePropertySet.FirstClassProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Renvoie les propriétés des applications clientes plus souvent utilisent. Vous pouvez retourner des propriétés supplémentaires à l’aide d’un chemin d’accès de la propriété.  <br/> |
   
## <a name="default-response-shapes"></a>Formes de réponse par défaut

EWS inclut un ensemble de formes de réponse par défaut pour les dossiers et des éléments. 
  
Le tableau suivant répertorie les propriétés par défaut qui sont renvoyées pour chaque dossier par les opérations [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) et [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) EWS. 
  
**Le tableau 2. Propriétés de dossier par défaut**

|**Propriété**|**Boîte de réception**|**Calendrier**|**Contacts**|**Éléments supprimés**|**Brouillons**|**Remarques**|**Autres dossiers**|**La boîte d’envoi**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Nom d’affichage  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|ID de dossier  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Nombre de sous-dossiers  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Nombre total de  <br/> |X   <br/> ||X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Nombre non lu  <br/> |X   <br/> |||X   <br/> |X   <br/> ||X   <br/> |X   <br/> |
   
Le tableau suivant répertorie les propriétés par défaut qui sont renvoyées pour chaque type d’élément par les opérations [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) et EWS [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) . 
  
**Le tableau 3. Propriétés de l’élément par défaut**

|**Propriété**|**Élément de calendrier**|**Élément de contact**|**Élément de message**|**Élément de tâche**|
|:-----|:-----|:-----|:-----|:-----|
|Corps  <br/> |||X(1)  <br/> ||
|CalendarItemType  <br/> ||x  <br/> |||
|CompanyName  <br/> ||x  <br/> |||
|CompleteName  <br/> ||x  <br/> |||
|DateTimeCreated  <br/> |||x  <br/> ||
|DateTimeSent  <br/> |||x  <br/> ||
|DueDate  <br/> ||||x(2)  <br/> |
|EmailAddresses  <br/> ||x  <br/> |||
|End  <br/> |x  <br/> ||||
|Classer sous  <br/> ||x  <br/> |||
|De  <br/> |||x  <br/> ||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ImAddresses  <br/> ||x  <br/> |||
|IsAssociated  <br/> |x  <br/> ||x  <br/> ||
|IsDeliveryReceiptRequested  <br/> |||x  <br/> ||
|ItemId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|JobTitle  <br/> ||x  <br/> |||
|LegacyFreeBusyStatus  <br/> |x  <br/> ||||
|Emplacement  <br/> |x  <br/> ||||
|Organisateur  <br/> |x  <br/> ||||
|PercentComplete  <br/> ||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> |||
|PhysicalAddresses  <br/> ||x  <br/> |||
|ResponseObjects  <br/> |x(1)  <br/> ||x(1)  <br/> ||
|Sensitity  <br/> |||x  <br/> ||
|Size  <br/> |||x  <br/> ||
|Date de début  <br/> ||||x(2)  <br/> |
|État  <br/> ||||x  <br/> |
|Objet  <br/> |x  <br/> ||x  <br/> |x  <br/> |
   
Notes :
  
1. Inclus dans la réponse de l’opération **GetItem** . Non inclus dans la réponse de l’opération **FindItem** . 
    
2. Uniquement inclus dans la réponse si le champ contient des données. Non inclus dans la réponse si le champ est vide.
    
### <a name="all-properties-set-and-response-shape"></a>Forme d’ensemble et réponse toutes les propriétés

Le tableau suivant répertorie les propriétés de première classe qui sont retournées par l’appel de l' API managée EWS [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) et méthodes d’API managées [Item.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) et la forme de réponse « toutes les propriétés » renvoyés par la [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) et [ GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) opérations EWS. 
  
Vous pouvez ajouter des propriétés supplémentaires à la propriété définir ou incluent les propriétés étendues. Pour plus d’informations, voir les [propriétés et les propriétés étendues dans EWS dans Exchange](properties-and-extended-properties-in-ews-in-exchange.md).
  
**Le tableau 4. Propriétés de première classe**

|||||||
|:-----|:-----|:-----|:-----|:-----|:-----|
|Property  <br/> |Élément de calendrier  <br/> |Élément de contact  <br/> |Élément de message  <br/> |Élément de publication  <br/> |Élément de tâche  <br/> |
|ActualWork  <br/> |||||x  <br/> |
|AdjacentMeetingCount  <br/> |x  <br/> |||||
|AdjacentMeetings  <br/> |x  <br/> |||||
|Alias  <br/> ||x  <br/> ||||
|AllowNewTimeProposal  <br/> |x  <br/> |||||
|AppointmentReplyTime  <br/> |x  <br/> |||||
|AppointmentSequenceNumber  <br/> |x  <br/> |||||
|AppointmentState  <br/> |x  <br/> |||||
|AssignedTime  <br/> |||||x  <br/> |
|AssistantName  <br/> ||x  <br/> ||||
|BccRecipients  <br/> |||x  <br/> |||
|BillingInformation  <br/> |||||x  <br/> |
|Corps  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> ||x(1)  <br/> |
|BusinessHomePage  <br/> ||x  <br/> |x  <br/> |||
|CalendarItemType  <br/> |x  <br/> |||||
|Catégories  <br/> |x  <br/> ||x  <br/> |x  <br/> |x  <br/> |
|CcRecipients  <br/> |||x  <br/> |||
|ChangeCount  <br/> |||||x  <br/> |
|Enfants  <br/> ||x  <br/> ||||
|Companies  <br/> |||||x  <br/> |
|CompleteDate  <br/> |||||x  <br/> |
|CompleteName  <br/> ||x  <br/> ||||
|ConferenceType  <br/> |x  <br/> |||||
|ConflictingMeetingCount  <br/> |x  <br/> |||||
|ConflictingMeetings  <br/> |x  <br/> |||||
|Contacts  <br/> |||||x  <br/> |
|ContactSource  <br/> ||x  <br/> ||||
|ConversationId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ConversationIndex  <br/> |||x  <br/> |x  <br/> ||
|ConversationTopic  <br/> |||x  <br/> |x  <br/> ||
|Culture  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeCreated  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeReceived  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeSent  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DateTimeStamp  <br/> |x  <br/> |||||
|DelegationState  <br/> |||||x  <br/> |
|Personne  <br/> |||||x  <br/> |
|DeletedOccurances  <br/> |x  <br/> |||||
|Service  <br/> ||x  <br/> ||||
|DirectoryId  <br/> ||x  <br/> ||||
|DirectReports  <br/> ||x  <br/> ||||
|DisplayCc  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DisplayName  <br/> ||x  <br/> ||||
|DisplayTo  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DueDate  <br/> |||||x  <br/> |
|Duration  <br/> |x  <br/> |||||
|EffectiveRights  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|EmailAddresses  <br/> ||x  <br/> ||||
|End  <br/> |x  <br/> |||||
|EndTimeZone  <br/> |x  <br/> |||||
|Classer sous  <br/> ||x  <br/> ||||
|FileAsMapping  <br/> ||x  <br/> ||||
|FirstOccurance  <br/> |x  <br/> |||||
|De  <br/> |||x  <br/> |x  <br/> ||
|Génération  <br/> ||x  <br/> ||||
|Prénom  <br/> ||x  <br/> ||||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|HasPicture  <br/> ||x  <br/> ||||
|ImAddresses  <br/> ||x  <br/> ||||
|Importance  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Initiales  <br/> ||x  <br/> ||||
|InReplyTo  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|InternetMessageId  <br/> |||x  <br/> |x  <br/> ||
|InternetMessageHeaders  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsAllDayEvent  <br/> |x  <br/> |||||
|IsAssociated  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsCancelled  <br/> |x  <br/> |||||
|Avertisse  <br/> |||||x  <br/> |
|IsDeliveryReceiptRequested  <br/> |||x  <br/> |||
|IsDraft  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsFromMe  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsMeeting  <br/> |x  <br/> |||||
|IsOnlineMeeting  <br/> |x  <br/> |||||
|Estlu  <br/> |||x  <br/> |||
|IsReadReceiptRequested  <br/> |||x  <br/> |||
|IsRecurring  <br/> |x  <br/> ||||x  <br/> |
|IsResend  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsResponseRequested  <br/> |x  <br/> ||x  <br/> |||
|IsSubmitted  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsUnmodified  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ItemClass  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ItemId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|JobTitle  <br/> ||x  <br/> ||||
|LastModifiedName  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Heure de dernière modification  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|LastOccurrance  <br/> |x  <br/> |||||
|LegacyFreeBusyStatus  <br/> |x  <br/> |||||
|Emplacement  <br/> |x  <br/> |||||
|Manager  <br/> ||x  <br/> ||||
|MeetingRequestWasSent  <br/> |x  <br/> |||||
|MeetingTimeZone  <br/> |x  <br/> |||||
|MeetingWorkspaceUrl  <br/> |x  <br/> |||||
|MiddleName  <br/> ||x  <br/> ||||
|Kilométrage  <br/> ||x  <br/> |||x  <br/> |
|ModifiedOccurrances  <br/> |x  <br/> |||||
|MyResponseType  <br/> |x  <br/> |||||
|NetShowUrl  <br/> |x  <br/> |||||
|Surnom  <br/> ||x  <br/> ||||
|Remarques  <br/> ||x  <br/> ||||
|OfficeLocation  <br/> ||x  <br/> ||||
|OptionalAttendees  <br/> |x  <br/> |||||
|Organisateur  <br/> |x  <br/> |||||
|OriginalStart  <br/> |x  <br/> |||||
|Owner  <br/> |||||x  <br/> |
|ParentFolderId  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|PercentComplete  <br/> |||||x  <br/> |
|PhoneNumbers  <br/> ||x  <br/> ||||
|PhoneticFirstName  <br/> ||x  <br/> ||||
|PhoneticFullName  <br/> ||x  <br/> ||||
|PhoneticLastName  <br/> ||x  <br/> ||||
|Photo  <br/> ||x  <br/> ||||
|PhysicalAddresses  <br/> ||x  <br/> ||||
|PostalAddressIndex  <br/> ||x  <br/> ||||
|PostedTime  <br/> ||||x  <br/> ||
|Profession  <br/> ||x  <br/> ||||
|Reçu par  <br/> |||x  <br/> |||
|ReceivedRepresenting  <br/> |||x  <br/> |||
|Reccurrence  <br/> |x  <br/> ||||x  <br/> |
|Références  <br/> |||x  <br/> |x  <br/> ||
|ReminderDueBy  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReminderIsSet  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReminderMinutesBeforeStart  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|ReplyTo  <br/> |||x  <br/> |||
|RequiredAttendees  <br/> |x  <br/> |||||
|Ressources  <br/> |x  <br/> |||||
|ResponseObjects  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |x(1)  <br/> |
|Expéditeur  <br/> |||x  <br/> |x  <br/> ||
|Critère de diffusion  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Size  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|NomEpoux  <br/> ||x  <br/> ||||
|Démarrer  <br/> |x  <br/> |||||
|Date de début  <br/> |||||x  <br/> |
|StartTimeZone  <br/> |x  <br/> |||||
|État  <br/> |||||x  <br/> |
|StatusDescription  <br/> |||||x  <br/> |
|Objet  <br/> |x  <br/> |x  <br/> |x  <br/> ||x  <br/> |
|Nom de famille  <br/> ||x  <br/> ||||
|TimeZone  <br/> |x  <br/> |||||
|ToRecipients  <br/> |||x  <br/> |||
|TotalWork  <br/> |||||x  <br/> |
|WebClientEditFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|WebClientReadFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
   
Notes :
  
1. Inclus lorsque [la liaison à un élément](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) et dans la réponse de l' [opération GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx). Non inclus dans le résultat de la méthode [Item.FindItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou la réponse de l' [opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).
    
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Opération FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [GetItem Operation](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)
    
- [Opération FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Opération GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)
    

