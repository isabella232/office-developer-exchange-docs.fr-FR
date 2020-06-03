---
title: Opération CreateItem (élément de calendrier)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: aa4a7c94-f668-4bd2-8079-c855f6ab17e1
description: L’opération CreateItem crée des éléments de calendrier dans la Banque d’Exchange.
ms.openlocfilehash: 535edf9fe567bc3063a5b853f01d604ea4c7eb95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457500"
---
# <a name="createitem-operation-calendar-item"></a>Opération CreateItem (élément de calendrier)

L’opération CreateItem crée des éléments de calendrier dans la Banque d’Exchange.
  
## <a name="remarks"></a>Remarques

L’opération CreateItem crée des rendez-vous, des réunions et des demandes de réunion. Si un élément de calendrier est créé sans participants, il est considéré comme un rendez-vous. Si les participants sont spécifiés, l’élément de calendrier est une réunion. Lorsqu’une réunion est créée à l’aide de l’opération CreateItem, les demandes de réunion sont automatiquement envoyées aux participants identifiés si l’attribut SendMeetingInvitations est défini pour envoyer les demandes de réunion.
  
## <a name="createitem-calendar-item-request-example"></a>Exemple de requête CreateItem (élément de calendrier)

### <a name="description"></a>Description

L’exemple de requête CreateItem suivant montre comment créer une réunion avec deux participants obligatoires. Cette demande enverra les demandes de réunion aux deux participants.
  
### <a name="code"></a>Code

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                SendMeetingInvitations="SendToAllAndSaveCopy" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar"/>
      </SavedItemFolderId>
      <Items>
        <t:CalendarItem xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Planning Meeting</Subject>
          <Body BodyType="Text">Plan the agenda for next week's meeting.</Body>
          <ReminderIsSet>true</ReminderIsSet>
          <ReminderMinutesBeforeStart>60</ReminderMinutesBeforeStart>
          <Start>2006-11-02T14:00:00</Start>
          <End>2006-11-02T15:00:00</End>
          <IsAllDayEvent>false</IsAllDayEvent>
          <LegacyFreeBusyStatus>Busy</LegacyFreeBusyStatus>
          <Location>Conference Room 721</Location>
          <RequiredAttendees>
            <Attendee>
              <Mailbox>
                <EmailAddress>User1@example.com</EmailAddress>
              </Mailbox>
            </Attendee>
            <Attendee>
              <Mailbox>
                <EmailAddress>User2@example.com</EmailAddress>
              </Mailbox>
            </Attendee>
          </RequiredAttendees>
        </t:CalendarItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Pour obtenir un exemple de réponse à une demande de réunion, consultez la rubrique [opération CreateItem (demande de réunion)](createitem-operation-meeting-request.md) . 
  
### <a name="request-elements"></a>Demander des éléments

Les éléments suivants sont utilisés dans la demande :
  
- [CreateItem](createitem.md)
    
- [SavedItemFolderId](saveditemfolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [CalendarItem](calendaritem.md)
    
- [Subject](subject.md)
    
- [Corps](body.md)
    
- [ReminderIsSet](reminderisset.md)
    
- [ReminderMinutesBeforeStart](reminderminutesbeforestart.md)
    
- [Démarrage](start.md)
    
- [Fin](end-ex15websvcsotherref.md)
    
- [IsAllDayEvent](isalldayevent.md)
    
- [LegacyFreeBusyStatus](legacyfreebusystatus.md)
    
- [Emplacement](location.md)
    
- [RequiredAttendees](requiredattendees.md)
    
- [Participant](attendee.md)
    
- [Boîte aux lettres](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
## <a name="successful-createitem-calendar-item-response"></a>Réponse CreateItem (élément de calendrier) réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à la demande CreateItem.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAAlAFV" ChangeKey="DwAAABYA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Les **attributs de l’élément** [ItemId](itemid.md) et **ChangeKey** ont été raccourcis pour conserver la lisibilité. 
  
### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
- [CalendarItem](calendaritem.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>Voir aussi



[CreateItem Operation](createitem-operation.md)

