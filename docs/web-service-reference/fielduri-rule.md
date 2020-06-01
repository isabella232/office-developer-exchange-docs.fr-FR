---
title: FieldUri (règle)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: L’élément FieldURI spécifie l’URI vers le champ de règle à l’origine de l’erreur de validation.
ms.openlocfilehash: 3d88efdf951af580f81b5e2e7a544dcdf70ea830
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461246"
---
# <a name="fielduri-rule"></a><span data-ttu-id="37275-103">FieldUri (règle)</span><span class="sxs-lookup"><span data-stu-id="37275-103">FieldUri (Rule)</span></span>

<span data-ttu-id="37275-104">L’élément **FieldURI** spécifie l’URI vers le champ de règle à l’origine de l’erreur de validation.</span><span class="sxs-lookup"><span data-stu-id="37275-104">The **FieldURI** element specifies the URI to the rule field that caused the validation error.</span></span> 
  
```XML
<FieldURI/>
```

 <span data-ttu-id="37275-105">**RuleFieldURIType**</span><span class="sxs-lookup"><span data-stu-id="37275-105">**RuleFieldURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37275-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="37275-106">Attributes and elements</span></span>

<span data-ttu-id="37275-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="37275-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37275-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="37275-108">Attributes</span></span>

<span data-ttu-id="37275-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="37275-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37275-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="37275-110">Child elements</span></span>

<span data-ttu-id="37275-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="37275-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="37275-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="37275-112">Parent elements</span></span>

|<span data-ttu-id="37275-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="37275-113">**Element**</span></span>|<span data-ttu-id="37275-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="37275-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37275-115">Erreur</span><span class="sxs-lookup"><span data-stu-id="37275-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="37275-116">Représente une seule erreur de validation sur une valeur de propriété de règle, une valeur de propriété de prédicat ou une valeur de propriété d’action particulière.</span><span class="sxs-lookup"><span data-stu-id="37275-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="37275-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="37275-117">Text value</span></span>

<span data-ttu-id="37275-118">La valeur de texte de cet élément est restreinte à l’une des chaînes suivantes :</span><span class="sxs-lookup"><span data-stu-id="37275-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="37275-119">RuleId</span><span class="sxs-lookup"><span data-stu-id="37275-119">RuleId</span></span>
    
- <span data-ttu-id="37275-120">DisplayName</span><span class="sxs-lookup"><span data-stu-id="37275-120">DisplayName</span></span>
    
- <span data-ttu-id="37275-121">Priority</span><span class="sxs-lookup"><span data-stu-id="37275-121">Priority</span></span>
    
- <span data-ttu-id="37275-122">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="37275-122">IsNotSupported</span></span>
    
- <span data-ttu-id="37275-123">Actions</span><span class="sxs-lookup"><span data-stu-id="37275-123">Actions</span></span>
    
- <span data-ttu-id="37275-124">Condition : catégories</span><span class="sxs-lookup"><span data-stu-id="37275-124">Condition:Categories</span></span>
    
- <span data-ttu-id="37275-125">Condition : ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="37275-125">Condition:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="37275-126">Condition : ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="37275-126">Condition:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="37275-127">Condition : ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="37275-127">Condition:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="37275-128">Condition : ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="37275-128">Condition:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="37275-129">Condition : ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="37275-129">Condition:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="37275-130">Condition : ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="37275-130">Condition:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="37275-131">Condition : FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="37275-131">Condition:FlaggedForAction</span></span>
    
- <span data-ttu-id="37275-132">Condition : FromAddresses</span><span class="sxs-lookup"><span data-stu-id="37275-132">Condition:FromAddresses</span></span>
    
- <span data-ttu-id="37275-133">Condition : FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="37275-133">Condition:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="37275-134">Condition : HasAttachments</span><span class="sxs-lookup"><span data-stu-id="37275-134">Condition:HasAttachments</span></span>
    
- <span data-ttu-id="37275-135">Condition : importance</span><span class="sxs-lookup"><span data-stu-id="37275-135">Condition:Importance</span></span>
    
- <span data-ttu-id="37275-136">Condition : IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="37275-136">Condition:IsApprovalRequest</span></span>
    
- <span data-ttu-id="37275-137">Condition : IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="37275-137">Condition:IsAutomaticForward</span></span>
    
- <span data-ttu-id="37275-138">Condition : IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="37275-138">Condition:IsAutomaticReply</span></span>
    
- <span data-ttu-id="37275-139">Condition : IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="37275-139">Condition:IsEncrypted</span></span>
    
- <span data-ttu-id="37275-140">Condition : IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="37275-140">Condition:IsMeetingRequest</span></span>
    
- <span data-ttu-id="37275-141">Condition : IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="37275-141">Condition:IsMeetingResponse</span></span>
    
- <span data-ttu-id="37275-142">Condition : IsNDR</span><span class="sxs-lookup"><span data-stu-id="37275-142">Condition:IsNDR</span></span>
    
- <span data-ttu-id="37275-143">Condition : IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="37275-143">Condition:IsPermissionControlled</span></span>
    
- <span data-ttu-id="37275-144">Condition : IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="37275-144">Condition:IsReadReceipt</span></span>
    
- <span data-ttu-id="37275-145">Condition : IsSigned</span><span class="sxs-lookup"><span data-stu-id="37275-145">Condition:IsSigned</span></span>
    
- <span data-ttu-id="37275-146">Condition : IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="37275-146">Condition:IsVoicemail</span></span>
    
- <span data-ttu-id="37275-147">Condition : ItemClasses</span><span class="sxs-lookup"><span data-stu-id="37275-147">Condition:ItemClasses</span></span>
    
- <span data-ttu-id="37275-148">Condition : MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="37275-148">Condition:MessageClassifications</span></span>
    
- <span data-ttu-id="37275-149">Condition : NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="37275-149">Condition:NotSentToMe</span></span>
    
- <span data-ttu-id="37275-150">Condition : SentCcMe</span><span class="sxs-lookup"><span data-stu-id="37275-150">Condition:SentCcMe</span></span>
    
- <span data-ttu-id="37275-151">Condition : SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="37275-151">Condition:SentOnlyToMe</span></span>
    
- <span data-ttu-id="37275-152">Condition : SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="37275-152">Condition:SentToAddresses</span></span>
    
- <span data-ttu-id="37275-153">Condition : SentToMe</span><span class="sxs-lookup"><span data-stu-id="37275-153">Condition:SentToMe</span></span>
    
- <span data-ttu-id="37275-154">Condition : SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="37275-154">Condition:SentToOrCcMe</span></span>
    
- <span data-ttu-id="37275-155">Condition : sensibilité</span><span class="sxs-lookup"><span data-stu-id="37275-155">Condition:Sensitivity</span></span>
    
- <span data-ttu-id="37275-156">Condition : WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="37275-156">Condition:WithinDateRange</span></span>
    
- <span data-ttu-id="37275-157">Condition : WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="37275-157">Condition:WithinSizeRange</span></span>
    
- <span data-ttu-id="37275-158">Exception : Categories</span><span class="sxs-lookup"><span data-stu-id="37275-158">Exception:Categories</span></span>
    
- <span data-ttu-id="37275-159">Exception : ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="37275-159">Exception:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="37275-160">Exception : ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="37275-160">Exception:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="37275-161">Exception : ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="37275-161">Exception:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="37275-162">Exception : ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="37275-162">Exception:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="37275-163">Exception : ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="37275-163">Exception:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="37275-164">Exception : ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="37275-164">Exception:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="37275-165">Exception : FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="37275-165">Exception:FlaggedForAction</span></span>
    
- <span data-ttu-id="37275-166">Exception : FromAddresses</span><span class="sxs-lookup"><span data-stu-id="37275-166">Exception:FromAddresses</span></span>
    
- <span data-ttu-id="37275-167">Exception : FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="37275-167">Exception:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="37275-168">Exception : HasAttachments</span><span class="sxs-lookup"><span data-stu-id="37275-168">Exception:HasAttachments</span></span>
    
- <span data-ttu-id="37275-169">Exception : importance</span><span class="sxs-lookup"><span data-stu-id="37275-169">Exception:Importance</span></span>
    
- <span data-ttu-id="37275-170">Exception : IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="37275-170">Exception:IsApprovalRequest</span></span>
    
- <span data-ttu-id="37275-171">Exception : IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="37275-171">Exception:IsAutomaticForward</span></span>
    
- <span data-ttu-id="37275-172">Exception : IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="37275-172">Exception:IsAutomaticReply</span></span>
    
- <span data-ttu-id="37275-173">Exception : IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="37275-173">Exception:IsEncrypted</span></span>
    
- <span data-ttu-id="37275-174">Exception : IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="37275-174">Exception:IsMeetingRequest</span></span>
    
- <span data-ttu-id="37275-175">Exception : IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="37275-175">Exception:IsMeetingResponse</span></span>
    
- <span data-ttu-id="37275-176">Exception : IsNDR</span><span class="sxs-lookup"><span data-stu-id="37275-176">Exception:IsNDR</span></span>
    
- <span data-ttu-id="37275-177">Exception : IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="37275-177">Exception:IsPermissionControlled</span></span>
    
- <span data-ttu-id="37275-178">Exception : IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="37275-178">Exception:IsReadReceipt</span></span>
    
- <span data-ttu-id="37275-179">Exception : IsSigned</span><span class="sxs-lookup"><span data-stu-id="37275-179">Exception:IsSigned</span></span>
    
- <span data-ttu-id="37275-180">Exception : IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="37275-180">Exception:IsVoicemail</span></span>
    
- <span data-ttu-id="37275-181">Exception : ItemClasses</span><span class="sxs-lookup"><span data-stu-id="37275-181">Exception:ItemClasses</span></span>
    
- <span data-ttu-id="37275-182">Exception : MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="37275-182">Exception:MessageClassifications</span></span>
    
- <span data-ttu-id="37275-183">Exception : NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="37275-183">Exception:NotSentToMe</span></span>
    
- <span data-ttu-id="37275-184">Exception : SentCcMe</span><span class="sxs-lookup"><span data-stu-id="37275-184">Exception:SentCcMe</span></span>
    
- <span data-ttu-id="37275-185">Exception : SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="37275-185">Exception:SentOnlyToMe</span></span>
    
- <span data-ttu-id="37275-186">Exception : SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="37275-186">Exception:SentToAddresses</span></span>
    
- <span data-ttu-id="37275-187">Exception : SentToMe</span><span class="sxs-lookup"><span data-stu-id="37275-187">Exception:SentToMe</span></span>
    
- <span data-ttu-id="37275-188">Exception : SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="37275-188">Exception:SentToOrCcMe</span></span>
    
- <span data-ttu-id="37275-189">Exception : Sensitivity</span><span class="sxs-lookup"><span data-stu-id="37275-189">Exception:Sensitivity</span></span>
    
- <span data-ttu-id="37275-190">Exception : WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="37275-190">Exception:WithinDateRange</span></span>
    
- <span data-ttu-id="37275-191">Exception : WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="37275-191">Exception:WithinSizeRange</span></span>
    
- <span data-ttu-id="37275-192">Action : AssignCategories</span><span class="sxs-lookup"><span data-stu-id="37275-192">Action:AssignCategories</span></span>
    
- <span data-ttu-id="37275-193">Action : CopyToFolder,</span><span class="sxs-lookup"><span data-stu-id="37275-193">Action:CopyToFolder</span></span>
    
- <span data-ttu-id="37275-194">Action : supprimer</span><span class="sxs-lookup"><span data-stu-id="37275-194">Action:Delete</span></span>
    
- <span data-ttu-id="37275-195">Action : ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="37275-195">Action:ForwardAsAttachmentToRecipients</span></span>
    
- <span data-ttu-id="37275-196">Action : ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="37275-196">Action:ForwardToRecipients</span></span>
    
- <span data-ttu-id="37275-197">Action : MarkImportance</span><span class="sxs-lookup"><span data-stu-id="37275-197">Action:MarkImportance</span></span>
    
- <span data-ttu-id="37275-198">Action : MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="37275-198">Action:MarkAsRead</span></span>
    
- <span data-ttu-id="37275-199">Action : MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="37275-199">Action:MoveToFolder</span></span>
    
- <span data-ttu-id="37275-200">Action : PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="37275-200">Action:PermanentDelete</span></span>
    
- <span data-ttu-id="37275-201">Action : RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="37275-201">Action:RedirectToRecipients</span></span>
    
- <span data-ttu-id="37275-202">Action : SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="37275-202">Action:SendSMSAlertToRecipients</span></span>
    
- <span data-ttu-id="37275-203">Action : ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="37275-203">Action:ServerReplyWithMessage</span></span>
    
- <span data-ttu-id="37275-204">Action : StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="37275-204">Action:StopProcessingRules</span></span>
    
- <span data-ttu-id="37275-205">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="37275-205">IsEnabled</span></span>
    
- <span data-ttu-id="37275-206">IsInError</span><span class="sxs-lookup"><span data-stu-id="37275-206">IsInError</span></span>
    
- <span data-ttu-id="37275-207">Conditions</span><span class="sxs-lookup"><span data-stu-id="37275-207">Conditions</span></span>
    
- <span data-ttu-id="37275-208">Exceptions</span><span class="sxs-lookup"><span data-stu-id="37275-208">Exceptions</span></span>
    
## <a name="remarks"></a><span data-ttu-id="37275-209">Remarques</span><span class="sxs-lookup"><span data-stu-id="37275-209">Remarks</span></span>

<span data-ttu-id="37275-210">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="37275-210">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37275-211">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="37275-211">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37275-212">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="37275-212">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="37275-213">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="37275-213">Schema Name</span></span>  <br/> |<span data-ttu-id="37275-214">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="37275-214">Messages schema</span></span>  <br/> |
|<span data-ttu-id="37275-215">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="37275-215">Validation File</span></span>  <br/> |<span data-ttu-id="37275-216">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="37275-216">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="37275-217">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="37275-217">Can be Empty</span></span>  <br/> |<span data-ttu-id="37275-218">False</span><span class="sxs-lookup"><span data-stu-id="37275-218">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37275-219">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="37275-219">See also</span></span>



- [<span data-ttu-id="37275-220">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="37275-220">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

