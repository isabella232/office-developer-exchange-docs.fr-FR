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
description: L’élément InternetMessageHeaders contient une collection de certains en-têtes de message Internet contenus dans un élément d’une boîte aux lettres. Pour obtenir la collection entière des en-têtes de message Internet, utilisez la propriété PR_TRANSPORT_MESSAGE_HEADERS. Pour plus d’informations sur EWS et les en-têtes de message Internet, obtention Internet Message headersin EWS, MIME et les en-têtes de message Internet manquants.
ms.openlocfilehash: 4719050c02590e021b29173c234466de3fdc58a4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467325"
---
# <a name="internetmessageheaders"></a><span data-ttu-id="546df-105">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="546df-105">InternetMessageHeaders</span></span>

<span data-ttu-id="546df-106">L’élément **InternetMessageHeaders** contient une collection de certains en-têtes de message Internet contenus dans un élément d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="546df-106">The **InternetMessageHeaders** element contains a collection of some of the Internet message headers that are contained in an item in a mailbox.</span></span> <span data-ttu-id="546df-107">Pour obtenir la collection entière des en-têtes de message Internet, utilisez la propriété **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="546df-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="546df-108">Pour plus d’informations sur EWS et les en-têtes de message Internet, consultez les rubriques « obtenir des en-têtes de message Internet » dans [EWS, MIME et les en-têtes de message Internet manquants](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="546df-108">For more information about EWS and Internet message headers, see "Getting Internet message headers" in [EWS, MIME, and the missing Internet message headers](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 <span data-ttu-id="546df-109">**NonEmptyArrayOfInternetHeadersType**</span><span class="sxs-lookup"><span data-stu-id="546df-109">**NonEmptyArrayOfInternetHeadersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="546df-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="546df-110">Attributes and elements</span></span>

<span data-ttu-id="546df-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="546df-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="546df-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="546df-112">Attributes</span></span>

<span data-ttu-id="546df-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="546df-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="546df-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="546df-114">Child elements</span></span>

|<span data-ttu-id="546df-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="546df-115">**Element**</span></span>|<span data-ttu-id="546df-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="546df-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="546df-117">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="546df-117">InternetMessageHeader</span></span>](internetmessageheader.md) <br/> |<span data-ttu-id="546df-118">Représente l’en-tête de message Internet d’un en-tête donné dans la collection headers.</span><span class="sxs-lookup"><span data-stu-id="546df-118">Represents the Internet message header for a given header within the headers collection.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="546df-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="546df-119">Parent elements</span></span>

|<span data-ttu-id="546df-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="546df-120">**Element**</span></span>|<span data-ttu-id="546df-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="546df-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="546df-122">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="546df-122">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="546df-123">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="546df-123">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="546df-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="546df-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="546df-125">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="546df-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="546df-126">Contact</span><span class="sxs-lookup"><span data-stu-id="546df-126">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="546df-127">Représente un élément de contact Exchange.</span><span class="sxs-lookup"><span data-stu-id="546df-127">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="546df-128">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="546df-128">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="546df-129">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="546df-129">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="546df-130">DistributionList</span><span class="sxs-lookup"><span data-stu-id="546df-130">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="546df-131">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="546df-131">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="546df-132">Élément</span><span class="sxs-lookup"><span data-stu-id="546df-132">Item</span></span>](item.md) <br/> |<span data-ttu-id="546df-133">Représente un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="546df-133">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="546df-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="546df-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="546df-135">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="546df-135">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="546df-136">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="546df-136">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="546df-137">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="546df-137">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="546df-138">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="546df-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="546df-139">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="546df-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="546df-140">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="546df-140">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="546df-141">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="546df-141">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="546df-142">Message</span><span class="sxs-lookup"><span data-stu-id="546df-142">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="546df-143">Représente un message électronique Exchange.</span><span class="sxs-lookup"><span data-stu-id="546df-143">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="546df-144">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="546df-144">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="546df-145">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="546df-145">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="546df-146">Tâche</span><span class="sxs-lookup"><span data-stu-id="546df-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="546df-147">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="546df-147">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="546df-148">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="546df-148">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="546df-149">Représente la réponse à une demande de réunion acceptée provisoirement.</span><span class="sxs-lookup"><span data-stu-id="546df-149">Represents a tentatively accepted reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="546df-150">Remarques</span><span class="sxs-lookup"><span data-stu-id="546df-150">Remarks</span></span>

<span data-ttu-id="546df-151">Voici la définition de la propriété étendue de l’API managée EWS pour la propriété **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="546df-151">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="546df-152">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="546df-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="546df-153">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="546df-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="546df-154">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="546df-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="546df-155">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="546df-155">Schema Name</span></span>  <br/> |<span data-ttu-id="546df-156">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="546df-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="546df-157">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="546df-157">Validation File</span></span>  <br/> |<span data-ttu-id="546df-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="546df-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="546df-159">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="546df-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="546df-160">False</span><span class="sxs-lookup"><span data-stu-id="546df-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="546df-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="546df-161">See also</span></span>



- [<span data-ttu-id="546df-162">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="546df-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="546df-163">EWS, MIME et les en-têtes de message Internet manquants</span><span class="sxs-lookup"><span data-stu-id="546df-163">EWS, MIME, and the missing Internet message headers</span></span>](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

