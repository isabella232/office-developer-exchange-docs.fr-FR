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
description: L’élément conditions identifie les conditions qui, lorsqu’elles sont remplies, déclencheront les actions de règle pour une règle.
ms.openlocfilehash: 2c6b4794a87cca79b4c723197b57360ad0ff973d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463201"
---
# <a name="conditions"></a><span data-ttu-id="bb09e-103">Conditions</span><span class="sxs-lookup"><span data-stu-id="bb09e-103">Conditions</span></span>

<span data-ttu-id="bb09e-104">L’élément **conditions** identifie les conditions qui, lorsqu’elles sont remplies, déclencheront les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="bb09e-104">The **Conditions** element identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span> 
  
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

 <span data-ttu-id="bb09e-105">**RulePredicatesType**</span><span class="sxs-lookup"><span data-stu-id="bb09e-105">**RulePredicatesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb09e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bb09e-106">Attributes and elements</span></span>

<span data-ttu-id="bb09e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bb09e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb09e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bb09e-108">Attributes</span></span>

<span data-ttu-id="bb09e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bb09e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb09e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bb09e-110">Child elements</span></span>

|<span data-ttu-id="bb09e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bb09e-111">**Element**</span></span>|<span data-ttu-id="bb09e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="bb09e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb09e-113">Catégories</span><span class="sxs-lookup"><span data-stu-id="bb09e-113">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bb09e-114">Contient les catégories qui doivent être appliquées à un message entrant afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-114">Contains the categories that must be applied to an incoming message in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-115">ContainsBodyStrings</span><span class="sxs-lookup"><span data-stu-id="bb09e-115">ContainsBodyStrings</span></span>](containsbodystrings.md) <br/> |<span data-ttu-id="bb09e-116">Indique les chaînes qui doivent apparaître dans le corps des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-116">Indicates the strings that must appear in the body of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-117">ContainsHeaderStrings</span><span class="sxs-lookup"><span data-stu-id="bb09e-117">ContainsHeaderStrings</span></span>](containsheaderstrings.md) <br/> |<span data-ttu-id="bb09e-118">Indique les chaînes qui doivent apparaître dans les en-têtes des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-118">Indicates the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-119">ContainsRecipientStrings</span><span class="sxs-lookup"><span data-stu-id="bb09e-119">ContainsRecipientStrings</span></span>](containsrecipientstrings.md) <br/> |<span data-ttu-id="bb09e-120">Indique les chaînes qui doivent apparaître dans les propriétés **ToRecipients** ou **CCRecipients** des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-120">Indicates the strings that must appear in either the **ToRecipients** or **CcRecipients** properties of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-121">ContainsSenderStrings</span><span class="sxs-lookup"><span data-stu-id="bb09e-121">ContainsSenderStrings</span></span>](containssenderstrings.md) <br/> |<span data-ttu-id="bb09e-122">Indique les chaînes qui doivent apparaître dans la propriété **from** des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-122">Indicates the strings that must appear in the **From** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-123">ContainsSubjectOrBodyStrings</span><span class="sxs-lookup"><span data-stu-id="bb09e-123">ContainsSubjectOrBodyStrings</span></span>](containssubjectorbodystrings.md) <br/> |<span data-ttu-id="bb09e-124">Indique les chaînes qui doivent apparaître dans le corps ou l’objet des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-124">Indicates the strings that must appear in either the body or the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-125">ContainsSubjectStrings</span><span class="sxs-lookup"><span data-stu-id="bb09e-125">ContainsSubjectStrings</span></span>](containssubjectstrings.md) <br/> |<span data-ttu-id="bb09e-126">Indique les chaînes qui doivent apparaître dans l’objet des messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-126">Indicates the strings that must appear in the subject of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-127">FlaggedForAction</span><span class="sxs-lookup"><span data-stu-id="bb09e-127">FlaggedForAction</span></span>](flaggedforaction.md) <br/> |<span data-ttu-id="bb09e-128">Spécifie l’indicateur de la valeur d’action qui doit apparaître dans les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-128">Specifies the flag for action value that must appear on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-129">FromAddresses</span><span class="sxs-lookup"><span data-stu-id="bb09e-129">FromAddresses</span></span>](fromaddresses.md) <br/> |<span data-ttu-id="bb09e-130">Indique les adresses de messagerie à partir desquelles les messages entrants doivent être envoyés pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-130">Indicates the e-mail addresses from which incoming messages must be sent in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-131">FromConnectedAccounts</span><span class="sxs-lookup"><span data-stu-id="bb09e-131">FromConnectedAccounts</span></span>](fromconnectedaccounts.md) <br/> |<span data-ttu-id="bb09e-132">Représente les noms de compte de messagerie à partir desquels les messages entrants doivent être regroupés pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-132">Represents the e-mail account names from which incoming messages have to have been aggregated in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-133">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="bb09e-133">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="bb09e-134">Indique si les messages entrants doivent contenir des pièces jointes afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-134">Indicates whether incoming messages have to have attachments in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-135">Importance</span><span class="sxs-lookup"><span data-stu-id="bb09e-135">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="bb09e-136">Spécifie l’importance qui est marquée sur les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-136">Specifies the importance that is stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-137">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="bb09e-137">IsApprovalRequest</span></span>](isapprovalrequest.md) <br/> |<span data-ttu-id="bb09e-138">Indique si les messages entrants doivent être des demandes d’approbation afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-138">Indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-139">IsAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="bb09e-139">IsAutomaticForward</span></span>](isautomaticforward.md) <br/> |<span data-ttu-id="bb09e-140">Indique si les messages entrants doivent être des transferts automatiques afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-140">Indicates whether incoming messages must be automatic forwards in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-141">IsAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="bb09e-141">IsAutomaticReply</span></span>](isautomaticreply.md) <br/> |<span data-ttu-id="bb09e-142">Indique si les messages entrants doivent être des réponses automatiques afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-142">Indicates whether incoming messages must be automatic replies in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-143">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="bb09e-143">IsEncrypted</span></span>](isencrypted.md) <br/> |<span data-ttu-id="bb09e-144">Indique si les messages entrants doivent être chiffrés S/MIME afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-144">Indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-145">IsMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="bb09e-145">IsMeetingRequest</span></span>](ismeetingrequest.md) <br/> |<span data-ttu-id="bb09e-146">Indique si les messages entrants doivent être des demandes de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-146">Indicates whether incoming messages must be meeting requests in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-147">IsMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="bb09e-147">IsMeetingResponse</span></span>](ismeetingresponse.md) <br/> |<span data-ttu-id="bb09e-148">Indique si les messages entrants doivent être des réponses à la demande de réunion afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-148">Indicates whether incoming messages must be meeting responses in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-149">IsNDR</span><span class="sxs-lookup"><span data-stu-id="bb09e-149">IsNDR</span></span>](isndr.md) <br/> |<span data-ttu-id="bb09e-150">Indique si les messages entrants doivent être des notifications d’échec de remise pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-150">Indicates whether incoming messages must be non-delivery reports (NDRs) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-151">IsPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="bb09e-151">IsPermissionControlled</span></span>](ispermissioncontrolled.md) <br/> |<span data-ttu-id="bb09e-152">Indique si les messages entrants doivent être contrôlés par des autorisations (protection RMS) afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-152">Indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-153">IsReadReceipt</span><span class="sxs-lookup"><span data-stu-id="bb09e-153">IsReadReceipt</span></span>](isreadreceipt.md) <br/> |<span data-ttu-id="bb09e-154">Indique si les messages entrants doivent être lus en confirmation de lecture afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-154">Indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-155">IsSigned</span><span class="sxs-lookup"><span data-stu-id="bb09e-155">IsSigned</span></span>](issigned.md) <br/> |<span data-ttu-id="bb09e-156">Indique si les messages entrants doivent être S/MIME signés pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-156">Indicates whether incoming messages must be S/MIME signed in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-157">IsVoicemail</span><span class="sxs-lookup"><span data-stu-id="bb09e-157">IsVoicemail</span></span>](isvoicemail.md) <br/> |<span data-ttu-id="bb09e-158">Indique si les messages entrants doivent être des messages vocaux afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-158">Indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-159">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="bb09e-159">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="bb09e-160">Représente les classes d’éléments qui doivent être marquées sur les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-160">Represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-161">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="bb09e-161">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="bb09e-162">Représente les classifications de message qui doivent être marquées sur les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-162">Represents the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-163">NotSentToMe</span><span class="sxs-lookup"><span data-stu-id="bb09e-163">NotSentToMe</span></span>](notsenttome.md) <br/> |<span data-ttu-id="bb09e-164">Indique si le propriétaire de la boîte aux lettres ne doit pas être dans la propriété **ToRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-164">Indicates whether the owner of the mailbox must not be in the **ToRecipients** property of the incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-165">SentCcMe</span><span class="sxs-lookup"><span data-stu-id="bb09e-165">SentCcMe</span></span>](sentccme.md) <br/> |<span data-ttu-id="bb09e-166">Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **CCRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-166">Indicates whether the owner of the mailbox has to be in the **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-167">SentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="bb09e-167">SentOnlyToMe</span></span>](sentonlytome.md) <br/> |<span data-ttu-id="bb09e-168">Indique si le propriétaire de la boîte aux lettres doit être le seul dans la propriété **ToRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-168">Indicates whether the owner of the mailbox has to be the only one in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-169">SentToAddresses</span><span class="sxs-lookup"><span data-stu-id="bb09e-169">SentToAddresses</span></span>](senttoaddresses.md) <br/> |<span data-ttu-id="bb09e-170">Indique les adresses de messagerie auxquelles les messages entrants doivent avoir été envoyés pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-170">Indicates the e-mail addresses that incoming messages have to have been sent to in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-171">SentToMe</span><span class="sxs-lookup"><span data-stu-id="bb09e-171">SentToMe</span></span>](senttome.md) <br/> |<span data-ttu-id="bb09e-172">Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **ToRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-172">Indicates whether the owner of the mailbox has to be in the **ToRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-173">SentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="bb09e-173">SentToOrCcMe</span></span>](senttoorccme.md) <br/> |<span data-ttu-id="bb09e-174">Indique si le propriétaire de la boîte aux lettres doit se trouver dans une propriété **ToRecipients** ou **CCRecipients** des messages entrants afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-174">Indicates whether the owner of the mailbox has to be in either a **ToRecipients** or **CcRecipients** property of incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-175">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="bb09e-175">Sensitivity</span></span>](sensitivity.md) <br/> |<span data-ttu-id="bb09e-176">Indique la sensibilité qui doit être marquée sur les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-176">Indicates the sensitivity that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-177">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="bb09e-177">WithinDateRange</span></span>](withindaterange.md) <br/> |<span data-ttu-id="bb09e-178">Spécifie la plage de dates au cours de laquelle les messages entrants doivent avoir été reçus afin que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-178">Specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="bb09e-179">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="bb09e-179">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="bb09e-180">Spécifie les tailles minimale et maximale que les messages entrants doivent être pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="bb09e-180">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bb09e-181">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bb09e-181">Parent elements</span></span>

|<span data-ttu-id="bb09e-182">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bb09e-182">**Element**</span></span>|<span data-ttu-id="bb09e-183">**Description**</span><span class="sxs-lookup"><span data-stu-id="bb09e-183">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb09e-184">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="bb09e-184">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="bb09e-185">Contient une seule règle et représente une règle dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="bb09e-185">Contains a single rule and represents a rule in a user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bb09e-186">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bb09e-186">Text value</span></span>

<span data-ttu-id="bb09e-187">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bb09e-187">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bb09e-188">Remarques</span><span class="sxs-lookup"><span data-stu-id="bb09e-188">Remarks</span></span>

<span data-ttu-id="bb09e-189">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb09e-189">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb09e-190">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bb09e-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb09e-191">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bb09e-191">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bb09e-192">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bb09e-192">Schema Name</span></span>  <br/> |<span data-ttu-id="bb09e-193">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bb09e-193">Types schema</span></span>  <br/> |
|<span data-ttu-id="bb09e-194">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bb09e-194">Validation File</span></span>  <br/> |<span data-ttu-id="bb09e-195">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bb09e-195">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bb09e-196">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bb09e-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="bb09e-197">True</span><span class="sxs-lookup"><span data-stu-id="bb09e-197">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb09e-198">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bb09e-198">See also</span></span>



[<span data-ttu-id="bb09e-199">Exceptions</span><span class="sxs-lookup"><span data-stu-id="bb09e-199">Exceptions</span></span>](exceptions.md)


- [<span data-ttu-id="bb09e-200">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bb09e-200">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

