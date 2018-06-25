---
title: FieldUri (règle)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: L’élément FieldURI Spécifie l’URI pour le champ règle qui a provoqué l’erreur de validation.
ms.openlocfilehash: 88ba54994625d3a950b58e900f28c986c31eddac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756353"
---
# <a name="fielduri-rule"></a><span data-ttu-id="b8477-103">FieldUri (règle)</span><span class="sxs-lookup"><span data-stu-id="b8477-103">FieldUri (Rule)</span></span>

<span data-ttu-id="b8477-104">L’élément **FieldURI** Spécifie l’URI pour le champ règle qui a provoqué l’erreur de validation.</span><span class="sxs-lookup"><span data-stu-id="b8477-104">The **FieldURI** element specifies the URI to the rule field that caused the validation error.</span></span> 
  
```XML
<FieldURI/>
```

 <span data-ttu-id="b8477-105">**RuleFieldURIType**</span><span class="sxs-lookup"><span data-stu-id="b8477-105">**RuleFieldURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8477-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b8477-106">Attributes and elements</span></span>

<span data-ttu-id="b8477-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b8477-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8477-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b8477-108">Attributes</span></span>

<span data-ttu-id="b8477-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b8477-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8477-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b8477-110">Child elements</span></span>

<span data-ttu-id="b8477-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b8477-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b8477-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b8477-112">Parent elements</span></span>

|<span data-ttu-id="b8477-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b8477-113">**Element**</span></span>|<span data-ttu-id="b8477-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b8477-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8477-115">Erreur</span><span class="sxs-lookup"><span data-stu-id="b8477-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="b8477-116">Représente une seule erreur de validation sur une valeur de la propriété règle particulière, la valeur de propriété prédicat ou la valeur de la propriété action.</span><span class="sxs-lookup"><span data-stu-id="b8477-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b8477-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b8477-117">Text value</span></span>

<span data-ttu-id="b8477-118">La valeur de texte pour cet élément est limitée à une des chaînes suivantes :</span><span class="sxs-lookup"><span data-stu-id="b8477-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="b8477-119">ID de la règle</span><span class="sxs-lookup"><span data-stu-id="b8477-119">RuleId</span></span>
    
- <span data-ttu-id="b8477-120">DisplayName</span><span class="sxs-lookup"><span data-stu-id="b8477-120">DisplayName</span></span>
    
- <span data-ttu-id="b8477-121">Priority</span><span class="sxs-lookup"><span data-stu-id="b8477-121">Priority</span></span>
    
- <span data-ttu-id="b8477-122">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="b8477-122">IsNotSupported</span></span>
    
- <span data-ttu-id="b8477-123">Actions</span><span class="sxs-lookup"><span data-stu-id="b8477-123">Actions</span></span>
    
- <span data-ttu-id="b8477-124">Condition : catégories</span><span class="sxs-lookup"><span data-stu-id="b8477-124">Condition:Categories</span></span>
    
- <span data-ttu-id="b8477-125">Condition : ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-125">Condition:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="b8477-126">Condition : ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-126">Condition:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="b8477-127">Condition : ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-127">Condition:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="b8477-128">Condition : ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-128">Condition:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="b8477-129">Condition : ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-129">Condition:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="b8477-130">Condition : ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-130">Condition:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="b8477-131">Condition : FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="b8477-131">Condition:FlaggedForAction</span></span>
    
- <span data-ttu-id="b8477-132">Condition : FromAddresses</span><span class="sxs-lookup"><span data-stu-id="b8477-132">Condition:FromAddresses</span></span>
    
- <span data-ttu-id="b8477-133">Condition : FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="b8477-133">Condition:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="b8477-134">Condition : HasAttachments</span><span class="sxs-lookup"><span data-stu-id="b8477-134">Condition:HasAttachments</span></span>
    
- <span data-ttu-id="b8477-135">Condition : Importance</span><span class="sxs-lookup"><span data-stu-id="b8477-135">Condition:Importance</span></span>
    
- <span data-ttu-id="b8477-136">Condition : IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="b8477-136">Condition:IsApprovalRequest</span></span>
    
- <span data-ttu-id="b8477-137">Condition : IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="b8477-137">Condition:IsAutomaticForward</span></span>
    
- <span data-ttu-id="b8477-138">Condition : IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="b8477-138">Condition:IsAutomaticReply</span></span>
    
- <span data-ttu-id="b8477-139">Condition : IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="b8477-139">Condition:IsEncrypted</span></span>
    
- <span data-ttu-id="b8477-140">Condition : IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b8477-140">Condition:IsMeetingRequest</span></span>
    
- <span data-ttu-id="b8477-141">Condition : IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b8477-141">Condition:IsMeetingResponse</span></span>
    
- <span data-ttu-id="b8477-142">Condition : IsNDR</span><span class="sxs-lookup"><span data-stu-id="b8477-142">Condition:IsNDR</span></span>
    
- <span data-ttu-id="b8477-143">Condition : IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="b8477-143">Condition:IsPermissionControlled</span></span>
    
- <span data-ttu-id="b8477-144">Condition : IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="b8477-144">Condition:IsReadReceipt</span></span>
    
- <span data-ttu-id="b8477-145">Condition : IsSigned</span><span class="sxs-lookup"><span data-stu-id="b8477-145">Condition:IsSigned</span></span>
    
- <span data-ttu-id="b8477-146">Condition : IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="b8477-146">Condition:IsVoicemail</span></span>
    
- <span data-ttu-id="b8477-147">Condition : ItemClasses</span><span class="sxs-lookup"><span data-stu-id="b8477-147">Condition:ItemClasses</span></span>
    
- <span data-ttu-id="b8477-148">Condition : MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="b8477-148">Condition:MessageClassifications</span></span>
    
- <span data-ttu-id="b8477-149">Condition : NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="b8477-149">Condition:NotSentToMe</span></span>
    
- <span data-ttu-id="b8477-150">Condition : SentCcMe</span><span class="sxs-lookup"><span data-stu-id="b8477-150">Condition:SentCcMe</span></span>
    
- <span data-ttu-id="b8477-151">Condition : SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="b8477-151">Condition:SentOnlyToMe</span></span>
    
- <span data-ttu-id="b8477-152">Condition : SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="b8477-152">Condition:SentToAddresses</span></span>
    
- <span data-ttu-id="b8477-153">Condition : SentToMe</span><span class="sxs-lookup"><span data-stu-id="b8477-153">Condition:SentToMe</span></span>
    
- <span data-ttu-id="b8477-154">Condition : SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="b8477-154">Condition:SentToOrCcMe</span></span>
    
- <span data-ttu-id="b8477-155">Condition : critère de diffusion</span><span class="sxs-lookup"><span data-stu-id="b8477-155">Condition:Sensitivity</span></span>
    
- <span data-ttu-id="b8477-156">Condition : WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="b8477-156">Condition:WithinDateRange</span></span>
    
- <span data-ttu-id="b8477-157">Condition : WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="b8477-157">Condition:WithinSizeRange</span></span>
    
- <span data-ttu-id="b8477-158">Exception : catégories</span><span class="sxs-lookup"><span data-stu-id="b8477-158">Exception:Categories</span></span>
    
- <span data-ttu-id="b8477-159">Exception : ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-159">Exception:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="b8477-160">Exception : ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-160">Exception:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="b8477-161">Exception : ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-161">Exception:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="b8477-162">Exception : ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-162">Exception:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="b8477-163">Exception : ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-163">Exception:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="b8477-164">Exception : ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="b8477-164">Exception:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="b8477-165">Exception : FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="b8477-165">Exception:FlaggedForAction</span></span>
    
- <span data-ttu-id="b8477-166">Exception : FromAddresses</span><span class="sxs-lookup"><span data-stu-id="b8477-166">Exception:FromAddresses</span></span>
    
- <span data-ttu-id="b8477-167">Exception : FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="b8477-167">Exception:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="b8477-168">Exception : HasAttachments</span><span class="sxs-lookup"><span data-stu-id="b8477-168">Exception:HasAttachments</span></span>
    
- <span data-ttu-id="b8477-169">Exception : Importance</span><span class="sxs-lookup"><span data-stu-id="b8477-169">Exception:Importance</span></span>
    
- <span data-ttu-id="b8477-170">Exception : IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="b8477-170">Exception:IsApprovalRequest</span></span>
    
- <span data-ttu-id="b8477-171">Exception : IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="b8477-171">Exception:IsAutomaticForward</span></span>
    
- <span data-ttu-id="b8477-172">Exception : IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="b8477-172">Exception:IsAutomaticReply</span></span>
    
- <span data-ttu-id="b8477-173">Exception : IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="b8477-173">Exception:IsEncrypted</span></span>
    
- <span data-ttu-id="b8477-174">Exception : IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b8477-174">Exception:IsMeetingRequest</span></span>
    
- <span data-ttu-id="b8477-175">Exception : IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b8477-175">Exception:IsMeetingResponse</span></span>
    
- <span data-ttu-id="b8477-176">Exception : IsNDR</span><span class="sxs-lookup"><span data-stu-id="b8477-176">Exception:IsNDR</span></span>
    
- <span data-ttu-id="b8477-177">Exception : IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="b8477-177">Exception:IsPermissionControlled</span></span>
    
- <span data-ttu-id="b8477-178">Exception : IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="b8477-178">Exception:IsReadReceipt</span></span>
    
- <span data-ttu-id="b8477-179">Exception : IsSigned</span><span class="sxs-lookup"><span data-stu-id="b8477-179">Exception:IsSigned</span></span>
    
- <span data-ttu-id="b8477-180">Exception : IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="b8477-180">Exception:IsVoicemail</span></span>
    
- <span data-ttu-id="b8477-181">Exception : ItemClasses</span><span class="sxs-lookup"><span data-stu-id="b8477-181">Exception:ItemClasses</span></span>
    
- <span data-ttu-id="b8477-182">Exception : MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="b8477-182">Exception:MessageClassifications</span></span>
    
- <span data-ttu-id="b8477-183">Exception : NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="b8477-183">Exception:NotSentToMe</span></span>
    
- <span data-ttu-id="b8477-184">Exception : SentCcMe</span><span class="sxs-lookup"><span data-stu-id="b8477-184">Exception:SentCcMe</span></span>
    
- <span data-ttu-id="b8477-185">Exception : SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="b8477-185">Exception:SentOnlyToMe</span></span>
    
- <span data-ttu-id="b8477-186">Exception : SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="b8477-186">Exception:SentToAddresses</span></span>
    
- <span data-ttu-id="b8477-187">Exception : SentToMe</span><span class="sxs-lookup"><span data-stu-id="b8477-187">Exception:SentToMe</span></span>
    
- <span data-ttu-id="b8477-188">Exception : SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="b8477-188">Exception:SentToOrCcMe</span></span>
    
- <span data-ttu-id="b8477-189">Exception : critère de diffusion</span><span class="sxs-lookup"><span data-stu-id="b8477-189">Exception:Sensitivity</span></span>
    
- <span data-ttu-id="b8477-190">Exception : WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="b8477-190">Exception:WithinDateRange</span></span>
    
- <span data-ttu-id="b8477-191">Exception : WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="b8477-191">Exception:WithinSizeRange</span></span>
    
- <span data-ttu-id="b8477-192">Action : AssignCategories</span><span class="sxs-lookup"><span data-stu-id="b8477-192">Action:AssignCategories</span></span>
    
- <span data-ttu-id="b8477-193">Action : CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="b8477-193">Action:CopyToFolder</span></span>
    
- <span data-ttu-id="b8477-194">Suppression de l’action :</span><span class="sxs-lookup"><span data-stu-id="b8477-194">Action:Delete</span></span>
    
- <span data-ttu-id="b8477-195">Action : ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="b8477-195">Action:ForwardAsAttachmentToRecipients</span></span>
    
- <span data-ttu-id="b8477-196">Action : ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="b8477-196">Action:ForwardToRecipients</span></span>
    
- <span data-ttu-id="b8477-197">Action : MarkImportance</span><span class="sxs-lookup"><span data-stu-id="b8477-197">Action:MarkImportance</span></span>
    
- <span data-ttu-id="b8477-198">Action : MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="b8477-198">Action:MarkAsRead</span></span>
    
- <span data-ttu-id="b8477-199">Action : MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="b8477-199">Action:MoveToFolder</span></span>
    
- <span data-ttu-id="b8477-200">Action : PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="b8477-200">Action:PermanentDelete</span></span>
    
- <span data-ttu-id="b8477-201">Action : RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="b8477-201">Action:RedirectToRecipients</span></span>
    
- <span data-ttu-id="b8477-202">Action : SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="b8477-202">Action:SendSMSAlertToRecipients</span></span>
    
- <span data-ttu-id="b8477-203">Action : ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="b8477-203">Action:ServerReplyWithMessage</span></span>
    
- <span data-ttu-id="b8477-204">Action : StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="b8477-204">Action:StopProcessingRules</span></span>
    
- <span data-ttu-id="b8477-205">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="b8477-205">IsEnabled</span></span>
    
- <span data-ttu-id="b8477-206">IsInError</span><span class="sxs-lookup"><span data-stu-id="b8477-206">IsInError</span></span>
    
- <span data-ttu-id="b8477-207">Conditions</span><span class="sxs-lookup"><span data-stu-id="b8477-207">Conditions</span></span>
    
- <span data-ttu-id="b8477-208">Exceptions</span><span class="sxs-lookup"><span data-stu-id="b8477-208">Exceptions</span></span>
    
## <a name="remarks"></a><span data-ttu-id="b8477-209">Remarques</span><span class="sxs-lookup"><span data-stu-id="b8477-209">Remarks</span></span>

<span data-ttu-id="b8477-210">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b8477-210">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8477-211">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b8477-211">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8477-212">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b8477-212">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b8477-213">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b8477-213">Schema Name</span></span>  <br/> |<span data-ttu-id="b8477-214">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b8477-214">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b8477-215">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b8477-215">Validation File</span></span>  <br/> |<span data-ttu-id="b8477-216">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b8477-216">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b8477-217">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b8477-217">Can be Empty</span></span>  <br/> |<span data-ttu-id="b8477-218">False</span><span class="sxs-lookup"><span data-stu-id="b8477-218">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b8477-219">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b8477-219">See also</span></span>



- [<span data-ttu-id="b8477-220">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b8477-220">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

