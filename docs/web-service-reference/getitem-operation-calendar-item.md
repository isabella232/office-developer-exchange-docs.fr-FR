---
title: Opération de GetItem (élément de calendrier)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8
description: L’opération GetItem Obtient les éléments de calendrier à partir de la banque d’informations Exchange.
ms.openlocfilehash: 69bce0f0cc7b5c986f9bf4767c3cd429a309e50d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756646"
---
# <a name="getitem-operation-calendar-item"></a><span data-ttu-id="0dd0c-103">Opération de GetItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="0dd0c-103">GetItem operation (calendar item)</span></span>

<span data-ttu-id="0dd0c-104">L’opération GetItem Obtient les éléments de calendrier à partir de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-104">The GetItem operation gets calendar items from the Exchange store.</span></span>
  
## <a name="getitem-request-example"></a><span data-ttu-id="0dd0c-105">Exemple de requête GetItem</span><span class="sxs-lookup"><span data-stu-id="0dd0c-105">GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="0dd0c-106">Description</span><span class="sxs-lookup"><span data-stu-id="0dd0c-106">Description</span></span>

<span data-ttu-id="0dd0c-107">L’exemple suivant d’une demande de GetItem montre comment former une demande pour obtenir l’identité et l’objet d’un élément.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-107">The following example of a GetItem request shows how to form a request to get the identity and subject of an item.</span></span>
  
### <a name="code"></a><span data-ttu-id="0dd0c-108">Code</span><span class="sxs-lookup"><span data-stu-id="0dd0c-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AsdD89=" ChangeKey="Jajs3=="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="0dd0c-109">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="0dd0c-109">Request elements</span></span>

<span data-ttu-id="0dd0c-110">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="0dd0c-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="0dd0c-111">GetItem</span><span class="sxs-lookup"><span data-stu-id="0dd0c-111">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="0dd0c-112">ItemShape</span><span class="sxs-lookup"><span data-stu-id="0dd0c-112">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="0dd0c-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="0dd0c-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="0dd0c-114">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="0dd0c-114">AdditionalProperties</span></span>](additionalproperties.md)
    
- [<span data-ttu-id="0dd0c-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="0dd0c-115">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="0dd0c-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="0dd0c-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="0dd0c-117">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="0dd0c-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="0dd0c-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="0dd0c-119">Pour trouver d’autres options pour le message de demande de l’opération GetItem, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-119">To find other options for the request message of the GetItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="0dd0c-120">Commencer à l’élément [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="0dd0c-120">Start at the [GetItem](getitem.md) element.</span></span> 
  
## <a name="successful-getitem-response"></a><span data-ttu-id="0dd0c-121">Réponse GetItem réussie</span><span class="sxs-lookup"><span data-stu-id="0dd0c-121">Successful GetItem Response</span></span>

### <a name="description"></a><span data-ttu-id="0dd0c-122">Description</span><span class="sxs-lookup"><span data-stu-id="0dd0c-122">Description</span></span>

<span data-ttu-id="0dd0c-123">L’exemple suivant montre une réponse positive à la demande de GetItem.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-123">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="0dd0c-124">La demande ayant créé cette réponse utilisé le baseshape IdOnly.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-124">The request that created this response used the IdOnly baseshape.</span></span> <span data-ttu-id="0dd0c-125">Dans cet exemple, la réponse renvoie uniquement l’ID de l’élément.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-125">In this example, the response returns only the ID of the item.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0dd0c-126">L’ID d’élément et le symbole de modification ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-126">The item ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0dd0c-127">Code</span><span class="sxs-lookup"><span data-stu-id="0dd0c-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAd" ChangeKey="otlIqB=="/>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="description"></a><span data-ttu-id="0dd0c-128">Description</span><span class="sxs-lookup"><span data-stu-id="0dd0c-128">Description</span></span>

<span data-ttu-id="0dd0c-129">L’exemple suivant montre une réponse positive à la demande de GetItem.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-129">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="0dd0c-130">La demande ayant créé cette réponse utilisé le baseshape par défaut.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-130">The request that created this response used the Default baseshape.</span></span> <span data-ttu-id="0dd0c-131">Dans cet exemple, la réponse renvoie la forme par défaut pour un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-131">In this example, the response returns the Default shape for a calendar item.</span></span>
  
> [!NOTE]
> <span data-ttu-id="0dd0c-132">L’ID d’élément et le symbole de modification ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-132">The item ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0dd0c-133">Code</span><span class="sxs-lookup"><span data-stu-id="0dd0c-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAdTB" ChangeKey="otlIqBwrt=="/>
              <t:ResponseObjects>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:Start>2006-06-16T00:30:00Z</t:Start>
              <t:End>2006-06-16T01:00:00Z</t:End>
              <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
              <t:CalendarItemType>Single</t:CalendarItemType>
              <t:Organizer>
                <t:Mailbox>
                  <t:Name>Bob</t:Name>
                  <t:EmailAddress>someone@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:Organizer>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="description"></a><span data-ttu-id="0dd0c-134">Description</span><span class="sxs-lookup"><span data-stu-id="0dd0c-134">Description</span></span>

<span data-ttu-id="0dd0c-135">L’exemple suivant montre une réponse positive à la demande de GetItem.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-135">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="0dd0c-136">La demande ayant créé cette réponse utilisé le baseshape AllProperties.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-136">The request that created this response used the AllProperties baseshape.</span></span> <span data-ttu-id="0dd0c-137">Dans cet exemple, la réponse renvoie la forme de AllProperties pour un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-137">In this example, the response returns the AllProperties shape for a calendar item.</span></span>
  
### <a name="code"></a><span data-ttu-id="0dd0c-138">Code</span><span class="sxs-lookup"><span data-stu-id="0dd0c-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAdT" ChangeKey="otlIqB=="/>
              <t:ParentFolderId Id="ASUAdT=="/>
              <t:ItemClass>IPM.Appointment</t:ItemClass>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text"/>
              <t:DateTimeReceived>2006-06-16T00:12:41Z</t:DateTimeReceived>
              <t:Size>374</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>false</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-06-16T00:12:41Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-06-16T00:12:41Z</t:DateTimeCreated>
              <t:ResponseObjects>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:ReminderDueBy>2006-06-16T00:30:00Z</t:ReminderDueBy>
              <t:ReminderIsSet>true</t:ReminderIsSet>
              <t:ReminderMinutesBeforeStart>15</t:ReminderMinutesBeforeStart>
              <t:DisplayCc/>
              <t:DisplayTo/>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en-US</t:Culture>
              <t:Start>2006-06-16T00:30:00Z</t:Start>
              <t:End>2006-06-16T01:00:00Z</t:End>
              <t:IsAllDayEvent>false</t:IsAllDayEvent>
              <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
              <t:IsMeeting>false</t:IsMeeting>
              <t:IsCancelled>false</t:IsCancelled>
              <t:IsRecurring>false</t:IsRecurring>
              <t:MeetingRequestWasSent>false</t:MeetingRequestWasSent>
              <t:CalendarItemType>Single</t:CalendarItemType>
              <t:MyResponseType>Organizer</t:MyResponseType>
              <t:Organizer>
                <t:Mailbox>
                  <t:Name>Bob</t:Name>
                  <t:EmailAddress>someone@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:Organizer>
              <t:ConflictingMeetingCount>2</t:ConflictingMeetingCount>
              <t:AdjacentMeetingCount>0</t:AdjacentMeetingCount>
              <t:ConflictingMeetings>
                <t:CalendarItem>
                  <t:ItemId Id="ASUAdTB" ChangeKey="otlIqBwr=="/>
                  <t:Subject/>
                  <t:Start>2006-06-16T00:30:00Z</t:Start>
                  <t:End>2006-06-16T01:00:00Z</t:End>
                  <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
                  <t:Location/>
                </t:CalendarItem>
                <t:CalendarItem>
                  <t:ItemId Id="ASUAd" ChangeKey="otlIqBw=="/>
                  <t:Subject/>
                  <t:Start>2006-06-16T00:30:00Z</t:Start>
                  <t:End>2006-06-16T01:00:00Z</t:End>
                  <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
                  <t:Location/>
                </t:CalendarItem>
              </t:ConflictingMeetings>
              <t:Duration>PT30M</t:Duration>
              <t:TimeZone>Pacific Standard Time</t:TimeZone>
              <t:AppointmentSequenceNumber>0</t:AppointmentSequenceNumber>
              <t:AppointmentState>0</t:AppointmentState>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="0dd0c-139">Commentaires</span><span class="sxs-lookup"><span data-stu-id="0dd0c-139">Comments</span></span>

<span data-ttu-id="0dd0c-140">Pour trouver d’autres options pour le message de réponse de l’opération GetItem, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="0dd0c-140">To find other options for the response message of the GetItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="0dd0c-141">Démarrez au niveau de l’élément [GetItemResponse](getitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="0dd0c-141">Start at the [GetItemResponse](getitemresponse.md) element.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="0dd0c-142">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="0dd0c-142">Successful response elements</span></span>

<span data-ttu-id="0dd0c-143">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="0dd0c-143">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0dd0c-144">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0dd0c-144">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0dd0c-145">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="0dd0c-145">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="0dd0c-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0dd0c-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0dd0c-147">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0dd0c-147">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="0dd0c-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0dd0c-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0dd0c-149">Items</span><span class="sxs-lookup"><span data-stu-id="0dd0c-149">Items</span></span>](items.md)
    
- [<span data-ttu-id="0dd0c-150">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="0dd0c-150">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="0dd0c-151">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="0dd0c-151">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="0dd0c-152">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="0dd0c-152">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="0dd0c-153">ItemClass</span><span class="sxs-lookup"><span data-stu-id="0dd0c-153">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="0dd0c-154">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="0dd0c-154">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="0dd0c-155">Corps</span><span class="sxs-lookup"><span data-stu-id="0dd0c-155">Body</span></span>](body.md)
    
- [<span data-ttu-id="0dd0c-156">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="0dd0c-156">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="0dd0c-157">Taille</span><span class="sxs-lookup"><span data-stu-id="0dd0c-157">Size</span></span>](size.md)
    
- [<span data-ttu-id="0dd0c-158">Importance</span><span class="sxs-lookup"><span data-stu-id="0dd0c-158">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="0dd0c-159">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="0dd0c-159">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="0dd0c-160">IsDraft</span><span class="sxs-lookup"><span data-stu-id="0dd0c-160">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="0dd0c-161">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="0dd0c-161">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="0dd0c-162">IsResend</span><span class="sxs-lookup"><span data-stu-id="0dd0c-162">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="0dd0c-163">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="0dd0c-163">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="0dd0c-164">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="0dd0c-164">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="0dd0c-165">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="0dd0c-165">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="0dd0c-166">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="0dd0c-166">ResponseObjects</span></span>](responseobjects.md)
    
- [<span data-ttu-id="0dd0c-167">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="0dd0c-167">ForwardItem</span></span>](forwarditem.md)
    
- [<span data-ttu-id="0dd0c-168">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="0dd0c-168">ReminderDueBy</span></span>](reminderdueby.md)
    
- [<span data-ttu-id="0dd0c-169">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="0dd0c-169">ReminderIsSet</span></span>](reminderisset.md)
    
- [<span data-ttu-id="0dd0c-170">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="0dd0c-170">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md)
    
- [<span data-ttu-id="0dd0c-171">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="0dd0c-171">DisplayCc</span></span>](displaycc.md)
    
- [<span data-ttu-id="0dd0c-172">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="0dd0c-172">DisplayTo</span></span>](displayto.md)
    
- [<span data-ttu-id="0dd0c-173">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="0dd0c-173">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="0dd0c-174">Culture</span><span class="sxs-lookup"><span data-stu-id="0dd0c-174">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="0dd0c-175">Début</span><span class="sxs-lookup"><span data-stu-id="0dd0c-175">Start</span></span>](start.md)
    
- [<span data-ttu-id="0dd0c-176">Fin</span><span class="sxs-lookup"><span data-stu-id="0dd0c-176">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0dd0c-177">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="0dd0c-177">IsAllDayEvent</span></span>](isalldayevent.md)
    
- [<span data-ttu-id="0dd0c-178">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="0dd0c-178">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md)
    
- [<span data-ttu-id="0dd0c-179">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="0dd0c-179">IsMeeting</span></span>](ismeeting.md)
    
- [<span data-ttu-id="0dd0c-180">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="0dd0c-180">IsCancelled</span></span>](iscancelled.md)
    
- [<span data-ttu-id="0dd0c-181">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="0dd0c-181">IsRecurring</span></span>](isrecurring.md)
    
- [<span data-ttu-id="0dd0c-182">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="0dd0c-182">MeetingRequestWasSent</span></span>](meetingrequestwassent.md)
    
- [<span data-ttu-id="0dd0c-183">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="0dd0c-183">CalendarItemType</span></span>](calendaritemtype.md)
    
- [<span data-ttu-id="0dd0c-184">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="0dd0c-184">MyResponseType</span></span>](myresponsetype.md)
    
- [<span data-ttu-id="0dd0c-185">Bibliothèque multimédia</span><span class="sxs-lookup"><span data-stu-id="0dd0c-185">Organizer</span></span>](organizer.md)
    
- [<span data-ttu-id="0dd0c-186">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="0dd0c-186">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="0dd0c-187">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="0dd0c-187">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="0dd0c-188">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="0dd0c-188">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="0dd0c-189">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="0dd0c-189">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="0dd0c-190">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="0dd0c-190">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md)
    
- [<span data-ttu-id="0dd0c-191">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="0dd0c-191">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md)
    
- [<span data-ttu-id="0dd0c-192">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="0dd0c-192">ConflictingMeetings</span></span>](conflictingmeetings.md)
    
- [<span data-ttu-id="0dd0c-193">Location</span><span class="sxs-lookup"><span data-stu-id="0dd0c-193">Location</span></span>](location.md)
    
- [<span data-ttu-id="0dd0c-194">Durée (éléments)</span><span class="sxs-lookup"><span data-stu-id="0dd0c-194">Duration (Items)</span></span>](duration-items.md)
    
- [<span data-ttu-id="0dd0c-195">Fuseau horaire (élément)</span><span class="sxs-lookup"><span data-stu-id="0dd0c-195">TimeZone (Item)</span></span>](timezone-item.md)
    
- [<span data-ttu-id="0dd0c-196">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="0dd0c-196">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md)
    
- [<span data-ttu-id="0dd0c-197">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="0dd0c-197">AppointmentState</span></span>](appointmentstate.md)
    
## <a name="see-also"></a><span data-ttu-id="0dd0c-198">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0dd0c-198">See also</span></span>



[<span data-ttu-id="0dd0c-199">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="0dd0c-199">GetItem operation</span></span>](getitem-operation.md)

