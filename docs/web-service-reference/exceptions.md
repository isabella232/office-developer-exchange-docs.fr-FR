---
title: Exceptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exceptions
api_type:
- schema
ms.assetid: 7cd63ac2-3441-4ed4-915b-6f90af4b28fc
description: L’élément exceptions identifie les exceptions qui représentent toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.
ms.openlocfilehash: 1afc2980391ee588f9b9b813b87c2c699de3a6df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463355"
---
# <a name="exceptions"></a><span data-ttu-id="8f009-103">Exceptions</span><span class="sxs-lookup"><span data-stu-id="8f009-103">Exceptions</span></span>

<span data-ttu-id="8f009-104">L’élément **exceptions** identifie les exceptions qui représentent toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="8f009-104">The **Exceptions** element identifies the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span> 
  
```XML
<Conditions>
   <Categories/>
   <ContainsBodyStrings/>
   <ContainsHeaderStrings/>
   <ContainsRecipientStrings/>
   <ContainsSenderStrings/>
   <ContainsSubjectOrBodyStrings/>
   <ContainsSubjectStrings/>
   <FlaggedForAction/>
   <FromAddresses/>
   <FromConnectedAccounts/>
   <HasAttachments/>
   <Importance/>
   <IsApprovalRequest/>
   <IsAutomaticForward/>
   <IsAutomaticReply/>
   <IsEncrypted/>
   <IsMeetingRequest/>
   <IsMeetingResponse/>
   <IsNDR/>
   <IsPermissionControlled/>
   <IsReadReceipt/>
   <IsSigned/>
   <IsVoicemail/>
   <ItemClasses/>
   <MessageClassifications/>
   <NotSentToMe/>
   <SentCcMe/>
   <SentOnlyToMe/>
   <SentToAddresses/>
   <SentToMe/>
   <SentToOrCcMe/>
   <Sensitivity/>
   <WithinDateRange/>
   <WithinSizeRange/>
</Conditions>
```

 <span data-ttu-id="8f009-105">**RulePredicatesType**</span><span class="sxs-lookup"><span data-stu-id="8f009-105">**RulePredicatesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f009-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8f009-106">Attributes and elements</span></span>

<span data-ttu-id="8f009-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8f009-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f009-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8f009-108">Attributes</span></span>

<span data-ttu-id="8f009-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8f009-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f009-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8f009-110">Child elements</span></span>

|<span data-ttu-id="8f009-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8f009-111">**Element**</span></span>|<span data-ttu-id="8f009-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8f009-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f009-113">Catégories</span><span class="sxs-lookup"><span data-stu-id="8f009-113">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8f009-114">Contient les catégories qui doivent être appliquées à un message entrant afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-114">Contains the categories that must be applied to an incoming message in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-115">ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="8f009-115">ContainsBodyStrings</span></span>](containsbodystrings.md) <br/> |<span data-ttu-id="8f009-116">Indique les chaînes qui doivent apparaître dans le corps des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-116">Indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-117">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="8f009-117">ContainsHeaderStrings</span></span>](containsheaderstrings.md) <br/> |<span data-ttu-id="8f009-118">Indicaqtes les chaînes qui doivent apparaître dans les en-têtes des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-118">Indicaqtes the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-119">ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="8f009-119">ContainsRecipientStrings</span></span>](containsrecipientstrings.md) <br/> |<span data-ttu-id="8f009-120">Indique les chaînes qui doivent apparaître dans les propriétés **ToRecipients** ou **CCRecipients** des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-120">Indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-121">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="8f009-121">ContainsSenderStrings</span></span>](containssenderstrings.md) <br/> |<span data-ttu-id="8f009-122">Indique les chaînes qui doivent apparaître dans la propriété **from** des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-122">Indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-123">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="8f009-123">ContainsSubjectOrBodyStrings</span></span>](containssubjectorbodystrings.md) <br/> |<span data-ttu-id="8f009-124">Indique les chaînes qui doivent apparaître dans le corps ou l’objet des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-124">Indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-125">ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="8f009-125">ContainsSubjectStrings</span></span>](containssubjectstrings.md) <br/> |<span data-ttu-id="8f009-126">Indique les chaînes qui doivent apparaître dans l’objet des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-126">Indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-127">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="8f009-127">FlaggedForAction</span></span>](flaggedforaction.md) <br/> |<span data-ttu-id="8f009-128">Spécifie l’indicateur de la valeur d’action qui doit apparaître dans les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-128">Specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-129">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="8f009-129">FromAddresses</span></span>](fromaddresses.md) <br/> |<span data-ttu-id="8f009-130">Indique les adresses de messagerie à partir desquelles les messages entrants doivent être envoyés pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-130">Indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-131">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="8f009-131">FromConnectedAccounts</span></span>](fromconnectedaccounts.md) <br/> |<span data-ttu-id="8f009-132">Représente les noms de compte de messagerie à partir desquels les messages entrants doivent être regroupés pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-132">Represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-133">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="8f009-133">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="8f009-134">Indique si les messages entrants doivent contenir des pièces jointes afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-134">Indicates whether incoming messages have to have attachments in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-135">Importance</span><span class="sxs-lookup"><span data-stu-id="8f009-135">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="8f009-136">Spécifie l’importance qui est marquée sur les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-136">Specifies the importance that is stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-137">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="8f009-137">IsApprovalRequest</span></span>](isapprovalrequest.md) <br/> |<span data-ttu-id="8f009-138">Indique si les messages entrants doivent être des demandes d’approbation afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-138">Indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-139">IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="8f009-139">IsAutomaticForward</span></span>](isautomaticforward.md) <br/> |<span data-ttu-id="8f009-140">Indique si les messages entrants doivent être des transferts automatiques afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-140">Indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-141">IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="8f009-141">IsAutomaticReply</span></span>](isautomaticreply.md) <br/> |<span data-ttu-id="8f009-142">Indique si les messages entrants doivent être des réponses automatiques afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-142">Indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-143">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="8f009-143">IsEncrypted</span></span>](isencrypted.md) <br/> |<span data-ttu-id="8f009-144">Indique si les messages entrants doivent être chiffrés S/MIME afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-144">Indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-145">IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8f009-145">IsMeetingRequest</span></span>](ismeetingrequest.md) <br/> |<span data-ttu-id="8f009-146">Indique si les messages entrants doivent être des demandes de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-146">Indicates whether incoming messages must be meeting requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-147">IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="8f009-147">IsMeetingResponse</span></span>](ismeetingresponse.md) <br/> |<span data-ttu-id="8f009-148">Indique si les messages entrants doivent être des réponses à la demande de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-148">Indicates whether incoming messages must be meeting responses in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-149">IsNDR</span><span class="sxs-lookup"><span data-stu-id="8f009-149">IsNDR</span></span>](isndr.md) <br/> |<span data-ttu-id="8f009-150">Indique si les messages entrants doivent être des notifications d’échec de remise pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-150">Indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-151">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="8f009-151">IsPermissionControlled</span></span>](ispermissioncontrolled.md) <br/> |<span data-ttu-id="8f009-152">Indique si les messages entrants doivent être contrôlés par des autorisations (protection RMS) afin que la condition ou l’exception s’applique</span><span class="sxs-lookup"><span data-stu-id="8f009-152">Indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply</span></span>  <br/> |
|[<span data-ttu-id="8f009-153">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="8f009-153">IsReadReceipt</span></span>](isreadreceipt.md) <br/> |<span data-ttu-id="8f009-154">Indique si les messages entrants doivent être lus en confirmation de lecture afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-154">Indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-155">IsSigned</span><span class="sxs-lookup"><span data-stu-id="8f009-155">IsSigned</span></span>](issigned.md) <br/> |<span data-ttu-id="8f009-156">Indique si les messages entrants doivent être S/MIME signés pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-156">Indicates whether incoming messages must be S/MIME signed in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-157">IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="8f009-157">IsVoicemail</span></span>](isvoicemail.md) <br/> |<span data-ttu-id="8f009-158">Indique si les messages entrants doivent être des messages vocaux afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-158">Indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-159">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="8f009-159">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="8f009-160">Représente les classes d’éléments qui doivent être marquées sur les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-160">Represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-161">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="8f009-161">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="8f009-162">Représente les classifications de message qui doivent être marquées sur les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-162">Represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-163">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="8f009-163">NotSentToMe</span></span>](notsenttome.md) <br/> |<span data-ttu-id="8f009-164">Indique si le propriétaire de la boîte aux lettres ne doit pas être dans la propriété **ToRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-164">Indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-165">SentCcMe</span><span class="sxs-lookup"><span data-stu-id="8f009-165">SentCcMe</span></span>](sentccme.md) <br/> |<span data-ttu-id="8f009-166">Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **CCRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-166">Indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-167">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="8f009-167">SentOnlyToMe</span></span>](sentonlytome.md) <br/> |<span data-ttu-id="8f009-168">Indique si le propriétaire de la boîte aux lettres doit être le seul dans la propriété **ToRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-168">Indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-169">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="8f009-169">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="8f009-170">Indique les adresses de messagerie auxquelles les messages entrants doivent avoir été envoyés pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-170">Indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-171">SentToMe</span><span class="sxs-lookup"><span data-stu-id="8f009-171">SentToMe</span></span>](senttome.md) <br/> |<span data-ttu-id="8f009-172">Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **ToRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-172">Indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-173">SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="8f009-173">SentToOrCcMe</span></span>](senttoorccme.md) <br/> |<span data-ttu-id="8f009-174">Indique si le propriétaire de la boîte aux lettres doit se trouver dans une propriété **ToRecipients** ou **CCRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-174">Indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-175">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="8f009-175">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="8f009-176">Indique la sensibilité qui doit être marquée sur les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-176">Indicates the sensitivity that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-177">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="8f009-177">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="8f009-178">Spécifie la plage de dates au cours de laquelle les messages entrants doivent avoir été reçus afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-178">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8f009-179">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="8f009-179">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="8f009-180">Spécifie les tailles minimale et maximale que les messages entrants doivent être pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="8f009-180">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8f009-181">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8f009-181">Parent elements</span></span>

|<span data-ttu-id="8f009-182">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8f009-182">**Element**</span></span>|<span data-ttu-id="8f009-183">**Description**</span><span class="sxs-lookup"><span data-stu-id="8f009-183">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f009-184">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="8f009-184">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="8f009-185">Contient une seule règle et représente une règle dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8f009-185">Contains a single rule and represents a rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8f009-186">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8f009-186">Text value</span></span>

<span data-ttu-id="8f009-187">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8f009-187">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8f009-188">Remarques</span><span class="sxs-lookup"><span data-stu-id="8f009-188">Remarks</span></span>

<span data-ttu-id="8f009-189">Les prédicats de règle sont utilisés en tant que conditions de règle ou exceptions.</span><span class="sxs-lookup"><span data-stu-id="8f009-189">The rule predicates are used as rule conditions or exceptions.</span></span>
  
<span data-ttu-id="8f009-190">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8f009-190">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f009-191">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8f009-191">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f009-192">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8f009-192">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8f009-193">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8f009-193">Schema Name</span></span>  <br/> |<span data-ttu-id="8f009-194">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8f009-194">Types schema</span></span>  <br/> |
|<span data-ttu-id="8f009-195">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8f009-195">Validation File</span></span>  <br/> |<span data-ttu-id="8f009-196">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8f009-196">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8f009-197">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8f009-197">Can be Empty</span></span>  <br/> |<span data-ttu-id="8f009-198">True</span><span class="sxs-lookup"><span data-stu-id="8f009-198">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8f009-199">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8f009-199">See also</span></span>



[<span data-ttu-id="8f009-200">Conditions</span><span class="sxs-lookup"><span data-stu-id="8f009-200">Conditions</span></span>](conditions.md)


- [<span data-ttu-id="8f009-201">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8f009-201">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

