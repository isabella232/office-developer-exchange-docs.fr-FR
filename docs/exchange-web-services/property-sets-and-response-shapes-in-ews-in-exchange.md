---
title: Jeux de propriétés et de réponse des formes dans EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 04a29804-6067-48e7-9f5c-534e253a230e
description: Découvrez comment gérer les formes de réponse et les jeux de propriétés renvoyés par l’API gérée EWS et EWS dans Exchange.
ms.openlocfilehash: 7720a07a6fd288f289bba371ce6fd8a6e349a8ce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543848"
---
# <a name="property-sets-and-response-shapes-in-ews-in-exchange"></a>Jeux de propriétés et de réponse des formes dans EWS dans Exchange

Découvrez comment gérer les formes de réponse et les jeux de propriétés renvoyés par l’API gérée EWS et EWS dans Exchange.
  
Le magasin Exchange de données fournit une solution de stockage flexible qui vous permet de stocker différents éléments, tels que des contacts et des entrées de calendrier, dans le même dossier . toutefois, il peut être difficile de gérer les données renvoyées par un appel à une opération EWS ou à une méthode d’API gérée EWS.
  
Pour faciliter la gestion des données renvoyées par Exchange Online, Exchange Online dans le cadre de Office 365 ou de la version d’Exc bigge à partir de Exchange 2013, l’API gérée EWS utilise des jeux de propriétés et EWS utilise des formes de réponse. Il s’agit de collections prédéfinie qui fournissent les propriétés les plus courantes d’un élément de magasin. L’ensemble des propriétés renvoyées est déterminé par le type d’élément. Cela signifie que lorsque vous liez un élément à l’aide de la méthode [item.bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) de l’API gérée Exchange, vous obtenez un ensemble différent de propriétés en fonction du type d’élément auquel vous liez. La liaison à un élément de calendrier retourne un ensemble de propriétés différent de la liaison à un élément de contact. De même, si vous utilisez EWS, l’opération [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) renvoie un ensemble différent de propriétés en fonction du type d’élément renvoyé. 
  
La liaison à un dossier à l’aide de la méthode [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) ou à l’aide de l’opération [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) renvoie également différents ensembles de propriétés en fonction du dossier que vous demandez. 
  
**Tableau 1. Formes de réponse prédéfinies**

|**Forme de réponse**|**Équivalent d’API gérée EWS**|**Description**|
|:-----|:-----|:-----|
|ID uniquement  <br/> |[BasePropertySet.IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Renvoie uniquement l’identificateur de l’élément ou du dossier. La plupart des applications doivent utiliser cette forme de réponse et spécifier les propriétés supplémentaires qui sont requises.  <br/> |
|Par défaut  <br/> |N/A  <br/> |Renvoie un ensemble prédéféré de propriétés qui sont la valeur par défaut pour l’élément ou le dossier (EWS uniquement).  <br/> |
|Toutes les propriétés  <br/> |[BasePropertySet.FirstClassProperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) <br/> |Renvoie les propriétés que les applications clientes utilisent le plus souvent. Vous pouvez renvoyer des propriétés supplémentaires à l’aide d’un chemin de propriété.  <br/> |
   
## <a name="default-response-shapes"></a>Formes de réponse par défaut

EWS inclut un ensemble de formes de réponse par défaut pour les dossiers et les éléments. 
  
Le tableau suivant répertorie les propriétés par défaut renvoyées pour chaque dossier par les opérations [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) et [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) EWS. 
  
**Tableau 2. Propriétés de dossier par défaut**

|**Propriété**|**Boîte de réception**|**Calendar**|**Contacts**|**Éléments supprimés**|**Brouillons**|**Remarques**|**Autres dossiers**|**Boîte d’envoi**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Nom d’affichage  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Identificateur de dossier  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Nombre de sous-foldages  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Nombre total  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Nombre de non-lus  <br/> |X  <br/> |||X  <br/> |X  <br/> ||X  <br/> |X  <br/> |
   
Le tableau suivant répertorie les propriétés par défaut renvoyées pour chaque type d’élément par les opérations [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) et [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS. 
  
**Tableau 3. Propriétés d’élément par défaut**

|**Propriété**|**Élément de calendrier**|**Contact**|**Élément de message**|**Tâche**|
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
|FileAs  <br/> ||x  <br/> |||
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
|StartDate  <br/> ||||x(2)  <br/> |
|État  <br/> ||||x  <br/> |
|Sujet  <br/> |x  <br/> ||x  <br/> |x  <br/> |
   
Remarques :
  
1. Inclus dans la réponse de **l’opération GetItem.** Non inclus dans la réponse de **l’opération FindItem.** 
    
2. Inclus uniquement dans la réponse si le champ contient des données. Non inclus dans la réponse si le champ est vide.
    
### <a name="all-properties-set-and-response-shape"></a>Toutes les propriétés définies et forme de réponse

Le tableau suivant répertorie les propriétés de première classe renvoyées en appelant les méthodes d’API gérée EWS [Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) et [Item.FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) EWS, ainsi que la forme de réponse « toutes les propriétés » renvoyée par les opérations [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) et [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS. 
  
Vous pouvez ajouter des propriétés supplémentaires au jeu de propriétés ou inclure des propriétés étendues. Pour plus d’informations, voir [Propriétés et propriétés étendues dans EWS dans Exchange](properties-and-extended-properties-in-ews-in-exchange.md).
  
**Tableau 4. Propriétés de première classe**

|||||||
|:-----|:-----|:-----|:-----|:-----|:-----|
|Property  <br/> |Élément de calendrier  <br/> |Contact  <br/> |Élément de message  <br/> |Élément de publication  <br/> |Tâche  <br/> |
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
|Categories  <br/> |x  <br/> ||x  <br/> |x  <br/> |x  <br/> |
|CcRecipients  <br/> |||x  <br/> |||
|ChangeCount  <br/> |||||x  <br/> |
|Children  <br/> ||x  <br/> ||||
|Sociétés  <br/> |||||x  <br/> |
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
|Delegator  <br/> |||||x  <br/> |
|DeletedOccurrences  <br/> |x  <br/> |||||
|Service  <br/> ||x  <br/> ||||
|DirectoryId  <br/> ||x  <br/> ||||
|DirectReports  <br/> ||x  <br/> ||||
|DisplayCc  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DisplayName  <br/> ||x  <br/> ||||
|DisplayTo  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|DueDate  <br/> |||||x  <br/> |
|Durée  <br/> |x  <br/> |||||
|EffectiveRights  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|EmailAddresses  <br/> ||x  <br/> ||||
|End  <br/> |x  <br/> |||||
|EndTimeZone  <br/> |x  <br/> |||||
|FileAs  <br/> ||x  <br/> ||||
|FileAsMapping  <br/> ||x  <br/> ||||
|FirstOccurrence  <br/> |x  <br/> |||||
|De  <br/> |||x  <br/> |x  <br/> ||
|Generation  <br/> ||x  <br/> ||||
|GivenName  <br/> ||x  <br/> ||||
|HasAttachments  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|HasPicture  <br/> ||x  <br/> ||||
|ImAddresses  <br/> ||x  <br/> ||||
|Importance  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Initials  <br/> ||x  <br/> ||||
|InReplyTo  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|InternetMessageId  <br/> |||x  <br/> |x  <br/> ||
|InternetMessageHeaders  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsAllDayEvent  <br/> |x  <br/> |||||
|IsAssociated  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsCancelled  <br/> |x  <br/> |||||
|IsComplete  <br/> |||||x  <br/> |
|IsDeliveryReceiptRequested  <br/> |||x  <br/> |||
|IsDraft  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsFromMe  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|IsMeeting  <br/> |x  <br/> |||||
|IsOnlineMeeting  <br/> |x  <br/> |||||
|IsRead  <br/> |||x  <br/> |||
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
|LastModifiedTime  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|LastOccurrance  <br/> |x  <br/> |||||
|LegacyFreeBusyStatus  <br/> |x  <br/> |||||
|Emplacement  <br/> |x  <br/> |||||
|Responsable  <br/> ||x  <br/> ||||
|MeetingRequestWasSent  <br/> |x  <br/> |||||
|MeetingTimeZone  <br/> |x  <br/> |||||
|MeetingWorkspaceUrl  <br/> |x  <br/> |||||
|MiddleName  <br/> ||x  <br/> ||||
|Mileage  <br/> ||x  <br/> |||x  <br/> |
|ModifiedOccurrances  <br/> |x  <br/> |||||
|MyResponseType  <br/> |x  <br/> |||||
|NetShowUrl  <br/> |x  <br/> |||||
|NickName  <br/> ||x  <br/> ||||
|Remarques  <br/> ||x  <br/> ||||
|OfficeLocation  <br/> ||x  <br/> ||||
|OptionalAttendees  <br/> |x  <br/> |||||
|Organisateur  <br/> |x  <br/> |||||
|OriginalStart  <br/> |x  <br/> |||||
|Propriétaire  <br/> |||||x  <br/> |
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
|ReceivedBy  <br/> |||x  <br/> |||
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
|Niveau de confidentialité  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|Size  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|SpouseName  <br/> ||x  <br/> ||||
|Début  <br/> |x  <br/> |||||
|StartDate  <br/> |||||x  <br/> |
|StartTimeZone  <br/> |x  <br/> |||||
|Statut  <br/> |||||x  <br/> |
|StatusDescription  <br/> |||||x  <br/> |
|Sujet  <br/> |x  <br/> |x  <br/> |x  <br/> ||x  <br/> |
|Surname  <br/> ||x  <br/> ||||
|TimeZone  <br/> |x  <br/> |||||
|ToRecipients  <br/> |||x  <br/> |||
|TotalWork  <br/> |||||x  <br/> |
|WebClientEditFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
|WebClientReadFormQueryString  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |x  <br/> |
   
Remarques :
  
1. Inclus lors [de la liaison à un élément](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) et dans la réponse de [l’opération GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx). Non inclus dans le résultat de la [méthode Item.FindItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou de la réponse de [l’opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).
    
## <a name="see-also"></a>Voir aussi

- [Développer des clients de service web pour Exchange](develop-web-service-clients-for-exchange.md)
    
- [Opération FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [Opération GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx)
    
- [Opération FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Opération GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)
    

