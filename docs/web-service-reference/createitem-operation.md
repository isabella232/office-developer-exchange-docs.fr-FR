---
title: CreateItem Operation
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
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: L’opération CreateItem crée des éléments dans la banque d’informations Exchange.
ms.openlocfilehash: 7e1808c685cdbaa1e8867aa7425b2cc52218d001
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755723"
---
# <a name="createitem-operation"></a><span data-ttu-id="b2063-103">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="b2063-103">CreateItem operation</span></span>

<span data-ttu-id="b2063-104">L’opération CreateItem crée des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2063-104">The CreateItem operation creates items in the Exchange store.</span></span>
  
## <a name="using-the-createitem-operation"></a><span data-ttu-id="b2063-105">Utilisation de l’opération CreateItem</span><span class="sxs-lookup"><span data-stu-id="b2063-105">Using the CreateItem Operation</span></span>

<span data-ttu-id="b2063-106">Vous pouvez utiliser l’opération CreateItem pour créer les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="b2063-106">You can use the CreateItem operation to create the following:</span></span>
  
- <span data-ttu-id="b2063-107">Éléments de calendrier</span><span class="sxs-lookup"><span data-stu-id="b2063-107">Calendar items</span></span>
    
- <span data-ttu-id="b2063-108">Messages électroniques</span><span class="sxs-lookup"><span data-stu-id="b2063-108">E-mail messages</span></span>
    
- <span data-ttu-id="b2063-109">Demandes de rendez-vous</span><span class="sxs-lookup"><span data-stu-id="b2063-109">Meeting requests</span></span>
    
- <span data-ttu-id="b2063-110">Tâches</span><span class="sxs-lookup"><span data-stu-id="b2063-110">Tasks</span></span>
    
- <span data-ttu-id="b2063-111">Contacts</span><span class="sxs-lookup"><span data-stu-id="b2063-111">Contacts</span></span>
    
<span data-ttu-id="b2063-112">Pour plus d’informations, voir [CreateItem operation (élément de calendrier)](createitem-operation-calendar-item.md), [opération CreateItem (e-mail)](createitem-operation-email-message.md), [opération CreateItem (demande de réunion)](createitem-operation-meeting-request.md), [opération CreateItem (tâche)](createitem-operation-task.md)et [opération CreateItem (contacts) ](createitem-operation-contact.md).</span><span class="sxs-lookup"><span data-stu-id="b2063-112">For more information, see [CreateItem operation (calendar item)](createitem-operation-calendar-item.md), [CreateItem operation (email message)](createitem-operation-email-message.md), [CreateItem operation (meeting request)](createitem-operation-meeting-request.md), [CreateItem operation (task)](createitem-operation-task.md), and [CreateItem operation (contact)](createitem-operation-contact.md).</span></span>
  
<span data-ttu-id="b2063-113">L’opération CreateItem prend en charge l’utilisation d’objets de réponse.</span><span class="sxs-lookup"><span data-stu-id="b2063-113">The CreateItem operation supports the use of response objects.</span></span> <span data-ttu-id="b2063-114">Objets de réponse prennent en charge l’acceptation et le rejet des réunions et la gestion des boutons de vote qui sont inclus dans un message électronique standard.</span><span class="sxs-lookup"><span data-stu-id="b2063-114">Response objects support the acceptance and rejection of meetings and the handling of voting buttons that are included in a standard e-mail message.</span></span> <span data-ttu-id="b2063-115">Le tableau suivant répertorie les objets de réponse qui sont gérées de l’opération CreateItem.</span><span class="sxs-lookup"><span data-stu-id="b2063-115">The following table lists the response objects that are handled in the CreateItem operation.</span></span>
  
|<span data-ttu-id="b2063-116">**Objet de réponse**</span><span class="sxs-lookup"><span data-stu-id="b2063-116">**Response object**</span></span>|<span data-ttu-id="b2063-117">**Action**</span><span class="sxs-lookup"><span data-stu-id="b2063-117">**Action**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b2063-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="b2063-118">AcceptItem</span></span>  <br/> |<span data-ttu-id="b2063-119">Accepter une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="b2063-119">Accept a meeting request.</span></span>  <br/> |
|<span data-ttu-id="b2063-120">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="b2063-120">CancelCalendarItem</span></span>  <br/> |<span data-ttu-id="b2063-121">Annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="b2063-121">Cancel a meeting.</span></span> <span data-ttu-id="b2063-122">Cela diffère de la suppression de tous les participants, car il supprime la réunion pour l’organisateur également.</span><span class="sxs-lookup"><span data-stu-id="b2063-122">This differs from deleting all attendees because it deletes the meeting for the organizer also.</span></span>  <br/> |
|<span data-ttu-id="b2063-123">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="b2063-123">DeclineItem</span></span>  <br/> |<span data-ttu-id="b2063-124">Refuser une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="b2063-124">Decline a meeting request.</span></span>  <br/> |
|<span data-ttu-id="b2063-125">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="b2063-125">ForwardItem</span></span>  <br/> |<span data-ttu-id="b2063-126">Envoyer une demande de réunion à une autre personne en tant qu’une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="b2063-126">Send a meeting request to another person as a meeting request.</span></span>  <br/> |
|<span data-ttu-id="b2063-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="b2063-127">RemoveItem</span></span>  <br/> |<span data-ttu-id="b2063-128">Supprimer une réunion annulée à partir du calendrier.</span><span class="sxs-lookup"><span data-stu-id="b2063-128">Remove a canceled meeting from the calendar.</span></span>  <br/> |
|<span data-ttu-id="b2063-129">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="b2063-129">ReplyAllToItem</span></span>  <br/> |<span data-ttu-id="b2063-130">Envoyer un message qui inclut le corps de la demande de réunion d’origine à tous les participants de la réunion.</span><span class="sxs-lookup"><span data-stu-id="b2063-130">Send a message that includes the body of the original meeting request to all attendees of the meeting.</span></span>  <br/> |
|<span data-ttu-id="b2063-131">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="b2063-131">ReplyToItem</span></span>  <br/> |<span data-ttu-id="b2063-132">Envoyer un message qui inclut le corps de la demande de réunion d’origine à l’expéditeur de la demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="b2063-132">Send a message that includes the body of the original meeting request to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="b2063-133">SendReadReceipt</span><span class="sxs-lookup"><span data-stu-id="b2063-133">SendReadReceipt</span></span>  <br/> |<span data-ttu-id="b2063-134">Envoyer une confirmation de lecture à l’expéditeur de la demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="b2063-134">Send a read receipt to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="b2063-135">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="b2063-135">TentativelyAcceptItem</span></span>  <br/> |<span data-ttu-id="b2063-136">Accepter provisoirement une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="b2063-136">Tentatively accept a meeting request.</span></span>  <br/> |
   
<span data-ttu-id="b2063-137">L’opération CreateItem prend également en charge les objets de la conférence supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="b2063-137">The CreateItem operation also supports additional meeting objects.</span></span> <span data-ttu-id="b2063-138">Le tableau suivant répertorie les objets supplémentaires que l’opération CreateItem prend en charge.</span><span class="sxs-lookup"><span data-stu-id="b2063-138">The following table lists additional objects that the CreateItem operation supports.</span></span>
  
|<span data-ttu-id="b2063-139">**Objet de la réunion**</span><span class="sxs-lookup"><span data-stu-id="b2063-139">**Meeting object**</span></span>|<span data-ttu-id="b2063-140">**Description**</span><span class="sxs-lookup"><span data-stu-id="b2063-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b2063-141">Message de réunion</span><span class="sxs-lookup"><span data-stu-id="b2063-141">Meeting Message</span></span>  <br/> |<span data-ttu-id="b2063-142">Représente un message de réunion dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2063-142">Represents a meeting message in the Exchange store.</span></span> <span data-ttu-id="b2063-143">Il s’agit de l’objet de base pour les autres objets de la réunion.</span><span class="sxs-lookup"><span data-stu-id="b2063-143">This is the base object for the other meeting objects.</span></span>  <br/> |
|<span data-ttu-id="b2063-144">Demande de réunion</span><span class="sxs-lookup"><span data-stu-id="b2063-144">Meeting Request</span></span>  <br/> |<span data-ttu-id="b2063-145">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2063-145">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="b2063-146">Réponse à une réunion</span><span class="sxs-lookup"><span data-stu-id="b2063-146">Meeting Response</span></span>  <br/> |<span data-ttu-id="b2063-147">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2063-147">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="b2063-148">Annulation de réunion</span><span class="sxs-lookup"><span data-stu-id="b2063-148">Meeting Cancellation</span></span>  <br/> |<span data-ttu-id="b2063-149">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2063-149">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2063-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b2063-150">See also</span></span>



[<span data-ttu-id="b2063-151">Opération CreateItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="b2063-151">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)
  
[<span data-ttu-id="b2063-152">Opération CreateItem (contacts)</span><span class="sxs-lookup"><span data-stu-id="b2063-152">CreateItem operation (contact)</span></span>](createitem-operation-contact.md)
  
[<span data-ttu-id="b2063-153">Opération CreateItem (e-mail)</span><span class="sxs-lookup"><span data-stu-id="b2063-153">CreateItem operation (email message)</span></span>](createitem-operation-email-message.md)
  
[<span data-ttu-id="b2063-154">Opération CreateItem (demande de réunion)</span><span class="sxs-lookup"><span data-stu-id="b2063-154">CreateItem operation (meeting request)</span></span>](createitem-operation-meeting-request.md)
  
[<span data-ttu-id="b2063-155">Opération CreateItem (tâche)</span><span class="sxs-lookup"><span data-stu-id="b2063-155">CreateItem operation (task)</span></span>](createitem-operation-task.md)
  
 <span data-ttu-id="b2063-156">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="b2063-156">**CreateItemType**</span></span>

