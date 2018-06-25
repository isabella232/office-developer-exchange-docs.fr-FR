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
ms.openlocfilehash: 7b9b5f1dcffb95eb127572cb91f92d961c05a77e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838893"
---
# <a name="updateitem"></a><span data-ttu-id="d879f-103">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="d879f-103">UpdateItem</span></span>

<span data-ttu-id="d879f-104">L’élément **UpdateItem** définit une demande de mise à jour d’un élément dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d879f-104">The **UpdateItem** element defines a request to update an item in a mailbox.</span></span> 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 <span data-ttu-id="d879f-105">**UpdateItemType**</span><span class="sxs-lookup"><span data-stu-id="d879f-105">**UpdateItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d879f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d879f-106">Attributes and elements</span></span>

<span data-ttu-id="d879f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d879f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d879f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d879f-108">Attributes</span></span>

|<span data-ttu-id="d879f-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d879f-109">**Attribute**</span></span>|<span data-ttu-id="d879f-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d879f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d879f-111">**ConflictResolution**</span><span class="sxs-lookup"><span data-stu-id="d879f-111">**ConflictResolution**</span></span> <br/> |<span data-ttu-id="d879f-112">Identifie le type de résolution de conflit pour essayer pendant une mise à jour.</span><span class="sxs-lookup"><span data-stu-id="d879f-112">Identifies the type of conflict resolution to try during an update.</span></span> <span data-ttu-id="d879f-113">La valeur par défaut est résoudre automatiquement.</span><span class="sxs-lookup"><span data-stu-id="d879f-113">The default value is AutoResolve.</span></span>  <br/> |
|<span data-ttu-id="d879f-114">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="d879f-114">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="d879f-115">Décrit comment l’élément est traitée une fois qu’il est mis à jour.</span><span class="sxs-lookup"><span data-stu-id="d879f-115">Describes how the item will be handled after it is updated.</span></span> <span data-ttu-id="d879f-116">L’attribut **MessageDisposition** est requis pour les éléments de message, y compris les messages de réunion comme annulations de réunion, les demandes de réunion et les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="d879f-116">The **MessageDisposition** attribute is required for message items, including meeting messages such as meeting cancellations, meeting requests, and meeting responses.</span></span>  <br/> |
|<span data-ttu-id="d879f-117">**SendMeetingInvitationsOrCancellations**</span><span class="sxs-lookup"><span data-stu-id="d879f-117">**SendMeetingInvitationsOrCancellations**</span></span> <br/> |<span data-ttu-id="d879f-118">Décrit comment les mises à jour de réunion sont communiquées après qu’un élément de calendrier est mis à jour.</span><span class="sxs-lookup"><span data-stu-id="d879f-118">Describes how meeting updates are communicated after a calendar item is updated.</span></span> <span data-ttu-id="d879f-119">Cet attribut est requis pour les éléments de calendrier et occurrences d’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="d879f-119">This attribute is required for calendar items and calendar item occurrences.</span></span>  <br/> |
|<span data-ttu-id="d879f-120">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="d879f-120">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="d879f-121">Indique si les confirmations de lecture de l’élément mis à jour doivent être supprimées.</span><span class="sxs-lookup"><span data-stu-id="d879f-121">Indicates whether read receipts for the updated item should be suppressed.</span></span> <span data-ttu-id="d879f-122">Une valeur de texte de **la valeur true** indique read accusés de réception doivent être supprimées.</span><span class="sxs-lookup"><span data-stu-id="d879f-122">A text value of **true** indicates that read receipts should be suppressed.</span></span> <span data-ttu-id="d879f-123">La valeur **false** indique que les confirmations de lecture sont envoyées à l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="d879f-123">A value of **false** indicates that the read receipts will be sent to the sender.</span></span> <span data-ttu-id="d879f-124">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d879f-124">This attribute is optional.</span></span>  <br/> <span data-ttu-id="d879f-125">Cet attribut est une nouveauté d’Exchange Server 2013 SP1.</span><span class="sxs-lookup"><span data-stu-id="d879f-125">This attribute was introduced in Exchange Server 2013 SP1.</span></span>  <br/> |
   
#### <a name="conflictresolution-attribute"></a><span data-ttu-id="d879f-126">Attribut ConflictResolution</span><span class="sxs-lookup"><span data-stu-id="d879f-126">ConflictResolution Attribute</span></span>

|<span data-ttu-id="d879f-127">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d879f-127">**Value**</span></span>|<span data-ttu-id="d879f-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="d879f-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d879f-129">NeverOverwrite</span><span class="sxs-lookup"><span data-stu-id="d879f-129">NeverOverwrite</span></span>  <br/> |<span data-ttu-id="d879f-130">S’il existe un conflit, l’opération de mise à jour échoue et une erreur est renvoyée.</span><span class="sxs-lookup"><span data-stu-id="d879f-130">If there is a conflict, the update operation fails and an error is returned.</span></span>  <br/> |
|<span data-ttu-id="d879f-131">Résolution automatique</span><span class="sxs-lookup"><span data-stu-id="d879f-131">AutoResolve</span></span>  <br/> |<span data-ttu-id="d879f-132">L’opération de mise à jour corrige automatiquement tout conflit.</span><span class="sxs-lookup"><span data-stu-id="d879f-132">The update operation automatically resolves any conflict.</span></span>  <br/> |
|<span data-ttu-id="d879f-133">AlwaysOverwrite</span><span class="sxs-lookup"><span data-stu-id="d879f-133">AlwaysOverwrite</span></span>  <br/> |<span data-ttu-id="d879f-134">S’il existe un conflit, l’opération de mise à jour remplacera les informations.</span><span class="sxs-lookup"><span data-stu-id="d879f-134">If there is a conflict, the update operation will overwrite information.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="d879f-135">Attribut MessageDisposition</span><span class="sxs-lookup"><span data-stu-id="d879f-135">MessageDisposition Attribute</span></span>

|<span data-ttu-id="d879f-136">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d879f-136">**Value**</span></span>|<span data-ttu-id="d879f-137">**Description**</span><span class="sxs-lookup"><span data-stu-id="d879f-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d879f-138">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="d879f-138">SaveOnly</span></span>  <br/> |<span data-ttu-id="d879f-139">L’élément est mis à jour et enregistré dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="d879f-139">The item is updated and saved back to its current folder.</span></span>  <br/> |
|<span data-ttu-id="d879f-140">SendOnly</span><span class="sxs-lookup"><span data-stu-id="d879f-140">SendOnly</span></span>  <br/> |<span data-ttu-id="d879f-141">L’élément est mis à jour et envoyé, mais aucune copie n’est enregistrée.</span><span class="sxs-lookup"><span data-stu-id="d879f-141">The item is updated and sent but no copy is saved.</span></span>  <br/> |
|<span data-ttu-id="d879f-142">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="d879f-142">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="d879f-143">L’élément est mis à jour et une copie est enregistrée dans le dossier identifié par l’élément [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="d879f-143">The item is updated and a copy is saved in the folder identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a><span data-ttu-id="d879f-144">Attribut SendMeetingInvitationsOrCancellations</span><span class="sxs-lookup"><span data-stu-id="d879f-144">SendMeetingInvitationsOrCancellations Attribute</span></span>

|<span data-ttu-id="d879f-145">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d879f-145">**Value**</span></span>|<span data-ttu-id="d879f-146">**Description**</span><span class="sxs-lookup"><span data-stu-id="d879f-146">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d879f-147">SendToNone</span><span class="sxs-lookup"><span data-stu-id="d879f-147">SendToNone</span></span>  <br/> |<span data-ttu-id="d879f-148">L’élément de calendrier est mis à jour mais les mises à jour ne sont pas envoyées aux participants.</span><span class="sxs-lookup"><span data-stu-id="d879f-148">The calendar item is updated but updates are not sent to attendees.</span></span>  <br/> |
|<span data-ttu-id="d879f-149">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="d879f-149">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="d879f-150">L’élément de calendrier est mis à jour et la mise à jour de réunion est envoyée à tous les participants, mais n’est pas enregistré dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="d879f-150">The calendar item is updated and the meeting update is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="d879f-151">SendOnlyToChanged</span><span class="sxs-lookup"><span data-stu-id="d879f-151">SendOnlyToChanged</span></span>  <br/> |<span data-ttu-id="d879f-152">L’élément de calendrier est mis à jour et la mise à jour de réunion est envoyée uniquement aux participants qui sont affectées par la modification de la réunion.</span><span class="sxs-lookup"><span data-stu-id="d879f-152">The calendar item is updated and the meeting update is sent only to attendees that are affected by the change in the meeting.</span></span>  <br/> |
|<span data-ttu-id="d879f-153">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="d879f-153">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="d879f-154">L’élément de calendrier est mis à jour, la mise à jour de réunion est envoyée à tous les participants et une copie est enregistrée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="d879f-154">The calendar item is updated, the meeting update is sent to all attendees, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="d879f-155">SendToChangedAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="d879f-155">SendToChangedAndSaveCopy</span></span>  <br/> |<span data-ttu-id="d879f-156">L’élément de calendrier est mis à jour, la mise à jour de réunion est envoyée à tous les participants qui sont affectées par la modification de la réunion et une copie est enregistrée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="d879f-156">The calendar item is updated, the meeting update is sent to all attendees that are affected by the change in the meeting, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d879f-157">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d879f-157">Child elements</span></span>

|<span data-ttu-id="d879f-158">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d879f-158">**Element**</span></span>|<span data-ttu-id="d879f-159">**Description**</span><span class="sxs-lookup"><span data-stu-id="d879f-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d879f-160">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="d879f-160">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="d879f-161">Identifie le dossier cible pour les opérations de mise à jour, d’envoyer et de créer des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="d879f-161">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d879f-162">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="d879f-162">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="d879f-163">Contient un tableau d’éléments [ItemChange](itemchange.md) qui identifient les éléments et les mises à jour à appliquer aux éléments.</span><span class="sxs-lookup"><span data-stu-id="d879f-163">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d879f-164">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d879f-164">Parent elements</span></span>

<span data-ttu-id="d879f-165">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d879f-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d879f-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="d879f-166">Remarks</span></span>

<span data-ttu-id="d879f-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d879f-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d879f-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d879f-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d879f-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d879f-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d879f-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d879f-170">Schema Name</span></span>  <br/> |<span data-ttu-id="d879f-171">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d879f-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d879f-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d879f-172">Validation File</span></span>  <br/> |<span data-ttu-id="d879f-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d879f-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d879f-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d879f-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="d879f-175">False</span><span class="sxs-lookup"><span data-stu-id="d879f-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d879f-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d879f-176">See also</span></span>



[<span data-ttu-id="d879f-177">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="d879f-177">UpdateItem operation</span></span>](updateitem-operation.md)

