---
title: MessageXml
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageXml
api_type:
- schema
ms.assetid: bcaf9e35-d351-48f3-baad-f90c633cba8a
description: L’élément MessageXml fournit des informations de réponse d’erreur supplémentaires.
ms.openlocfilehash: 8b6d201fe35c99a65f920ed7f60c33a2271fbd2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828470"
---
# <a name="messagexml"></a><span data-ttu-id="667e1-103">MessageXml</span><span class="sxs-lookup"><span data-stu-id="667e1-103">MessageXml</span></span>

<span data-ttu-id="667e1-104">L’élément **MessageXml** fournit des informations de réponse d’erreur supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="667e1-104">The **MessageXml** element provides additional error response information.</span></span> 
  
- [<span data-ttu-id="667e1-105">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-105">ResponseMessage</span></span>](responsemessage.md)  
- [<span data-ttu-id="667e1-106">MessageXml</span><span class="sxs-lookup"><span data-stu-id="667e1-106">MessageXml</span></span>](messagexml.md)
  
```XML
<MessageXml/>
```

 <span data-ttu-id="667e1-107">**xs : tout**</span><span class="sxs-lookup"><span data-stu-id="667e1-107">**xs:any**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="667e1-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="667e1-108">Attributes and elements</span></span>

<span data-ttu-id="667e1-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="667e1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="667e1-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="667e1-110">Attributes</span></span>

<span data-ttu-id="667e1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="667e1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="667e1-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="667e1-112">Child elements</span></span>

<span data-ttu-id="667e1-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="667e1-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="667e1-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="667e1-114">Parent elements</span></span>

|<span data-ttu-id="667e1-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="667e1-115">**Element**</span></span>|<span data-ttu-id="667e1-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="667e1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="667e1-117">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-117">ResponseMessage</span></span>](responsemessage.md) <br/> | <span data-ttu-id="667e1-118">Fournit des informations descriptives concernant l’état de réponse.</span><span class="sxs-lookup"><span data-stu-id="667e1-118">Provides descriptive information about the response status.</span></span> <br/> <br/>  <span data-ttu-id="667e1-119">Voici quelques-unes des expressions XPath possibles pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="667e1-119">The following are some of the possible XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/ResponseMessage` <br/> <br/> `/GetUserAvailabilityResponse/SuggestionsResponse/ResponseMessage` <br/><br/>  `/SetUserOofSettingsResponse/ResponseMessage` <br/><br/>  `/GetUserOofSettingsResponse/ResponseMessage` <br/> |
|[<span data-ttu-id="667e1-120">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-120">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md) <br/> |<span data-ttu-id="667e1-121">Contient l’état et les résultats d’une seule demande DeleteItem.</span><span class="sxs-lookup"><span data-stu-id="667e1-121">Contains the status and result of a single DeleteItem request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-122">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-122">SendItemResponseMessage</span></span>](senditemresponsemessage.md) <br/> |<span data-ttu-id="667e1-123">Contient l’état et les résultats d’une seule demande SendItem.</span><span class="sxs-lookup"><span data-stu-id="667e1-123">Contains the status and result of a single SendItem request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-124">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-124">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md) <br/> |<span data-ttu-id="667e1-125">Contient l’état et les résultats d’une seule demande DeleteFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-125">Contains the status and result of a single DeleteFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-126">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-126">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md) <br/> |<span data-ttu-id="667e1-127">Contient l’état et les résultats d’une seule demande DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="667e1-127">Contains the status and result of a single DeleteAttachment request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-128">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-128">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md) <br/> |<span data-ttu-id="667e1-129">Contient l’état et les résultats d’une demande de désabonnement unique.</span><span class="sxs-lookup"><span data-stu-id="667e1-129">Contains the status and result of a single Unsubscribe request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-130">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-130">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md) <br/> |<span data-ttu-id="667e1-131">Contient l’état et les résultats d’une seule demande CreateFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-131">Contains the status and result of a single CreateFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-132">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-132">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md) <br/> |<span data-ttu-id="667e1-133">Contient l’état et les résultats d’une seule demande GetFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-133">Contains the status and result of a single GetFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-134">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-134">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md) <br/> |<span data-ttu-id="667e1-135">Contient l’état et les résultats d’une seule demande UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-135">Contains the status and result of a single UpdateFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-136">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-136">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md) <br/> |<span data-ttu-id="667e1-137">Contient l’état et les résultats d’une seule demande MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-137">Contains the status and result of a single MoveFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-138">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-138">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md) <br/> |<span data-ttu-id="667e1-139">Contient l’état et les résultats d’une seule demande CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-139">Contains the status and result of a single CopyFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-140">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-140">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md) <br/> |<span data-ttu-id="667e1-141">Contient l’état et les résultats d’une seule demande CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-141">Contains the status and result of a single CreateManagedFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-142">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-142">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md) <br/> |<span data-ttu-id="667e1-143">Contient l’état et les résultats d’une seule demande FindFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-143">Contains the status and result of a single FindFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-144">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-144">CreateItemResponseMessage</span></span>](createitemresponsemessage.md) <br/> |<span data-ttu-id="667e1-145">Contient l’état et les résultats d’une demande CreateItem unique.</span><span class="sxs-lookup"><span data-stu-id="667e1-145">Contains the status and result of a single CreateItem request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-146">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-146">GetItemResponseMessage</span></span>](getitemresponsemessage.md) <br/> |<span data-ttu-id="667e1-147">Contient l’état et les résultats d’une demande de GetItem unique.</span><span class="sxs-lookup"><span data-stu-id="667e1-147">Contains the status and result of a single GetItem request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-148">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-148">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="667e1-149">Contient l’état et les résultats d’une seule demande UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="667e1-149">Contains the status and result of a single UpdateItem request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-150">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-150">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md) <br/> |<span data-ttu-id="667e1-151">Contient l’état et les résultats d’une seule demande MoveItem.</span><span class="sxs-lookup"><span data-stu-id="667e1-151">Contains the status and result of a single MoveItem request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-152">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-152">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md) <br/> |<span data-ttu-id="667e1-153">Contient l’état et les résultats d’une seule demande CopyItem.</span><span class="sxs-lookup"><span data-stu-id="667e1-153">Contains the status and result of a single CopyItem request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-154">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-154">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md) <br/> |<span data-ttu-id="667e1-155">Contient l’état et les résultats d’une seule demande CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="667e1-155">Contains the status and result of a single CreateAttachment request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-156">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-156">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md) <br/> |<span data-ttu-id="667e1-157">Contient l’état et les résultats d’une seule demande GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="667e1-157">Contains the status and result of a single GetAttachment request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-158">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-158">FindItemResponseMessage</span></span>](finditemresponsemessage.md) <br/> |<span data-ttu-id="667e1-159">Contient l’état et les résultats d’une seule demande FindItem.</span><span class="sxs-lookup"><span data-stu-id="667e1-159">Contains the status and result of a single FindItem request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-160">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-160">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md) <br/> |<span data-ttu-id="667e1-161">Contient l’état et les résultats d’une demande ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="667e1-161">Contains the status and result of a ResolveNames request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-162">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-162">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md) <br/> |<span data-ttu-id="667e1-163">Contient l’état et les résultats d’une seule demande ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="667e1-163">Contains the status and result of a single ExpandDL request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-164">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-164">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="667e1-165">Contient l’état et les résultats d’une seule demande Subscribe.</span><span class="sxs-lookup"><span data-stu-id="667e1-165">Contains the status and result of a single Subscribe request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-166">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-166">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md) <br/> |<span data-ttu-id="667e1-167">Contient l’état et les résultats d’une seule demande GetEvents.</span><span class="sxs-lookup"><span data-stu-id="667e1-167">Contains the status and result of a single GetEvents request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-168">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-168">SendNotificationResponseMessage</span></span>](sendnotificationresponsemessage.md) <br/> |<span data-ttu-id="667e1-169">Contient l’état et les résultats d’une requête SendNotification.</span><span class="sxs-lookup"><span data-stu-id="667e1-169">Contains the status and result of a single SendNotification request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-170">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-170">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="667e1-171">Contient l’état et les résultats d’une demande SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="667e1-171">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-172">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-172">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="667e1-173">Contient l’état et les résultats d’une demande SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="667e1-173">Contains the status and result of a SyncFolderItems request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-174">ConvertIdResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-174">ConvertIdResponseMessage</span></span>](convertidresponsemessage.md) <br/> |<span data-ttu-id="667e1-175">Contient l’état et les résultats d’une demande ConvertId.</span><span class="sxs-lookup"><span data-stu-id="667e1-175">Contains the status and result of a ConvertId request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-176">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="667e1-176">AddDelegateResponse</span></span>](adddelegateresponse.md) <br/> |<span data-ttu-id="667e1-177">Contient l’état et les résultats d’une requête AddDelegate.</span><span class="sxs-lookup"><span data-stu-id="667e1-177">Contains the status and result of an AddDelegate request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-178">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-178">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="667e1-179">Contient l’état et les résultats d’une demande GetServerTimeZones.</span><span class="sxs-lookup"><span data-stu-id="667e1-179">Contains the status and result of a GetServerTimeZones request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-180">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-180">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="667e1-181">Contient l’état et les résultats d’une demande GetSharingFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-181">Contains the status and result of a GetSharingFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-182">GetSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="667e1-182">GetSharingFolderResponse</span></span>](getsharingfolderresponse.md) <br/> |<span data-ttu-id="667e1-183">Définit une réponse à une demande de GetSharingFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-183">Defines a response to a GetSharingFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-184">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-184">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="667e1-185">Contient l’état et les résultats d’une demande GetSharingMetadata.</span><span class="sxs-lookup"><span data-stu-id="667e1-185">Contains the status and result of a GetSharingMetadata request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-186">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="667e1-186">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="667e1-187">Définit une réponse à une demande de GetSharingMetadata.</span><span class="sxs-lookup"><span data-stu-id="667e1-187">Defines a response to a GetSharingMetadata request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-188">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-188">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="667e1-189">Contient l’état et les résultats d’une demande RefreshSharingFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-189">Contains the status and result of a RefreshSharingFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-190">RefreshSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="667e1-190">RefreshSharingFolderResponse</span></span>](refreshsharingfolderresponse.md) <br/> |<span data-ttu-id="667e1-191">Définit une réponse à une demande de RefreshSharingFolder.</span><span class="sxs-lookup"><span data-stu-id="667e1-191">Defines a response to a RefreshSharingFolder request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-192">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="667e1-192">FindConversationResponse</span></span>](findconversationresponse.md) <br/> |<span data-ttu-id="667e1-193">Contient l’état et les résultats d’une réponse **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="667e1-193">Contains the status and results of a **FindConversation** response.</span></span>  <br/> |
|[<span data-ttu-id="667e1-194">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-194">EmptyFolderResponseMessage</span></span>](emptyfolderresponsemessage.md) <br/> |<span data-ttu-id="667e1-195">Contient l’état et le résultat d’une demande **EmptyFolder** .</span><span class="sxs-lookup"><span data-stu-id="667e1-195">Contains the status and result of an **EmptyFolder** request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-196">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="667e1-196">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md) <br/> |<span data-ttu-id="667e1-197">Contient un état et les résultats d’une requête **UpdateInboxRules** .</span><span class="sxs-lookup"><span data-stu-id="667e1-197">Contains a status and result of an **UpdateInboxRules** request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-198">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667e1-198">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md) <br/> |<span data-ttu-id="667e1-199">Contient un état et les résultats d’une requête **UploadItemsResponse** .</span><span class="sxs-lookup"><span data-stu-id="667e1-199">Contains a status and result of an **UploadItemsResponse** request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-200">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="667e1-200">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="667e1-201">Contient une réponse à une demande de **GetInboxRules** .</span><span class="sxs-lookup"><span data-stu-id="667e1-201">Contains a response to a **GetInboxRules** request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-202">GetServiceConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="667e1-202">GetServiceConfigurationResponse</span></span>](getserviceconfigurationresponse.md) <br/> |<span data-ttu-id="667e1-203">Contient une réponse à une demande de **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="667e1-203">Contains a response to a **GetServiceConfiguration** request.</span></span>  <br/> |
|[<span data-ttu-id="667e1-204">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="667e1-204">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="667e1-205">Contient les paramètres de configuration de service.</span><span class="sxs-lookup"><span data-stu-id="667e1-205">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="667e1-206">Remarques</span><span class="sxs-lookup"><span data-stu-id="667e1-206">Remarks</span></span>

<span data-ttu-id="667e1-207">Cet élément n’est pas obligatoire et n’est pas inclus dans toutes les réponses.</span><span class="sxs-lookup"><span data-stu-id="667e1-207">This element is not required and is not included in all responses.</span></span> <span data-ttu-id="667e1-208">Il est inclus pour les messages d’erreur.</span><span class="sxs-lookup"><span data-stu-id="667e1-208">It is included for error messages.</span></span> <span data-ttu-id="667e1-209">Dans les requêtes qui impliquent des dossiers ou des éléments, l’élément **MessageXML** contient un ou plusieurs éléments qui contiennent les URI pour les propriétés qui a provoqué l’erreur.</span><span class="sxs-lookup"><span data-stu-id="667e1-209">In requests that involve folders or items, the **MessageXML** element will contain one or more elements that contain the URIs to the properties that caused the error.</span></span> <span data-ttu-id="667e1-210">Un exemple est l’élément [FieldURI](fielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="667e1-210">An example of this is the [FieldURI](fielduri.md) element.</span></span> 
  
<span data-ttu-id="667e1-211">L’élément **MessageXML** est de type **xs : tout**, ce qui signifie que n’importe quel code XML bien formé est contenu valide pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="667e1-211">The **MessageXML** element is of type **xs:any**, which means that any well-formed XML is valid content for the this element.</span></span>
  
<span data-ttu-id="667e1-212">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="667e1-212">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="667e1-213">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="667e1-213">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="667e1-214">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="667e1-214">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="667e1-215">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="667e1-215">Schema Name</span></span>  <br/> |<span data-ttu-id="667e1-216">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="667e1-216">Messages schema</span></span>  <br/> |
|<span data-ttu-id="667e1-217">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="667e1-217">Validation File</span></span>  <br/> |<span data-ttu-id="667e1-218">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="667e1-218">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="667e1-219">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="667e1-219">Can be Empty</span></span>  <br/> |<span data-ttu-id="667e1-220">False</span><span class="sxs-lookup"><span data-stu-id="667e1-220">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="667e1-221">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="667e1-221">See also</span></span>

- [<span data-ttu-id="667e1-222">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="667e1-222">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
