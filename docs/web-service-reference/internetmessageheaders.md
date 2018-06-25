---
title: InternetMessageHeaders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeaders
api_type:
- schema
ms.assetid: 4dcf8671-96df-4a2d-9836-7e8e3a67e0db
description: L’élément InternetMessageHeaders contient une collection de certaines des en-têtes de message Internet qui sont contenus dans un élément dans une boîte aux lettres. Pour obtenir l’ensemble des en-têtes de message Internet, utilisez la propriété PR_TRANSPORT_MESSAGE_HEADERS. Pour plus d’informations sur EWS et en-têtes de message Internet, headersin de message Internet seeGetting EWS, MIME et les en-têtes de message Internet manquants.
ms.openlocfilehash: 2da529a8a3532cebb2791b285b7673c962a2a656
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827954"
---
# <a name="internetmessageheaders"></a><span data-ttu-id="4b68a-105">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="4b68a-105">InternetMessageHeaders</span></span>

<span data-ttu-id="4b68a-106">L’élément **InternetMessageHeaders** contient une collection de certaines des en-têtes de message Internet qui sont contenus dans un élément dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4b68a-106">The **InternetMessageHeaders** element contains a collection of some of the Internet message headers that are contained in an item in a mailbox.</span></span> <span data-ttu-id="4b68a-107">Pour obtenir l’ensemble des en-têtes de message Internet, utilisez la propriété **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="4b68a-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="4b68a-108">Pour plus d’informations à propos des en-têtes de message Internet et EWS, voir « En-têtes des messages Internet de mise en route » dans [EWS, MIME et les en-têtes de message Internet manquants](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="4b68a-108">For more information about EWS and Internet message headers, see "Getting Internet message headers" in [EWS, MIME, and the missing Internet message headers](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 <span data-ttu-id="4b68a-109">**NonEmptyArrayOfInternetHeadersType**</span><span class="sxs-lookup"><span data-stu-id="4b68a-109">**NonEmptyArrayOfInternetHeadersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b68a-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4b68a-110">Attributes and elements</span></span>

<span data-ttu-id="4b68a-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4b68a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b68a-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="4b68a-112">Attributes</span></span>

<span data-ttu-id="4b68a-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4b68a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b68a-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4b68a-114">Child elements</span></span>

|<span data-ttu-id="4b68a-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b68a-115">**Element**</span></span>|<span data-ttu-id="4b68a-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b68a-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b68a-117">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="4b68a-117">InternetMessageHeader</span></span>](internetmessageheader.md) <br/> |<span data-ttu-id="4b68a-118">Représente l’en-tête de message Internet pour un en-tête donné dans la collection d’en-têtes.</span><span class="sxs-lookup"><span data-stu-id="4b68a-118">Represents the Internet message header for a given header within the headers collection.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b68a-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4b68a-119">Parent elements</span></span>

|<span data-ttu-id="4b68a-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b68a-120">**Element**</span></span>|<span data-ttu-id="4b68a-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b68a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b68a-122">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="4b68a-122">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="4b68a-123">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="4b68a-123">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="4b68a-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="4b68a-125">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b68a-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-126">Contact</span><span class="sxs-lookup"><span data-stu-id="4b68a-126">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="4b68a-127">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b68a-127">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-128">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="4b68a-128">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="4b68a-129">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="4b68a-129">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-130">DistributionList</span><span class="sxs-lookup"><span data-stu-id="4b68a-130">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="4b68a-131">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="4b68a-131">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-132">Élément</span><span class="sxs-lookup"><span data-stu-id="4b68a-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="4b68a-133">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b68a-133">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="4b68a-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="4b68a-135">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b68a-135">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-136">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="4b68a-136">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="4b68a-137">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b68a-137">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-138">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="4b68a-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="4b68a-139">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b68a-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-140">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="4b68a-140">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="4b68a-141">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b68a-141">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-142">Message</span><span class="sxs-lookup"><span data-stu-id="4b68a-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4b68a-143">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b68a-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-144">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="4b68a-144">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="4b68a-145">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b68a-145">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-146">Tâche</span><span class="sxs-lookup"><span data-stu-id="4b68a-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="4b68a-147">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b68a-147">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4b68a-148">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="4b68a-148">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="4b68a-149">Représente la réponse à une demande de réunion acceptée provisoirement.</span><span class="sxs-lookup"><span data-stu-id="4b68a-149">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4b68a-150">Remarques</span><span class="sxs-lookup"><span data-stu-id="4b68a-150">Remarks</span></span>

<span data-ttu-id="4b68a-151">Vous trouverez ci-dessous l’API managée EWS étendu de définition de la propriété pour la propriété **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="4b68a-151">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="4b68a-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b68a-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b68a-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4b68a-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b68a-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4b68a-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4b68a-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4b68a-155">Schema Name</span></span>  <br/> |<span data-ttu-id="4b68a-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4b68a-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="4b68a-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4b68a-157">Validation File</span></span>  <br/> |<span data-ttu-id="4b68a-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4b68a-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4b68a-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4b68a-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b68a-160">False</span><span class="sxs-lookup"><span data-stu-id="4b68a-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b68a-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4b68a-161">See also</span></span>



- [<span data-ttu-id="4b68a-162">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b68a-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="4b68a-163">EWS, MIME et les en-têtes de message Internet manquants</span><span class="sxs-lookup"><span data-stu-id="4b68a-163">EWS, MIME, and the missing Internet message headers</span></span>](http://msdn.microsoft.com/en-us/library/exchange/hh545614%28v=exchg.140%29.aspx)

