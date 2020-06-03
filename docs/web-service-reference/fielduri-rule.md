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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461246"
---
# <a name="fielduri-rule"></a><span data-ttu-id="a966b-103">FieldUri (règle)</span><span class="sxs-lookup"><span data-stu-id="a966b-103">FieldUri (Rule)</span></span>

<span data-ttu-id="a966b-104">L’élément **FieldURI** spécifie l’URI vers le champ de règle à l’origine de l’erreur de validation.</span><span class="sxs-lookup"><span data-stu-id="a966b-104">The **FieldURI** element specifies the URI to the rule field that caused the validation error.</span></span> 
  
```XML
<FieldURI/>
```

 <span data-ttu-id="a966b-105">**RuleFieldURIType**</span><span class="sxs-lookup"><span data-stu-id="a966b-105">**RuleFieldURIType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a966b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a966b-106">Attributes and elements</span></span>

<span data-ttu-id="a966b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a966b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a966b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a966b-108">Attributes</span></span>

<span data-ttu-id="a966b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a966b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a966b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a966b-110">Child elements</span></span>

<span data-ttu-id="a966b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a966b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a966b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a966b-112">Parent elements</span></span>

|<span data-ttu-id="a966b-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a966b-113">**Element**</span></span>|<span data-ttu-id="a966b-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a966b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a966b-115">Erreur</span><span class="sxs-lookup"><span data-stu-id="a966b-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="a966b-116">Représente une seule erreur de validation sur une valeur de propriété de règle, une valeur de propriété de prédicat ou une valeur de propriété d’action particulière.</span><span class="sxs-lookup"><span data-stu-id="a966b-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a966b-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a966b-117">Text value</span></span>

<span data-ttu-id="a966b-118">La valeur de texte de cet élément est restreinte à l’une des chaînes suivantes :</span><span class="sxs-lookup"><span data-stu-id="a966b-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="a966b-119">RuleId</span><span class="sxs-lookup"><span data-stu-id="a966b-119">RuleId</span></span>
    
- <span data-ttu-id="a966b-120">DisplayName</span><span class="sxs-lookup"><span data-stu-id="a966b-120">DisplayName</span></span>
    
- <span data-ttu-id="a966b-121">Priority</span><span class="sxs-lookup"><span data-stu-id="a966b-121">Priority</span></span>
    
- <span data-ttu-id="a966b-122">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="a966b-122">IsNotSupported</span></span>
    
- <span data-ttu-id="a966b-123">Actions</span><span class="sxs-lookup"><span data-stu-id="a966b-123">Actions</span></span>
    
- <span data-ttu-id="a966b-124">Condition : catégories</span><span class="sxs-lookup"><span data-stu-id="a966b-124">Condition:Categories</span></span>
    
- <span data-ttu-id="a966b-125">Condition : ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-125">Condition:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="a966b-126">Condition : ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-126">Condition:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="a966b-127">Condition : ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-127">Condition:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="a966b-128">Condition : ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-128">Condition:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="a966b-129">Condition : ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-129">Condition:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="a966b-130">Condition : ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-130">Condition:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="a966b-131">Condition : FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="a966b-131">Condition:FlaggedForAction</span></span>
    
- <span data-ttu-id="a966b-132">Condition : FromAddresses</span><span class="sxs-lookup"><span data-stu-id="a966b-132">Condition:FromAddresses</span></span>
    
- <span data-ttu-id="a966b-133">Condition : FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="a966b-133">Condition:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="a966b-134">Condition : HasAttachments</span><span class="sxs-lookup"><span data-stu-id="a966b-134">Condition:HasAttachments</span></span>
    
- <span data-ttu-id="a966b-135">Condition : importance</span><span class="sxs-lookup"><span data-stu-id="a966b-135">Condition:Importance</span></span>
    
- <span data-ttu-id="a966b-136">Condition : IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="a966b-136">Condition:IsApprovalRequest</span></span>
    
- <span data-ttu-id="a966b-137">Condition : IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="a966b-137">Condition:IsAutomaticForward</span></span>
    
- <span data-ttu-id="a966b-138">Condition : IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="a966b-138">Condition:IsAutomaticReply</span></span>
    
- <span data-ttu-id="a966b-139">Condition : IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="a966b-139">Condition:IsEncrypted</span></span>
    
- <span data-ttu-id="a966b-140">Condition : IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a966b-140">Condition:IsMeetingRequest</span></span>
    
- <span data-ttu-id="a966b-141">Condition : IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="a966b-141">Condition:IsMeetingResponse</span></span>
    
- <span data-ttu-id="a966b-142">Condition : IsNDR</span><span class="sxs-lookup"><span data-stu-id="a966b-142">Condition:IsNDR</span></span>
    
- <span data-ttu-id="a966b-143">Condition : IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="a966b-143">Condition:IsPermissionControlled</span></span>
    
- <span data-ttu-id="a966b-144">Condition : IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="a966b-144">Condition:IsReadReceipt</span></span>
    
- <span data-ttu-id="a966b-145">Condition : IsSigned</span><span class="sxs-lookup"><span data-stu-id="a966b-145">Condition:IsSigned</span></span>
    
- <span data-ttu-id="a966b-146">Condition : IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="a966b-146">Condition:IsVoicemail</span></span>
    
- <span data-ttu-id="a966b-147">Condition : ItemClasses</span><span class="sxs-lookup"><span data-stu-id="a966b-147">Condition:ItemClasses</span></span>
    
- <span data-ttu-id="a966b-148">Condition : MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="a966b-148">Condition:MessageClassifications</span></span>
    
- <span data-ttu-id="a966b-149">Condition : NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="a966b-149">Condition:NotSentToMe</span></span>
    
- <span data-ttu-id="a966b-150">Condition : SentCcMe</span><span class="sxs-lookup"><span data-stu-id="a966b-150">Condition:SentCcMe</span></span>
    
- <span data-ttu-id="a966b-151">Condition : SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="a966b-151">Condition:SentOnlyToMe</span></span>
    
- <span data-ttu-id="a966b-152">Condition : SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="a966b-152">Condition:SentToAddresses</span></span>
    
- <span data-ttu-id="a966b-153">Condition : SentToMe</span><span class="sxs-lookup"><span data-stu-id="a966b-153">Condition:SentToMe</span></span>
    
- <span data-ttu-id="a966b-154">Condition : SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="a966b-154">Condition:SentToOrCcMe</span></span>
    
- <span data-ttu-id="a966b-155">Condition : sensibilité</span><span class="sxs-lookup"><span data-stu-id="a966b-155">Condition:Sensitivity</span></span>
    
- <span data-ttu-id="a966b-156">Condition : WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="a966b-156">Condition:WithinDateRange</span></span>
    
- <span data-ttu-id="a966b-157">Condition : WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="a966b-157">Condition:WithinSizeRange</span></span>
    
- <span data-ttu-id="a966b-158">Exception : Categories</span><span class="sxs-lookup"><span data-stu-id="a966b-158">Exception:Categories</span></span>
    
- <span data-ttu-id="a966b-159">Exception : ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-159">Exception:ContainsBodyStrings</span></span>
    
- <span data-ttu-id="a966b-160">Exception : ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-160">Exception:ContainsHeaderStrings</span></span>
    
- <span data-ttu-id="a966b-161">Exception : ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-161">Exception:ContainsRecipientStrings</span></span>
    
- <span data-ttu-id="a966b-162">Exception : ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-162">Exception:ContainsSenderStrings</span></span>
    
- <span data-ttu-id="a966b-163">Exception : ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-163">Exception:ContainsSubjectOrBodyStrings</span></span>
    
- <span data-ttu-id="a966b-164">Exception : ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="a966b-164">Exception:ContainsSubjectStrings</span></span>
    
- <span data-ttu-id="a966b-165">Exception : FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="a966b-165">Exception:FlaggedForAction</span></span>
    
- <span data-ttu-id="a966b-166">Exception : FromAddresses</span><span class="sxs-lookup"><span data-stu-id="a966b-166">Exception:FromAddresses</span></span>
    
- <span data-ttu-id="a966b-167">Exception : FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="a966b-167">Exception:FromConnectedAccounts</span></span>
    
- <span data-ttu-id="a966b-168">Exception : HasAttachments</span><span class="sxs-lookup"><span data-stu-id="a966b-168">Exception:HasAttachments</span></span>
    
- <span data-ttu-id="a966b-169">Exception : importance</span><span class="sxs-lookup"><span data-stu-id="a966b-169">Exception:Importance</span></span>
    
- <span data-ttu-id="a966b-170">Exception : IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="a966b-170">Exception:IsApprovalRequest</span></span>
    
- <span data-ttu-id="a966b-171">Exception : IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="a966b-171">Exception:IsAutomaticForward</span></span>
    
- <span data-ttu-id="a966b-172">Exception : IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="a966b-172">Exception:IsAutomaticReply</span></span>
    
- <span data-ttu-id="a966b-173">Exception : IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="a966b-173">Exception:IsEncrypted</span></span>
    
- <span data-ttu-id="a966b-174">Exception : IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a966b-174">Exception:IsMeetingRequest</span></span>
    
- <span data-ttu-id="a966b-175">Exception : IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="a966b-175">Exception:IsMeetingResponse</span></span>
    
- <span data-ttu-id="a966b-176">Exception : IsNDR</span><span class="sxs-lookup"><span data-stu-id="a966b-176">Exception:IsNDR</span></span>
    
- <span data-ttu-id="a966b-177">Exception : IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="a966b-177">Exception:IsPermissionControlled</span></span>
    
- <span data-ttu-id="a966b-178">Exception : IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="a966b-178">Exception:IsReadReceipt</span></span>
    
- <span data-ttu-id="a966b-179">Exception : IsSigned</span><span class="sxs-lookup"><span data-stu-id="a966b-179">Exception:IsSigned</span></span>
    
- <span data-ttu-id="a966b-180">Exception : IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="a966b-180">Exception:IsVoicemail</span></span>
    
- <span data-ttu-id="a966b-181">Exception : ItemClasses</span><span class="sxs-lookup"><span data-stu-id="a966b-181">Exception:ItemClasses</span></span>
    
- <span data-ttu-id="a966b-182">Exception : MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="a966b-182">Exception:MessageClassifications</span></span>
    
- <span data-ttu-id="a966b-183">Exception : NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="a966b-183">Exception:NotSentToMe</span></span>
    
- <span data-ttu-id="a966b-184">Exception : SentCcMe</span><span class="sxs-lookup"><span data-stu-id="a966b-184">Exception:SentCcMe</span></span>
    
- <span data-ttu-id="a966b-185">Exception : SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="a966b-185">Exception:SentOnlyToMe</span></span>
    
- <span data-ttu-id="a966b-186">Exception : SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="a966b-186">Exception:SentToAddresses</span></span>
    
- <span data-ttu-id="a966b-187">Exception : SentToMe</span><span class="sxs-lookup"><span data-stu-id="a966b-187">Exception:SentToMe</span></span>
    
- <span data-ttu-id="a966b-188">Exception : SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="a966b-188">Exception:SentToOrCcMe</span></span>
    
- <span data-ttu-id="a966b-189">Exception : Sensitivity</span><span class="sxs-lookup"><span data-stu-id="a966b-189">Exception:Sensitivity</span></span>
    
- <span data-ttu-id="a966b-190">Exception : WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="a966b-190">Exception:WithinDateRange</span></span>
    
- <span data-ttu-id="a966b-191">Exception : WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="a966b-191">Exception:WithinSizeRange</span></span>
    
- <span data-ttu-id="a966b-192">Action : AssignCategories</span><span class="sxs-lookup"><span data-stu-id="a966b-192">Action:AssignCategories</span></span>
    
- <span data-ttu-id="a966b-193">Action : CopyToFolder,</span><span class="sxs-lookup"><span data-stu-id="a966b-193">Action:CopyToFolder</span></span>
    
- <span data-ttu-id="a966b-194">Action : supprimer</span><span class="sxs-lookup"><span data-stu-id="a966b-194">Action:Delete</span></span>
    
- <span data-ttu-id="a966b-195">Action : ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="a966b-195">Action:ForwardAsAttachmentToRecipients</span></span>
    
- <span data-ttu-id="a966b-196">Action : ForwardToRecipients</span><span class="sxs-lookup"><span data-stu-id="a966b-196">Action:ForwardToRecipients</span></span>
    
- <span data-ttu-id="a966b-197">Action : MarkImportance</span><span class="sxs-lookup"><span data-stu-id="a966b-197">Action:MarkImportance</span></span>
    
- <span data-ttu-id="a966b-198">Action : MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="a966b-198">Action:MarkAsRead</span></span>
    
- <span data-ttu-id="a966b-199">Action : MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="a966b-199">Action:MoveToFolder</span></span>
    
- <span data-ttu-id="a966b-200">Action : PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="a966b-200">Action:PermanentDelete</span></span>
    
- <span data-ttu-id="a966b-201">Action : RedirectToRecipients</span><span class="sxs-lookup"><span data-stu-id="a966b-201">Action:RedirectToRecipients</span></span>
    
- <span data-ttu-id="a966b-202">Action : SendSMSAlertToRecipients</span><span class="sxs-lookup"><span data-stu-id="a966b-202">Action:SendSMSAlertToRecipients</span></span>
    
- <span data-ttu-id="a966b-203">Action : ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="a966b-203">Action:ServerReplyWithMessage</span></span>
    
- <span data-ttu-id="a966b-204">Action : StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="a966b-204">Action:StopProcessingRules</span></span>
    
- <span data-ttu-id="a966b-205">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="a966b-205">IsEnabled</span></span>
    
- <span data-ttu-id="a966b-206">IsInError</span><span class="sxs-lookup"><span data-stu-id="a966b-206">IsInError</span></span>
    
- <span data-ttu-id="a966b-207">Conditions</span><span class="sxs-lookup"><span data-stu-id="a966b-207">Conditions</span></span>
    
- <span data-ttu-id="a966b-208">Exceptions</span><span class="sxs-lookup"><span data-stu-id="a966b-208">Exceptions</span></span>
    
## <a name="remarks"></a><span data-ttu-id="a966b-209">Remarques</span><span class="sxs-lookup"><span data-stu-id="a966b-209">Remarks</span></span>

<span data-ttu-id="a966b-210">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a966b-210">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a966b-211">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a966b-211">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a966b-212">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a966b-212">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a966b-213">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a966b-213">Schema Name</span></span>  <br/> |<span data-ttu-id="a966b-214">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a966b-214">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a966b-215">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a966b-215">Validation File</span></span>  <br/> |<span data-ttu-id="a966b-216">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a966b-216">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a966b-217">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a966b-217">Can be Empty</span></span>  <br/> |<span data-ttu-id="a966b-218">False</span><span class="sxs-lookup"><span data-stu-id="a966b-218">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a966b-219">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a966b-219">See also</span></span>



- [<span data-ttu-id="a966b-220">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a966b-220">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

