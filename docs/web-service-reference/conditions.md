---
title: Conditions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conditions
api_type:
- schema
ms.assetid: f049a48c-9585-43f7-8549-0b8cb19a5eea
description: L’élément Conditions identifie les conditions qui, lorsque remplies, déclenchent des actions de règle d’une règle.
ms.openlocfilehash: f66777e82892122c4c7dac45bdef3c42f5c4a577
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755534"
---
# <a name="conditions"></a><span data-ttu-id="8fbee-103">Conditions</span><span class="sxs-lookup"><span data-stu-id="8fbee-103">Conditions</span></span>

<span data-ttu-id="8fbee-104">L’élément **Conditions** identifie les conditions qui, lorsque remplies, déclenchent des actions de règle d’une règle.</span><span class="sxs-lookup"><span data-stu-id="8fbee-104">The **Conditions** element identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span> 
  
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

 <span data-ttu-id="8fbee-105">**RulePredicatesType**</span><span class="sxs-lookup"><span data-stu-id="8fbee-105">**RulePredicatesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8fbee-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8fbee-106">Attributes and elements</span></span>

<span data-ttu-id="8fbee-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8fbee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fbee-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8fbee-108">Attributes</span></span>

<span data-ttu-id="8fbee-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8fbee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8fbee-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8fbee-110">Child elements</span></span>

|<span data-ttu-id="8fbee-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8fbee-111">**Element**</span></span>|<span data-ttu-id="8fbee-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8fbee-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fbee-113">Categories</span><span class="sxs-lookup"><span data-stu-id="8fbee-113">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8fbee-114">Contient les catégories qui doivent être appliquées à un message entrant afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-114">Contains the categories that must be applied to an incoming message in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-115">ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="8fbee-115">ContainsBodyStrings</span></span>](containsbodystrings.md) <br/> |<span data-ttu-id="8fbee-116">Indique les chaînes qui doivent apparaître dans le corps des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-116">Indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-117">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="8fbee-117">ContainsHeaderStrings</span></span>](containsheaderstrings.md) <br/> |<span data-ttu-id="8fbee-118">Indique les chaînes qui doivent apparaître dans les en-têtes des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-118">Indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-119">ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="8fbee-119">ContainsRecipientStrings</span></span>](containsrecipientstrings.md) <br/> |<span data-ttu-id="8fbee-120">Indique les chaînes qui doivent apparaître dans les **ToRecipients** **CcRecipients** propriétés ou des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-120">Indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-121">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="8fbee-121">ContainsSenderStrings</span></span>](containssenderstrings.md) <br/> |<span data-ttu-id="8fbee-122">Indique les chaînes qui doivent apparaître dans la propriété **From** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-122">Indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-123">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="8fbee-123">ContainsSubjectOrBodyStrings</span></span>](containssubjectorbodystrings.md) <br/> |<span data-ttu-id="8fbee-124">Indique les chaînes qui doivent apparaître dans le corps ou l’objet des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-124">Indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-125">ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="8fbee-125">ContainsSubjectStrings</span></span>](containssubjectstrings.md) <br/> |<span data-ttu-id="8fbee-126">Indique les chaînes qui doivent apparaître dans l’objet des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-126">Indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-127">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="8fbee-127">FlaggedForAction</span></span>](flaggedforaction.md) <br/> |<span data-ttu-id="8fbee-128">Spécifie l’indicateur pour la valeur d’action qui doit apparaître dans les messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-128">Specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-129">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="8fbee-129">FromAddresses</span></span>](fromaddresses.md) <br/> |<span data-ttu-id="8fbee-130">Indique les adresses de messagerie à partir de laquelle les messages entrants doivent être envoyés afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-130">Indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-131">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="8fbee-131">FromConnectedAccounts</span></span>](fromconnectedaccounts.md) <br/> |<span data-ttu-id="8fbee-132">Représente les noms de compte de messagerie à partir de laquelle les messages entrants doivent avoir été agrégées afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-132">Represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-133">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="8fbee-133">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="8fbee-134">Indique si les messages entrants ont pour que les pièces jointes afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-134">Indicates whether incoming messages have to have attachments in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-135">Importance</span><span class="sxs-lookup"><span data-stu-id="8fbee-135">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="8fbee-136">Spécifie l’importance est marqué sur les messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-136">Specifies the importance that is stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-137">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="8fbee-137">IsApprovalRequest</span></span>](isapprovalrequest.md) <br/> |<span data-ttu-id="8fbee-138">Indique si les messages entrants doivent être des demandes d’approbation afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-138">Indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-139">IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="8fbee-139">IsAutomaticForward</span></span>](isautomaticforward.md) <br/> |<span data-ttu-id="8fbee-140">Indique si les messages entrants doivent être des transferts automatiques afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-140">Indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-141">IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="8fbee-141">IsAutomaticReply</span></span>](isautomaticreply.md) <br/> |<span data-ttu-id="8fbee-142">Indique si les messages entrants doivent être des réponses automatiques afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-142">Indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-143">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="8fbee-143">IsEncrypted</span></span>](isencrypted.md) <br/> |<span data-ttu-id="8fbee-144">Indique si les messages entrants doivent être chiffré afin que l’exception ou la condition à appliquer S/MIME.</span><span class="sxs-lookup"><span data-stu-id="8fbee-144">Indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-145">IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8fbee-145">IsMeetingRequest</span></span>](ismeetingrequest.md) <br/> |<span data-ttu-id="8fbee-146">Indique si les messages entrants doivent être les demandes de réunion dans l’ordre de l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-146">Indicates whether incoming messages must be meeting requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-147">IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="8fbee-147">IsMeetingResponse</span></span>](ismeetingresponse.md) <br/> |<span data-ttu-id="8fbee-148">Indique si les messages entrants doivent être réponses de réunion afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-148">Indicates whether incoming messages must be meeting responses in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-149">IsNDR</span><span class="sxs-lookup"><span data-stu-id="8fbee-149">IsNDR</span></span>](isndr.md) <br/> |<span data-ttu-id="8fbee-150">Indique si les messages entrants doivent être des rapports de non remise (NDR) afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-150">Indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-151">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="8fbee-151">IsPermissionControlled</span></span>](ispermissioncontrolled.md) <br/> |<span data-ttu-id="8fbee-152">Indique si les messages entrants doivent être sous contrôlée de l’autorisation (protégés par RMS) afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-152">Indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-153">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="8fbee-153">IsReadReceipt</span></span>](isreadreceipt.md) <br/> |<span data-ttu-id="8fbee-154">Indique si les messages entrants doivent être des confirmations de lecture afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-154">Indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-155">IsSigned</span><span class="sxs-lookup"><span data-stu-id="8fbee-155">IsSigned</span></span>](issigned.md) <br/> |<span data-ttu-id="8fbee-156">Indique si les messages entrants doivent être signés S/MIME afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-156">Indicates whether incoming messages must be S/MIME signed in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-157">IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="8fbee-157">IsVoicemail</span></span>](isvoicemail.md) <br/> |<span data-ttu-id="8fbee-158">Indique si les messages entrants doivent être des messages vocaux afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-158">Indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-159">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="8fbee-159">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="8fbee-160">Représente les classes d’élément qui doivent être marqués sur les messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-160">Represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-161">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="8fbee-161">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="8fbee-162">Représente les classifications de messages qui doivent être marquées sur les messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-162">Represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-163">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="8fbee-163">NotSentToMe</span></span>](notsenttome.md) <br/> |<span data-ttu-id="8fbee-164">Indique si le propriétaire de la boîte aux lettres ne doit pas être dans la propriété **ToRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-164">Indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-165">SentCcMe</span><span class="sxs-lookup"><span data-stu-id="8fbee-165">SentCcMe</span></span>](sentccme.md) <br/> |<span data-ttu-id="8fbee-166">Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **CcRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-166">Indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-167">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="8fbee-167">SentOnlyToMe</span></span>](sentonlytome.md) <br/> |<span data-ttu-id="8fbee-168">Indique si le propriétaire de la boîte aux lettres doit être le seul à la propriété **ToRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-168">Indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-169">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="8fbee-169">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="8fbee-170">Indique les adresses de messagerie dont les messages entrants ont été envoyées aux afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-170">Indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-171">SentToMe</span><span class="sxs-lookup"><span data-stu-id="8fbee-171">SentToMe</span></span>](senttome.md) <br/> |<span data-ttu-id="8fbee-172">Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **ToRecipients** des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-172">Indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-173">SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="8fbee-173">SentToOrCcMe</span></span>](senttoorccme.md) <br/> |<span data-ttu-id="8fbee-174">Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété un **CcRecipients** **ToRecipients** ou des messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-174">Indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-175">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="8fbee-175">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="8fbee-176">Indique le critère de diffusion qui doit être marqué sur les messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-176">Indicates the sensitivity that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-177">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="8fbee-177">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="8fbee-178">Spécifie la plage de dates dans laquelle les messages entrants ont reçue dans l’ordre de l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-178">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="8fbee-179">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="8fbee-179">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="8fbee-180">Spécifie les tailles minimales et maximales des messages entrants doivent être dans l’ordre de l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="8fbee-180">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8fbee-181">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8fbee-181">Parent elements</span></span>

|<span data-ttu-id="8fbee-182">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8fbee-182">**Element**</span></span>|<span data-ttu-id="8fbee-183">**Description**</span><span class="sxs-lookup"><span data-stu-id="8fbee-183">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fbee-184">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="8fbee-184">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="8fbee-185">Contient une règle unique et représente une règle de boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8fbee-185">Contains a single rule and represents a rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8fbee-186">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8fbee-186">Text value</span></span>

<span data-ttu-id="8fbee-187">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8fbee-187">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8fbee-188">Remarques</span><span class="sxs-lookup"><span data-stu-id="8fbee-188">Remarks</span></span>

<span data-ttu-id="8fbee-189">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8fbee-189">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8fbee-190">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8fbee-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8fbee-191">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8fbee-191">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8fbee-192">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8fbee-192">Schema Name</span></span>  <br/> |<span data-ttu-id="8fbee-193">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8fbee-193">Types schema</span></span>  <br/> |
|<span data-ttu-id="8fbee-194">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8fbee-194">Validation File</span></span>  <br/> |<span data-ttu-id="8fbee-195">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8fbee-195">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8fbee-196">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8fbee-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="8fbee-197">True</span><span class="sxs-lookup"><span data-stu-id="8fbee-197">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8fbee-198">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8fbee-198">See also</span></span>



[<span data-ttu-id="8fbee-199">Exceptions</span><span class="sxs-lookup"><span data-stu-id="8fbee-199">Exceptions</span></span>](exceptions.md)


- [<span data-ttu-id="8fbee-200">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8fbee-200">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

