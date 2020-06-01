---
title: ParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 258f4b1f-367e-4c7d-9c29-eb775a2398c7
description: L’élément ParentFolderId représente l’identificateur du dossier parent qui contient l’élément ou le dossier.
ms.openlocfilehash: 3bad638aa21019472df8f487f1e065d2e725e750
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465750"
---
# <a name="parentfolderid"></a><span data-ttu-id="d2088-103">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d2088-103">ParentFolderId</span></span>

<span data-ttu-id="d2088-104">L’élément **ParentFolderId** représente l’identificateur du dossier parent qui contient l’élément ou le dossier.</span><span class="sxs-lookup"><span data-stu-id="d2088-104">The **ParentFolderId** element represents the identifier of the parent folder that contains the item or folder.</span></span> 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

<span data-ttu-id="d2088-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="d2088-105">**FolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d2088-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d2088-106">Attributes and elements</span></span>

<span data-ttu-id="d2088-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d2088-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2088-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d2088-108">Attributes</span></span>

|<span data-ttu-id="d2088-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d2088-109">**Attribute**</span></span>|<span data-ttu-id="d2088-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2088-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2088-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="d2088-111">**Id**</span></span> <br/> |<span data-ttu-id="d2088-112">Contient une chaîne qui identifie un dossier dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2088-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="d2088-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="d2088-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d2088-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="d2088-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="d2088-115">Contient une chaîne qui identifie la version d’un dossier identifiée par l’attribut **ID** .</span><span class="sxs-lookup"><span data-stu-id="d2088-115">Contains a string that identifies a version of a folder that is identified by the **Id** attribute.</span></span> <span data-ttu-id="d2088-116">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d2088-116">This attribute is optional.</span></span> <span data-ttu-id="d2088-117">Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.</span><span class="sxs-lookup"><span data-stu-id="d2088-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d2088-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d2088-118">Child elements</span></span>

<span data-ttu-id="d2088-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d2088-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d2088-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d2088-120">Parent elements</span></span>

|<span data-ttu-id="d2088-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d2088-121">**Element**</span></span>|<span data-ttu-id="d2088-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2088-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2088-123">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="d2088-123">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="d2088-124">Représente un dossier de calendrier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-124">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d2088-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d2088-126">Représente un élément de calendrier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-126">Represents a calendar item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-127">Contact</span><span class="sxs-lookup"><span data-stu-id="d2088-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="d2088-128">Représente un élément de contact dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-128">Represents a contact item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-129">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="d2088-129">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="d2088-130">Représente un dossier de contacts dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-130">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-131">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="d2088-131">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="d2088-132">Représente un événement dans lequel un élément ou un dossier est copié.</span><span class="sxs-lookup"><span data-stu-id="d2088-132">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="d2088-133">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="d2088-133">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="d2088-134">Représente un événement dans lequel un élément ou un dossier est créé.</span><span class="sxs-lookup"><span data-stu-id="d2088-134">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="d2088-135">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="d2088-135">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="d2088-136">Représente un événement dans lequel un élément ou un dossier est supprimé.</span><span class="sxs-lookup"><span data-stu-id="d2088-136">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="d2088-137">DistributionList</span><span class="sxs-lookup"><span data-stu-id="d2088-137">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="d2088-138">Représente une liste de distribution privée dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-138">Represents a private distribution list in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-139">Folder</span><span class="sxs-lookup"><span data-stu-id="d2088-139">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="d2088-140">Représente un dossier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-140">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-141">Élément</span><span class="sxs-lookup"><span data-stu-id="d2088-141">Item</span></span>](item.md) <br/> |<span data-ttu-id="d2088-142">Représente un élément Exchange générique.</span><span class="sxs-lookup"><span data-stu-id="d2088-142">Represents a generic Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="d2088-143">Élément (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="d2088-143">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="d2088-144">Représente un élément unique à télécharger dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-144">Represents a single item to upload into a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-145">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="d2088-145">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="d2088-146">Représente une annulation de réunion dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-146">Represents a meeting cancellation in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-147">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="d2088-147">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="d2088-148">Représente un message de réunion dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-148">Represents a meeting message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-149">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="d2088-149">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d2088-150">Représente une demande de réunion dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-150">Represents a meeting request in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-151">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="d2088-151">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="d2088-152">Représente une réponse à une réunion dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-152">Represents a meeting response in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-153">Message</span><span class="sxs-lookup"><span data-stu-id="d2088-153">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d2088-154">Représente un message électronique dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-154">Represents an e-mail message in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-155">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="d2088-155">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="d2088-156">Représente un événement dans lequel un élément ou un dossier est modifié.</span><span class="sxs-lookup"><span data-stu-id="d2088-156">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="d2088-157">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="d2088-157">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="d2088-158">Représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent vers un autre dossier parent.</span><span class="sxs-lookup"><span data-stu-id="d2088-158">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="d2088-159">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="d2088-159">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="d2088-160">Représente un événement qui est déclenché par un nouvel élément de courrier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-160">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-161">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="d2088-161">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="d2088-162">Représente une réponse à accepter à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="d2088-162">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d2088-163">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="d2088-163">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="d2088-164">Représente un provisoire répond à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="d2088-164">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d2088-165">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="d2088-165">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="d2088-166">Représente une réponse de refus à une demande de réunion.</span><span class="sxs-lookup"><span data-stu-id="d2088-166">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="d2088-167">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="d2088-167">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="d2088-168">Supprime un élément de la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2088-168">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d2088-169">Task</span><span class="sxs-lookup"><span data-stu-id="d2088-169">Task</span></span>](task.md) <br/> |<span data-ttu-id="d2088-170">Représente un élément de tâche dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-170">Represents a task item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-171">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="d2088-171">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="d2088-172">Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2088-172">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d2088-173">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="d2088-173">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="d2088-174">Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2088-174">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d2088-175">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="d2088-175">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="d2088-176">Contient un élément de la banque Exchange pour transférer à des destinataires.</span><span class="sxs-lookup"><span data-stu-id="d2088-176">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="d2088-177">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="d2088-177">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="d2088-178">Représente l'objet de réponse qui est utilisé pour annuler une réunion.</span><span class="sxs-lookup"><span data-stu-id="d2088-178">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="d2088-179">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="d2088-179">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="d2088-180">Représente un dossier de tâches dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-180">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d2088-181">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="d2088-181">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="d2088-182">Représente un dossier de recherche dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d2088-182">Represents a search folder in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2088-183">Remarques</span><span class="sxs-lookup"><span data-stu-id="d2088-183">Remarks</span></span>

<span data-ttu-id="d2088-184">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d2088-184">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2088-185">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d2088-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2088-186">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d2088-186">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2088-187">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d2088-187">Schema Name</span></span>  <br/> |<span data-ttu-id="d2088-188">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d2088-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="d2088-189">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d2088-189">Validation File</span></span>  <br/> |<span data-ttu-id="d2088-190">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d2088-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2088-191">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d2088-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2088-192">False</span><span class="sxs-lookup"><span data-stu-id="d2088-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2088-193">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d2088-193">See also</span></span>

- [<span data-ttu-id="d2088-194">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d2088-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

