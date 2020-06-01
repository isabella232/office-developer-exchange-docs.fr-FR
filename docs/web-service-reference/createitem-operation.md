---
title: Opération CreateItem
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
description: L’opération CreateItem crée des éléments dans la Banque d’Exchange.
ms.openlocfilehash: f6aaa9ed8e8257f19780492d6137fb015c1b6136
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458865"
---
# <a name="createitem-operation"></a><span data-ttu-id="4e749-103">Opération CreateItem</span><span class="sxs-lookup"><span data-stu-id="4e749-103">CreateItem operation</span></span>

<span data-ttu-id="4e749-104">L’opération CreateItem crée des éléments dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e749-104">The CreateItem operation creates items in the Exchange store.</span></span>
  
## <a name="using-the-createitem-operation"></a><span data-ttu-id="4e749-105">Utilisation de l’opération CreateItem</span><span class="sxs-lookup"><span data-stu-id="4e749-105">Using the CreateItem Operation</span></span>

<span data-ttu-id="4e749-106">Vous pouvez utiliser l’opération CreateItem pour créer les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="4e749-106">You can use the CreateItem operation to create the following:</span></span>
  
- <span data-ttu-id="4e749-107">Éléments de calendrier</span><span class="sxs-lookup"><span data-stu-id="4e749-107">Calendar items</span></span>
    
- <span data-ttu-id="4e749-108">Messages électroniques</span><span class="sxs-lookup"><span data-stu-id="4e749-108">E-mail messages</span></span>
    
- <span data-ttu-id="4e749-109">Demandes de réunion</span><span class="sxs-lookup"><span data-stu-id="4e749-109">Meeting requests</span></span>
    
- <span data-ttu-id="4e749-110">Tâches</span><span class="sxs-lookup"><span data-stu-id="4e749-110">Tasks</span></span>
    
- <span data-ttu-id="4e749-111">Contacts</span><span class="sxs-lookup"><span data-stu-id="4e749-111">Contacts</span></span>
    
<span data-ttu-id="4e749-112">Pour plus d’informations, consultez opération [CreateItem (élément de calendrier)](createitem-operation-calendar-item.md), [opération CreateItem (message électronique)](createitem-operation-email-message.md), [opération CreateItem (demande de réunion)](createitem-operation-meeting-request.md), [opération CreateItem (tâche)](createitem-operation-task.md)et [opération CreateItem (contact)](createitem-operation-contact.md).</span><span class="sxs-lookup"><span data-stu-id="4e749-112">For more information, see [CreateItem operation (calendar item)](createitem-operation-calendar-item.md), [CreateItem operation (email message)](createitem-operation-email-message.md), [CreateItem operation (meeting request)](createitem-operation-meeting-request.md), [CreateItem operation (task)](createitem-operation-task.md), and [CreateItem operation (contact)](createitem-operation-contact.md).</span></span>
  
<span data-ttu-id="4e749-113">L’opération CreateItem prend en charge l’utilisation des objets Response.</span><span class="sxs-lookup"><span data-stu-id="4e749-113">The CreateItem operation supports the use of response objects.</span></span> <span data-ttu-id="4e749-114">Les objets Response prennent en charge l’acceptation et le rejet des réunions et la gestion des boutons de vote inclus dans un message électronique standard.</span><span class="sxs-lookup"><span data-stu-id="4e749-114">Response objects support the acceptance and rejection of meetings and the handling of voting buttons that are included in a standard e-mail message.</span></span> <span data-ttu-id="4e749-115">Le tableau suivant répertorie les objets Response qui sont gérés dans l’opération CreateItem.</span><span class="sxs-lookup"><span data-stu-id="4e749-115">The following table lists the response objects that are handled in the CreateItem operation.</span></span>
  
|<span data-ttu-id="4e749-116">**Response, objet**</span><span class="sxs-lookup"><span data-stu-id="4e749-116">**Response object**</span></span>|<span data-ttu-id="4e749-117">**Action**</span><span class="sxs-lookup"><span data-stu-id="4e749-117">**Action**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4e749-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="4e749-118">AcceptItem</span></span>  <br/> |<span data-ttu-id="4e749-119">Accepter une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="4e749-119">Accept a meeting request.</span></span>  <br/> |
|<span data-ttu-id="4e749-120">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="4e749-120">CancelCalendarItem</span></span>  <br/> |<span data-ttu-id="4e749-121">Annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="4e749-121">Cancel a meeting.</span></span> <span data-ttu-id="4e749-122">Cela diffère de la suppression de tous les participants, car elle supprime également la réunion pour l’organisateur.</span><span class="sxs-lookup"><span data-stu-id="4e749-122">This differs from deleting all attendees because it deletes the meeting for the organizer also.</span></span>  <br/> |
|<span data-ttu-id="4e749-123">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="4e749-123">DeclineItem</span></span>  <br/> |<span data-ttu-id="4e749-124">Refuser une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="4e749-124">Decline a meeting request.</span></span>  <br/> |
|<span data-ttu-id="4e749-125">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="4e749-125">ForwardItem</span></span>  <br/> |<span data-ttu-id="4e749-126">Envoyer une demande de réunion à une autre personne sous la forme d’une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="4e749-126">Send a meeting request to another person as a meeting request.</span></span>  <br/> |
|<span data-ttu-id="4e749-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="4e749-127">RemoveItem</span></span>  <br/> |<span data-ttu-id="4e749-128">Supprimer une réunion annulée du calendrier.</span><span class="sxs-lookup"><span data-stu-id="4e749-128">Remove a canceled meeting from the calendar.</span></span>  <br/> |
|<span data-ttu-id="4e749-129">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="4e749-129">ReplyAllToItem</span></span>  <br/> |<span data-ttu-id="4e749-130">Envoyer un message qui inclut le corps de la demande de réunion d’origine à tous les participants de la réunion.</span><span class="sxs-lookup"><span data-stu-id="4e749-130">Send a message that includes the body of the original meeting request to all attendees of the meeting.</span></span>  <br/> |
|<span data-ttu-id="4e749-131">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="4e749-131">ReplyToItem</span></span>  <br/> |<span data-ttu-id="4e749-132">Envoyez un message qui inclut le corps de la demande de réunion d’origine à l’expéditeur de la demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="4e749-132">Send a message that includes the body of the original meeting request to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="4e749-133">SendReadReceipt</span><span class="sxs-lookup"><span data-stu-id="4e749-133">SendReadReceipt</span></span>  <br/> |<span data-ttu-id="4e749-134">Envoyer une confirmation de lecture à l’expéditeur de la demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="4e749-134">Send a read receipt to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="4e749-135">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="4e749-135">TentativelyAcceptItem</span></span>  <br/> |<span data-ttu-id="4e749-136">Accepter provisoirement une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="4e749-136">Tentatively accept a meeting request.</span></span>  <br/> |
   
<span data-ttu-id="4e749-137">L’opération CreateItem prend également en charge des objets de réunion supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="4e749-137">The CreateItem operation also supports additional meeting objects.</span></span> <span data-ttu-id="4e749-138">Le tableau suivant répertorie les objets supplémentaires pris en charge par l’opération CreateItem.</span><span class="sxs-lookup"><span data-stu-id="4e749-138">The following table lists additional objects that the CreateItem operation supports.</span></span>
  
|<span data-ttu-id="4e749-139">**Objet de réunion**</span><span class="sxs-lookup"><span data-stu-id="4e749-139">**Meeting object**</span></span>|<span data-ttu-id="4e749-140">**Description**</span><span class="sxs-lookup"><span data-stu-id="4e749-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4e749-141">Message de réunion</span><span class="sxs-lookup"><span data-stu-id="4e749-141">Meeting Message</span></span>  <br/> |<span data-ttu-id="4e749-142">Représente un message de réunion dans la Banque d’aide Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e749-142">Represents a meeting message in the Exchange store.</span></span> <span data-ttu-id="4e749-143">Il s’agit de l’objet de base pour les autres objets de réunion.</span><span class="sxs-lookup"><span data-stu-id="4e749-143">This is the base object for the other meeting objects.</span></span>  <br/> |
|<span data-ttu-id="4e749-144">Demande de réunion</span><span class="sxs-lookup"><span data-stu-id="4e749-144">Meeting Request</span></span>  <br/> |<span data-ttu-id="4e749-145">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e749-145">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="4e749-146">Réponse à une réunion</span><span class="sxs-lookup"><span data-stu-id="4e749-146">Meeting Response</span></span>  <br/> |<span data-ttu-id="4e749-147">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e749-147">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="4e749-148">Annulation de réunion</span><span class="sxs-lookup"><span data-stu-id="4e749-148">Meeting Cancellation</span></span>  <br/> |<span data-ttu-id="4e749-149">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e749-149">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e749-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4e749-150">See also</span></span>



[<span data-ttu-id="4e749-151">Opération CreateItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="4e749-151">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)
  
[<span data-ttu-id="4e749-152">Opération CreateItem (contact)</span><span class="sxs-lookup"><span data-stu-id="4e749-152">CreateItem operation (contact)</span></span>](createitem-operation-contact.md)
  
[<span data-ttu-id="4e749-153">Opération CreateItem (message électronique)</span><span class="sxs-lookup"><span data-stu-id="4e749-153">CreateItem operation (email message)</span></span>](createitem-operation-email-message.md)
  
[<span data-ttu-id="4e749-154">Opération CreateItem (demande de réunion)</span><span class="sxs-lookup"><span data-stu-id="4e749-154">CreateItem operation (meeting request)</span></span>](createitem-operation-meeting-request.md)
  
[<span data-ttu-id="4e749-155">Opération CreateItem (tâche)</span><span class="sxs-lookup"><span data-stu-id="4e749-155">CreateItem operation (task)</span></span>](createitem-operation-task.md)
  
 <span data-ttu-id="4e749-156">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="4e749-156">**CreateItemType**</span></span>

