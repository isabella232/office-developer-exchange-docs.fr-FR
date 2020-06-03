---
title: Proposer une nouvelle heure de réunion à l'aide d’EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d5ac8e5b-3876-4f20-b4d3-44505e066042
description: Découvrez comment proposer de nouveaux horaires de réunion à partir de votre application cliente Exchange à l’aide d’EWS dans Exchange.
ms.openlocfilehash: 4f001bb82d2325624b567412620283619b51f25b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456809"
---
# <a name="propose-a-new-meeting-time-by-using-ews-in-exchange"></a><span data-ttu-id="dcc0b-103">Proposer une nouvelle heure de réunion à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dcc0b-103">Propose a new meeting time by using EWS in Exchange</span></span>

<span data-ttu-id="dcc0b-104">Découvrez comment proposer de nouveaux horaires de réunion à partir de votre application cliente Exchange à l’aide d’EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-104">Find out how to propose new meeting times from your Exchange client application by using EWS in Exchange.</span></span>
  
<span data-ttu-id="dcc0b-105">La fonctionnalité proposer une nouvelle heure permet aux participants de proposer de nouveaux horaires de réunion à l’organisateur de la réunion dans le cadre du flux de travail du calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-105">The propose new time feature enables attendees to propose new meeting times to the meeting organizer as part of the Exchange calendar workflow.</span></span> <span data-ttu-id="dcc0b-106">Lorsqu’un participant propose une nouvelle réunion, l’organisateur peut utiliser la nouvelle heure de réunion proposée pour mettre à jour la réunion et envoyer des mises à jour à tous les participants.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-106">When an attendee proposes a new meeting, the organizer can use the proposed new meeting time to update the meeting and send updates to all attendees.</span></span> <span data-ttu-id="dcc0b-107">Pour permettre aux participants de proposer de nouvelles heures de réunion, vous devez déterminer si l’organisateur autorise de nouvelles propositions de temps.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-107">Before you can enable attendees to propose new meeting times, you need to determine whether the organizer allows for new time proposals.</span></span> <span data-ttu-id="dcc0b-108">Cet article explique comment déterminer si vous pouvez proposer une nouvelle heure et comment utiliser EWS pour proposer une nouvelle heure.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-108">This article describes how to determine whether you can propose a new time and how to use EWS to propose a new time.</span></span>
  
> [!NOTE]
> <span data-ttu-id="dcc0b-109">L’API managée EWS n’implémente pas cette fonctionnalité.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-109">The EWS Managed API does not implement this functionality.</span></span> 
  
## <a name="determine-whether-you-can-propose-a-new-time-for-a-meeting-by-using-ews"></a><span data-ttu-id="dcc0b-110">Déterminer si vous pouvez proposer une nouvelle heure pour une réunion à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="dcc0b-110">Determine whether you can propose a new time for a meeting by using EWS</span></span>
<span data-ttu-id="dcc0b-111"><a name="bk_Determine"> </a></span><span class="sxs-lookup"><span data-stu-id="dcc0b-111"><a name="bk_Determine"> </a></span></span>

<span data-ttu-id="dcc0b-112">Pour pouvoir proposer une nouvelle heure pour une réunion, vous devez trouver une référence à cette réunion et déterminer si l’organisateur de la réunion a configuré la réunion pour prendre en charge de nouvelles propositions de temps.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-112">Before you can propose a new time for a meeting, you need to find a reference to that meeting and determine whether the meeting organizer configured the meeting to support new time proposals.</span></span> <span data-ttu-id="dcc0b-113">Vous pouvez obtenir une référence à une réunion en effectuant l’une des opérations suivantes :</span><span class="sxs-lookup"><span data-stu-id="dcc0b-113">You can get a reference to a meeting by doing either of the following:</span></span> 
  
- <span data-ttu-id="dcc0b-114">Recherche de la demande de réunion dans la boîte de réception</span><span class="sxs-lookup"><span data-stu-id="dcc0b-114">Finding the meeting request in the Inbox</span></span>
    
- <span data-ttu-id="dcc0b-115">Recherche du rendez-vous dans le calendrier</span><span class="sxs-lookup"><span data-stu-id="dcc0b-115">Finding the appointment in the calendar</span></span>
    
<span data-ttu-id="dcc0b-116">Pour rechercher une référence de réunion, procédez comme suit :</span><span class="sxs-lookup"><span data-stu-id="dcc0b-116">Use the following steps to find a meeting reference:</span></span>
  
1. <span data-ttu-id="dcc0b-117">Utilisez l’opération EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) (ou la méthode de l’API managée EWS de [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) ) pour rechercher la demande de réunion ou l’élément de calendrier cible.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-117">Use the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation (or the [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=EXCHG.80%29.aspx) EWS Managed API method) to find the target meeting request or calendar item.</span></span> <span data-ttu-id="dcc0b-118">Vous pouvez également utiliser l’opération EWS [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) pour obtenir l’identificateur de la demande de réunion ou de l’élément de calendrier cible.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-118">Alternatively, you can use the [SyncFolderItems](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) EWS operation to get the identifier of the target meeting request or calendar item.</span></span> 
    
2. <span data-ttu-id="dcc0b-119">Analysez les résultats de l’opération **FindItem** (ou de la méthode **Folder. FindItems** ) pour obtenir l’identificateur de l’élément de réunion.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-119">Parse the results of the **FindItem** operation (or **Folder.FindItems** method) to get the item identifier of the meeting item.</span></span> 
    
3. <span data-ttu-id="dcc0b-120">Utilisez l’opération EWS de [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) pour obtenir les objets de réponse pour la réunion.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-120">Use the [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS operation to get the response objects for the meeting.</span></span> 
    
<span data-ttu-id="dcc0b-121">Le code XML suivant montre ce qui est envoyé pour demander les objets de réponse sur un élément.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-121">The following XML shows what is sent to request the response objects on an item.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ResponseObjects"/>
          <t:FieldURI FieldURI="item:Subject"/>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="dcc0b-122">La réponse de l’opération **GetItem** doit ressembler au code XML suivant si vous demandez l’identificateur de l’élément, l’heure de début et de fin de la réunion, la collection d’objets de réponse et, si l’organisateur autorise les modifications proposées à l’heure de la réunion.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-122">The **GetItem** operation response will look similar to the following XML if you request the item identifier, the meeting start and end time, the response object collection, and if the organizer allows for proposed changes to the meeting time.</span></span> <span data-ttu-id="dcc0b-123">La collection d’objets Response, représentée par l’élément [ResponseObjects](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) , contient l’ensemble des réponses valides pour l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-123">The response object collection, which is represented by the [ResponseObjects](https://msdn.microsoft.com/library/ad29e064-3f3d-4b7b-aa4c-9ec27326381d%28Office.15%29.aspx) element, contains the set of responses that are valid for the calendar item.</span></span> <span data-ttu-id="dcc0b-124">L’élément **ProposeNewTime** est un objet de réponse qui indique que l’utilisateur peut proposer une nouvelle heure pour la réunion.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-124">The **ProposeNewTime** element is a response object that indicates that the user can propose a new time for the meeting.</span></span> <span data-ttu-id="dcc0b-125">Les éléments [AcceptItem](https://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx), [TentativelyAcceptItem](https://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx)et [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) représentent les objets de réponse que vous pouvez utiliser pour proposer une nouvelle heure de réunion à l’organisateur de la réunion.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-125">The [AcceptItem](https://msdn.microsoft.com/library/05a15431-77e1-411a-a16b-5481d364d3cc%28Office.15%29.aspx), [TentativelyAcceptItem](https://msdn.microsoft.com/library/ce6f50ef-ad8a-47e4-915a-487b2ef7a2e0%28Office.15%29.aspx), and [DeclineItem](https://msdn.microsoft.com/library/2d8d2389-924e-4d03-a324-35d56cf0d6b1%28Office.15%29.aspx) elements represent the response objects that you can use to propose a new meeting time to the meeting organizer.</span></span> 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
              <t:Subject>Competitive analysis: kick off meeting</t:Subject>
              <t:ResponseObjects>
                <t:AcceptItem/>
                <t:TentativelyAcceptItem/>
                <t:DeclineItem/>
                <t:ProposeNewTime/>
                <t:ReplyToItem/>
                <t:ReplyAllToItem/>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:Start>2013-11-09T17:00:00Z</t:Start>
              <t:End>2013-11-09T17:30:00Z</t:End>
            </t:MeetingRequest>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="propose-a-new-meeting-time-by-using-ews"></a><span data-ttu-id="dcc0b-126">Proposer une nouvelle heure de réunion à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="dcc0b-126">Propose a new meeting time by using EWS</span></span>
<span data-ttu-id="dcc0b-127"><a name="bk_Propose"> </a></span><span class="sxs-lookup"><span data-stu-id="dcc0b-127"><a name="bk_Propose"> </a></span></span>

<span data-ttu-id="dcc0b-128">Si vous avez reçu un objet de réponse **ProposeNewTime** lors de l’utilisation de l’opération **GetItem** pour obtenir un élément de calendrier ou une demande de réunion, vous pouvez répondre avec une nouvelle heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-128">If you received a **ProposeNewTime** response object when you used the **GetItem** operation to get a calendar item or meeting request, you can respond with a proposed new meeting time.</span></span> <span data-ttu-id="dcc0b-129">Si vous n’avez pas reçu d’objet de réponse **ProposeNewTime** , vous ne pourrez pas proposer une nouvelle heure de réunion dans le cadre du flux de travail du calendrier.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-129">If you didn't receive a **ProposeNewTime** response object, you won't be able to propose a new meeting time as part of the calendar workflow.</span></span> <span data-ttu-id="dcc0b-130">Toutefois, vous pouvez répondre à l’organisateur pour demander une nouvelle heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-130">You can, however, reply to the organizer to request a new meeting time.</span></span> <span data-ttu-id="dcc0b-131">Si vous recevez un objet de réponse **ProposeNewTime** , vous pouvez répondre à la réunion en référençant son identificateur et proposer une nouvelle heure de réunion à l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-131">If you receive a **ProposeNewTime** response object, you can respond to the meeting by referencing its identifier, and propose a new meeting time to the organizer.</span></span> <span data-ttu-id="dcc0b-132">C’est là où l’objet de réponse **ProposeNewTime** est différent du modèle d’objet réponse classique dans la mesure où vous ne répondez pas à un objet Response **ProposeNewTime** .</span><span class="sxs-lookup"><span data-stu-id="dcc0b-132">This is where the **ProposeNewTime** response object is different than the typical response object pattern in that you don't respond with a **ProposeNewTime** response object.</span></span> <span data-ttu-id="dcc0b-133">Vous utilisez l’un des autres objets de réponse à la réunion, tels que **AcceptItem**, **TentativelyAcceptItem**ou **DeclineItem**, pour proposer une nouvelle réunion.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-133">You use one of the other meeting response objects, such as **AcceptItem**, **TentativelyAcceptItem**, or **DeclineItem**, to propose a new meeting.</span></span> <span data-ttu-id="dcc0b-134">Cet exemple utilise l’objet Response **AcceptItem** .</span><span class="sxs-lookup"><span data-stu-id="dcc0b-134">This example uses the **AcceptItem** response object.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013"/>
  </soap:Header>
  <soap:Body>
    <m:CreateItem>
      <m:Items>
        <t:AcceptItem>
          <t:Body BodyType="Text">This time works better for the HiPPO.</t:Body>
          <t:ReferenceItemId Id="AAMkADEzOTExYjJkL1AAA=" ChangeKey="CwAAAB/G6X"/>
          <t:ProposedStart>2013-11-28T04:00:00Z</t:ProposedStart>
          <t:ProposedEnd>2013-11-28T04:30:00Z</t:ProposedEnd>
        </t:AcceptItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="dcc0b-135">La réponse à cette demande contient l’identificateur de l’élément de calendrier qui a été ajouté au calendrier du participant et une copie de la demande de réunion qui a été placée dans le dossier éléments supprimés du participant.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-135">The response to this request contains the identifier of the calendar item that was added to the attendee's calendar and a copy of the meeting request that was placed in the attendee's Deleted Items folder.</span></span> <span data-ttu-id="dcc0b-136">Le message de réponse avec la nouvelle proposition d’heure a également été enregistré dans le dossier éléments envoyés du participant (vous devrez trouver le message de réponse à la réunion pour obtenir un descripteur).</span><span class="sxs-lookup"><span data-stu-id="dcc0b-136">The response message with the new time proposal was also saved in the attendee's Sent Items folder (you will need to find the meeting response message to get a handle on it).</span></span>
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkAGRmOWE2OWAAA=" ChangeKey="DwAAJsmU"/>
            </t:CalendarItem>
            <t:MeetingRequest>
              <t:ItemId Id="AAMkAGRmOWE2AAABB=" ChangeKey="AAAGJu1A"/>
            </t:MeetingRequest>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="dcc0b-137">L’organisateur reçoit un message [MeetingResponse](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) lorsque le participant répond avec une nouvelle heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-137">The organizer will receive a [MeetingResponse](https://msdn.microsoft.com/library/9f798e79-dafd-4d4d-9967-95fd8e5c0502%28Office.15%29.aspx) message when the attendee responds with a proposed new meeting time.</span></span> <span data-ttu-id="dcc0b-138">Le message **MeetingResponse** contient l’heure de début et l’heure de fin de la réunion proposée, ainsi que l’identificateur de l’élément de calendrier associé dans le calendrier de l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-138">The **MeetingResponse** message contains the proposed new meeting start time and end time, and the identifier of the associated calendar item in the organizer's calendar.</span></span> <span data-ttu-id="dcc0b-139">L’organisateur peut utiliser ces informations pour mettre à jour son élément de calendrier existant pour la réunion.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-139">The organizer can use that information to update their existing calendar item for the meeting.</span></span> <span data-ttu-id="dcc0b-140">Voici le flux de travail pour que l’organisateur réponde à un message **MeetingResponse** qui propose une nouvelle heure de réunion :</span><span class="sxs-lookup"><span data-stu-id="dcc0b-140">The following is the workflow for the organizer to respond to a **MeetingResponse** message that proposes a new meeting time:</span></span> 
  
1. <span data-ttu-id="dcc0b-141">Déterminez si les éléments **ProposedStart** ou **ProposedEnd** ont été définis dans le **MeetingResponse**.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-141">Determine whether the **ProposedStart** or **ProposedEnd** elements have been set in the **MeetingResponse**.</span></span> <span data-ttu-id="dcc0b-142">Si c’est le cas, passez à l’étape 2.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-142">If so, go to step 2.</span></span> <span data-ttu-id="dcc0b-143">Si ce n’est pas le cas, le message **MeetingResponse** indique uniquement si le participant a accepté, accepté provisoirement ou refusé la réunion.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-143">If not, the **MeetingResponse** message only indicates whether the attendee has accepted, tentatively accepted, or declined the meeting.</span></span> 
    
2. <span data-ttu-id="dcc0b-144">Obtenir l’élément de calendrier existant de l’organisateur de la réunion à l’aide de l’identificateur EWS renvoyé dans l’élément **AssociatedCalendarItemId** .</span><span class="sxs-lookup"><span data-stu-id="dcc0b-144">Get the organizer's existing calendar item for the meeting by using the EWS identifier returned in the **AssociatedCalendarItemId** element.</span></span> 
    
3. <span data-ttu-id="dcc0b-145">Comparez l’heure de début et de fin d’origine à la nouvelle heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-145">Compare the original start and end time with the proposed new meeting time.</span></span> <span data-ttu-id="dcc0b-146">Si la nouvelle heure de réunion proposée est acceptable pour l’organisateur, passez à l’étape 4.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-146">If the proposed new meeting time is acceptable to the organizer, go to step 4.</span></span> <span data-ttu-id="dcc0b-147">Dans le cas contraire, l’organisateur de la réunion peut ignorer l’heure de la réunion proposée ou envoyer une réponse par courrier électronique au participant qui a proposé la nouvelle heure de la réunion.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-147">Otherwise, the meeting organizer can either ignore the proposed meeting time, or send an email response to the attendee that proposed the new meeting time.</span></span>
    
4. <span data-ttu-id="dcc0b-148">Module Effectuez un appel de l’opération EWS [GetUserAvailability](https://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) pour déterminer si le temps proposé est suffisant pour tous les participants, y compris les boîtes aux lettres de salle et de ressource.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-148">(Optional) Perform a [GetUserAvailability](https://msdn.microsoft.com/library/8da17226-5d3a-4525-9ffa-d83730f47bb1%28Office.15%29.aspx) EWS operation call to find out whether the proposed time will work for all attendees, including room and resource mailboxes.</span></span> <span data-ttu-id="dcc0b-149">(Vous pouvez également utiliser la méthode de l’API managée EWS [ExchangeService. GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) pour effectuer cette opération.)</span><span class="sxs-lookup"><span data-stu-id="dcc0b-149">(You can also use the [ExchangeService.GetUserAvailability](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getuseravailability%28v=exchg.80%29.aspx) EWS Managed API method to do this.)</span></span> 
    
5. <span data-ttu-id="dcc0b-150">L’organisateur peut ensuite mettre à jour sa réunion avec les nouvelles heures de réunion proposées et envoyer les mises à jour à tous les participants à l’aide de l’opération EWS [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) (ou du [rendez-vous. mettre à jour](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) la méthode de l’API managée EWS).</span><span class="sxs-lookup"><span data-stu-id="dcc0b-150">The organizer can then update their meeting with the new proposed meeting times and send the updates to all attendees by using the [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) EWS operation (or the [Appointment.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) EWS Managed API method).</span></span> 
    
<span data-ttu-id="dcc0b-151">La figure suivante illustre le processus qui se produit entre l’organisateur de la réunion, le participant et le serveur Exchange qui a géré les appels EWS.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-151">The following figure shows the process that occurs between the meeting organizer, the attendee, and the Exchange server that handled the EWS calls.</span></span>
  
<span data-ttu-id="dcc0b-152">**Figure 1. Processus de proposition d’une nouvelle heure de réunion**</span><span class="sxs-lookup"><span data-stu-id="dcc0b-152">**Figure 1. Process for proposing a new meeting time**</span></span>

![La figure illustre le flux de travail entre l’organisateur, Exchange et un participant lorsqu’un nouvel horaire de réunion est proposé. Si l’organisateur autorise de nouvelles propositions de réunion, un participant peut proposer un nouvel horaire de réunion avec un objet de réponse.](media/Ex_ProposeNewMeetingTime.png)
  
## <a name="version-differences"></a><span data-ttu-id="dcc0b-155">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="dcc0b-155">Version differences</span></span>
<span data-ttu-id="dcc0b-156"><a name="bk_Behavior"> </a></span><span class="sxs-lookup"><span data-stu-id="dcc0b-156"><a name="bk_Behavior"> </a></span></span>

<span data-ttu-id="dcc0b-157">La fonctionnalité proposer une nouvelle heure a été introduite dans la version d’Exchange Build 15.00.0800.007.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-157">The propose new time feature was introduced in Exchange build version 15.00.0800.007.</span></span> <span data-ttu-id="dcc0b-158">Dans les versions antérieures d’Exchange, les utilisateurs d’applications EWS doivent envoyer un message électronique distinct à l’organisateur de la réunion pour demander une autre heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="dcc0b-158">In earlier versions of Exchange, EWS application users have to send a separate email to the meeting organizer to request a different meeting time.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="dcc0b-159">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dcc0b-159">See also</span></span>


- [<span data-ttu-id="dcc0b-160">Calendriers et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dcc0b-160">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="dcc0b-161">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="dcc0b-161">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [<span data-ttu-id="dcc0b-162">Créer des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dcc0b-162">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="dcc0b-163">Mettre à jour des rendez-vous et des réunions à l’aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dcc0b-163">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="dcc0b-164">Supprimer des rendez-vous et annuler des réunions à l'aide d’EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dcc0b-164">Delete appointments and cancel meetings by using EWS in Exchange</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

