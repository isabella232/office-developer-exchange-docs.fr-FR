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
description: L’opération CreateItem crée des éléments de calendrier dans la banque d’informations Exchange.
ms.openlocfilehash: c2174dd806b922e640ef7afcab32b98c67c65b41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755717"
---
# <a name="createitem-operation-calendar-item"></a><span data-ttu-id="00945-103">Opération CreateItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="00945-103">CreateItem operation (calendar item)</span></span>

<span data-ttu-id="00945-104">L’opération CreateItem crée des éléments de calendrier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="00945-104">The CreateItem operation creates calendar items in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00945-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="00945-105">Remarks</span></span>

<span data-ttu-id="00945-106">L’opération CreateItem crée des rendez-vous, réunions et des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="00945-106">The CreateItem operation creates appointments, meetings, and meeting requests.</span></span> <span data-ttu-id="00945-107">Si un élément de calendrier est créé sans participants, il est considéré comme un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="00945-107">If a calendar item is created without attendees, it is considered an appointment.</span></span> <span data-ttu-id="00945-108">Si les participants sont spécifiés, l’élément de calendrier est une réunion.</span><span class="sxs-lookup"><span data-stu-id="00945-108">If attendees are specified, the calendar item is a meeting.</span></span> <span data-ttu-id="00945-109">Lorsqu’une réunion est créée à l’aide de l’opération CreateItem, les demandes de réunion sont automatiquement envoyées aux participants identifiés si l’attribut SendMeetingInvitations est configuré pour envoyer les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="00945-109">When a meeting is created by using the CreateItem operation, meeting requests are automatically sent to the identified attendees if the SendMeetingInvitations attribute is set to send the meeting requests.</span></span>
  
## <a name="createitem-calendar-item-request-example"></a><span data-ttu-id="00945-110">Exemple de requête CreateItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="00945-110">CreateItem (Calendar Item) request example</span></span>

### <a name="description"></a><span data-ttu-id="00945-111">Description</span><span class="sxs-lookup"><span data-stu-id="00945-111">Description</span></span>

<span data-ttu-id="00945-112">Une demande CreateItem l’exemple suivant montre comment créer une réunion avec deux participants obligatoires.</span><span class="sxs-lookup"><span data-stu-id="00945-112">The following example of a CreateItem request shows how to create a meeting with two required attendees.</span></span> <span data-ttu-id="00945-113">Cette demande enverra les demandes de réunion pour les deux participants.</span><span class="sxs-lookup"><span data-stu-id="00945-113">This request will send the meeting requests to the two attendees.</span></span>
  
### <a name="code"></a><span data-ttu-id="00945-114">Code</span><span class="sxs-lookup"><span data-stu-id="00945-114">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                SendMeetingInvitations="SendToAllAndSaveCopy" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar"/>
      </SavedItemFolderId>
      <Items>
        <t:CalendarItem xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="00945-115">Commentaires</span><span class="sxs-lookup"><span data-stu-id="00945-115">Comments</span></span>

<span data-ttu-id="00945-116">Pour obtenir un exemple de la réponse à une demande de réunion, consultez la rubrique [opération CreateItem (demande de réunion)](createitem-operation-meeting-request.md) .</span><span class="sxs-lookup"><span data-stu-id="00945-116">For an example of how to respond to a meeting request, see the [CreateItem operation (meeting request)](createitem-operation-meeting-request.md) topic.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="00945-117">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="00945-117">Request elements</span></span>

<span data-ttu-id="00945-118">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="00945-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="00945-119">CreateItem</span><span class="sxs-lookup"><span data-stu-id="00945-119">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="00945-120">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="00945-120">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="00945-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="00945-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="00945-122">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="00945-122">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="00945-123">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="00945-123">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="00945-124">Objet</span><span class="sxs-lookup"><span data-stu-id="00945-124">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="00945-125">Corps</span><span class="sxs-lookup"><span data-stu-id="00945-125">Body</span></span>](body.md)
    
- [<span data-ttu-id="00945-126">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="00945-126">ReminderIsSet</span></span>](reminderisset.md)
    
- [<span data-ttu-id="00945-127">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="00945-127">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md)
    
- [<span data-ttu-id="00945-128">Début</span><span class="sxs-lookup"><span data-stu-id="00945-128">Start</span></span>](start.md)
    
- [<span data-ttu-id="00945-129">Fin</span><span class="sxs-lookup"><span data-stu-id="00945-129">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="00945-130">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="00945-130">IsAllDayEvent</span></span>](isalldayevent.md)
    
- [<span data-ttu-id="00945-131">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="00945-131">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md)
    
- [<span data-ttu-id="00945-132">Location</span><span class="sxs-lookup"><span data-stu-id="00945-132">Location</span></span>](location.md)
    
- [<span data-ttu-id="00945-133">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="00945-133">RequiredAttendees</span></span>](requiredattendees.md)
    
- [<span data-ttu-id="00945-134">Attendee</span><span class="sxs-lookup"><span data-stu-id="00945-134">Attendee</span></span>](attendee.md)
    
- [<span data-ttu-id="00945-135">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="00945-135">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="00945-136">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="00945-136">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-createitem-calendar-item-response"></a><span data-ttu-id="00945-137">Réponse CreateItem réussie (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="00945-137">Successful CreateItem (Calendar Item) Response</span></span>

### <a name="description"></a><span data-ttu-id="00945-138">Description</span><span class="sxs-lookup"><span data-stu-id="00945-138">Description</span></span>

<span data-ttu-id="00945-139">L’exemple suivant montre une réponse positive à la demande CreateItem.</span><span class="sxs-lookup"><span data-stu-id="00945-139">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="00945-140">Code</span><span class="sxs-lookup"><span data-stu-id="00945-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="00945-141">Commentaires</span><span class="sxs-lookup"><span data-stu-id="00945-141">Comments</span></span>

<span data-ttu-id="00945-142">Les attributs **Id** et **ChangeKey** d’élément [ItemId](itemid.md) ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="00945-142">The [ItemId](itemid.md) element **Id** and **ChangeKey** attributes have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="00945-143">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="00945-143">Successful response elements</span></span>

<span data-ttu-id="00945-144">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="00945-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="00945-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="00945-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="00945-146">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="00945-146">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="00945-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="00945-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="00945-148">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="00945-148">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="00945-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="00945-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="00945-150">Items</span><span class="sxs-lookup"><span data-stu-id="00945-150">Items</span></span>](items.md)
    
- [<span data-ttu-id="00945-151">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="00945-151">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="00945-152">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="00945-152">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="00945-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00945-153">See also</span></span>



[<span data-ttu-id="00945-154">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="00945-154">CreateItem operation</span></span>](createitem-operation.md)

