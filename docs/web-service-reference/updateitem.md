---
title: UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 34643d58-2743-45b0-a08d-bff6dc1da61d
description: L’élément UpdateItem définit une demande de mise à jour d’un élément dans une boîte aux lettres.
ms.openlocfilehash: 43821db58457ffce22be918a7ba6427f57230010
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466569"
---
# <a name="updateitem"></a><span data-ttu-id="1b969-103">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="1b969-103">UpdateItem</span></span>

<span data-ttu-id="1b969-104">L’élément **UpdateItem** définit une demande de mise à jour d’un élément dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1b969-104">The **UpdateItem** element defines a request to update an item in a mailbox.</span></span> 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 <span data-ttu-id="1b969-105">**UpdateItemType**</span><span class="sxs-lookup"><span data-stu-id="1b969-105">**UpdateItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b969-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1b969-106">Attributes and elements</span></span>

<span data-ttu-id="1b969-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1b969-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b969-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1b969-108">Attributes</span></span>

|<span data-ttu-id="1b969-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1b969-109">**Attribute**</span></span>|<span data-ttu-id="1b969-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="1b969-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1b969-111">**ConflictResolution**</span><span class="sxs-lookup"><span data-stu-id="1b969-111">**ConflictResolution**</span></span> <br/> |<span data-ttu-id="1b969-112">Identifie le type de résolution de conflit à essayer pendant une mise à jour.</span><span class="sxs-lookup"><span data-stu-id="1b969-112">Identifies the type of conflict resolution to try during an update.</span></span> <span data-ttu-id="1b969-113">La valeur par défaut est autosolve.</span><span class="sxs-lookup"><span data-stu-id="1b969-113">The default value is AutoResolve.</span></span>  <br/> |
|<span data-ttu-id="1b969-114">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="1b969-114">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="1b969-115">Décrit la façon dont l’élément sera géré après sa mise à jour.</span><span class="sxs-lookup"><span data-stu-id="1b969-115">Describes how the item will be handled after it is updated.</span></span> <span data-ttu-id="1b969-116">L’attribut **MessageDisposition** est requis pour les éléments de message, y compris les messages de réunion, tels que les annulations de réunion, les demandes de réunion et les réponses aux réunions.</span><span class="sxs-lookup"><span data-stu-id="1b969-116">The **MessageDisposition** attribute is required for message items, including meeting messages such as meeting cancellations, meeting requests, and meeting responses.</span></span>  <br/> |
|<span data-ttu-id="1b969-117">**SendMeetingInvitationsOrCancellations**</span><span class="sxs-lookup"><span data-stu-id="1b969-117">**SendMeetingInvitationsOrCancellations**</span></span> <br/> |<span data-ttu-id="1b969-118">Indique comment les mises à jour de réunion sont communiquées après la mise à jour d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="1b969-118">Describes how meeting updates are communicated after a calendar item is updated.</span></span> <span data-ttu-id="1b969-119">Cet attribut est requis pour les éléments de calendrier et les occurrences d’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="1b969-119">This attribute is required for calendar items and calendar item occurrences.</span></span>  <br/> |
|<span data-ttu-id="1b969-120">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="1b969-120">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="1b969-121">Indique si les confirmations de lecture pour l’élément mis à jour doivent être supprimées.</span><span class="sxs-lookup"><span data-stu-id="1b969-121">Indicates whether read receipts for the updated item should be suppressed.</span></span> <span data-ttu-id="1b969-122">Une valeur de texte **true** indique que les confirmations de lecture doivent être supprimées.</span><span class="sxs-lookup"><span data-stu-id="1b969-122">A text value of **true** indicates that read receipts should be suppressed.</span></span> <span data-ttu-id="1b969-123">La valeur **false** indique que les confirmations de lecture seront envoyées à l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="1b969-123">A value of **false** indicates that the read receipts will be sent to the sender.</span></span> <span data-ttu-id="1b969-124">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="1b969-124">This attribute is optional.</span></span>  <br/> <span data-ttu-id="1b969-125">Cet attribut a été introduit dans Exchange Server 2013 SP1.</span><span class="sxs-lookup"><span data-stu-id="1b969-125">This attribute was introduced in Exchange Server 2013 SP1.</span></span>  <br/> |
   
#### <a name="conflictresolution-attribute"></a><span data-ttu-id="1b969-126">Attribut ConflictResolution</span><span class="sxs-lookup"><span data-stu-id="1b969-126">ConflictResolution Attribute</span></span>

|<span data-ttu-id="1b969-127">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1b969-127">**Value**</span></span>|<span data-ttu-id="1b969-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="1b969-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1b969-129">NeverOverwrite</span><span class="sxs-lookup"><span data-stu-id="1b969-129">NeverOverwrite</span></span>  <br/> |<span data-ttu-id="1b969-130">En cas de conflit, l’opération de mise à jour échoue et une erreur est renvoyée.</span><span class="sxs-lookup"><span data-stu-id="1b969-130">If there is a conflict, the update operation fails and an error is returned.</span></span>  <br/> |
|<span data-ttu-id="1b969-131">Autosolve</span><span class="sxs-lookup"><span data-stu-id="1b969-131">AutoResolve</span></span>  <br/> |<span data-ttu-id="1b969-132">L’opération de mise à jour résout automatiquement les conflits.</span><span class="sxs-lookup"><span data-stu-id="1b969-132">The update operation automatically resolves any conflict.</span></span>  <br/> |
|<span data-ttu-id="1b969-133">AlwaysOverwrite</span><span class="sxs-lookup"><span data-stu-id="1b969-133">AlwaysOverwrite</span></span>  <br/> |<span data-ttu-id="1b969-134">En cas de conflit, l’opération de mise à jour remplace les informations.</span><span class="sxs-lookup"><span data-stu-id="1b969-134">If there is a conflict, the update operation will overwrite information.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="1b969-135">Attribut MessageDisposition</span><span class="sxs-lookup"><span data-stu-id="1b969-135">MessageDisposition Attribute</span></span>

|<span data-ttu-id="1b969-136">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1b969-136">**Value**</span></span>|<span data-ttu-id="1b969-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="1b969-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1b969-138">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="1b969-138">SaveOnly</span></span>  <br/> |<span data-ttu-id="1b969-139">L’élément est mis à jour et enregistré dans son dossier actuel.</span><span class="sxs-lookup"><span data-stu-id="1b969-139">The item is updated and saved back to its current folder.</span></span>  <br/> |
|<span data-ttu-id="1b969-140">SendOnly</span><span class="sxs-lookup"><span data-stu-id="1b969-140">SendOnly</span></span>  <br/> |<span data-ttu-id="1b969-141">L’élément est mis à jour et envoyé, mais aucune copie n’est enregistrée.</span><span class="sxs-lookup"><span data-stu-id="1b969-141">The item is updated and sent but no copy is saved.</span></span>  <br/> |
|<span data-ttu-id="1b969-142">Méthodesendandsavecopy</span><span class="sxs-lookup"><span data-stu-id="1b969-142">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="1b969-143">L’élément est mis à jour et une copie est enregistrée dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="1b969-143">The item is updated and a copy is saved in the folder identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a><span data-ttu-id="1b969-144">Attribut SendMeetingInvitationsOrCancellations</span><span class="sxs-lookup"><span data-stu-id="1b969-144">SendMeetingInvitationsOrCancellations Attribute</span></span>

|<span data-ttu-id="1b969-145">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1b969-145">**Value**</span></span>|<span data-ttu-id="1b969-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="1b969-146">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1b969-147">SendToNone</span><span class="sxs-lookup"><span data-stu-id="1b969-147">SendToNone</span></span>  <br/> |<span data-ttu-id="1b969-148">L’élément de calendrier est mis à jour, mais les mises à jour ne sont pas envoyées aux participants.</span><span class="sxs-lookup"><span data-stu-id="1b969-148">The calendar item is updated but updates are not sent to attendees.</span></span>  <br/> |
|<span data-ttu-id="1b969-149">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="1b969-149">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="1b969-150">L’élément de calendrier est mis à jour et la mise à jour de réunion est envoyée à tous les participants, mais n’est pas enregistrée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="1b969-150">The calendar item is updated and the meeting update is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="1b969-151">SendOnlyToChanged</span><span class="sxs-lookup"><span data-stu-id="1b969-151">SendOnlyToChanged</span></span>  <br/> |<span data-ttu-id="1b969-152">L’élément de calendrier est mis à jour et la mise à jour de réunion n’est envoyée qu’aux participants affectés par la modification de la réunion.</span><span class="sxs-lookup"><span data-stu-id="1b969-152">The calendar item is updated and the meeting update is sent only to attendees that are affected by the change in the meeting.</span></span>  <br/> |
|<span data-ttu-id="1b969-153">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="1b969-153">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="1b969-154">L’élément de calendrier est mis à jour, la mise à jour de réunion est envoyée à tous les participants et une copie est enregistrée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="1b969-154">The calendar item is updated, the meeting update is sent to all attendees, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="1b969-155">SendToChangedAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="1b969-155">SendToChangedAndSaveCopy</span></span>  <br/> |<span data-ttu-id="1b969-156">L’élément de calendrier est mis à jour, la mise à jour de réunion est envoyée à tous les participants affectés par la modification de la réunion, et une copie est enregistrée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="1b969-156">The calendar item is updated, the meeting update is sent to all attendees that are affected by the change in the meeting, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1b969-157">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1b969-157">Child elements</span></span>

|<span data-ttu-id="1b969-158">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1b969-158">**Element**</span></span>|<span data-ttu-id="1b969-159">**Description**</span><span class="sxs-lookup"><span data-stu-id="1b969-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b969-160">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="1b969-160">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="1b969-161">Identifie le dossier cible pour les opérations de mise à jour, d’envoi et de création d’éléments dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b969-161">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1b969-162">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="1b969-162">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="1b969-163">Contient un tableau d’éléments [ItemChange,](itemchange.md) qui identifient les éléments et les mises à jour à appliquer aux éléments.</span><span class="sxs-lookup"><span data-stu-id="1b969-163">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1b969-164">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1b969-164">Parent elements</span></span>

<span data-ttu-id="1b969-165">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1b969-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1b969-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="1b969-166">Remarks</span></span>

<span data-ttu-id="1b969-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b969-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b969-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1b969-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b969-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1b969-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1b969-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1b969-170">Schema Name</span></span>  <br/> |<span data-ttu-id="1b969-171">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1b969-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1b969-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1b969-172">Validation File</span></span>  <br/> |<span data-ttu-id="1b969-173">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1b969-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b969-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1b969-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b969-175">False</span><span class="sxs-lookup"><span data-stu-id="1b969-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b969-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1b969-176">See also</span></span>



[<span data-ttu-id="1b969-177">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="1b969-177">UpdateItem operation</span></span>](updateitem-operation.md)

