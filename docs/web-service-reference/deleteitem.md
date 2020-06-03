---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: L’élément DeleteItem définit une demande de suppression d’un élément d’une boîte aux lettres dans la Banque d’Exchange.
ms.openlocfilehash: ed13ee32b487f49740aed80e8705257d3e2e6938
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529202"
---
# <a name="deleteitem"></a><span data-ttu-id="fb641-103">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="fb641-103">DeleteItem</span></span>

<span data-ttu-id="fb641-104">L’élément **DeleteItem** définit une demande de suppression d’un élément d’une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb641-104">The **DeleteItem** element defines a request to delete an item from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 <span data-ttu-id="fb641-105">**DeleteItemType**</span><span class="sxs-lookup"><span data-stu-id="fb641-105">**DeleteItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb641-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fb641-106">Attributes and elements</span></span>

<span data-ttu-id="fb641-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fb641-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb641-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fb641-108">Attributes</span></span>

|<span data-ttu-id="fb641-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="fb641-109">**Attribute**</span></span>|<span data-ttu-id="fb641-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb641-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb641-111">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="fb641-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="fb641-112">Indique comment un élément est supprimé.</span><span class="sxs-lookup"><span data-stu-id="fb641-112">Describes how an item is deleted.</span></span> <span data-ttu-id="fb641-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="fb641-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="fb641-114">**SendMeetingCancellations**</span><span class="sxs-lookup"><span data-stu-id="fb641-114">**SendMeetingCancellations**</span></span> <br/> |<span data-ttu-id="fb641-115">Indique si la suppression d’un élément de calendrier est communiquée aux participants.</span><span class="sxs-lookup"><span data-stu-id="fb641-115">Describes whether a calendar item deletion is communicated to attendees.</span></span> <span data-ttu-id="fb641-116">Cet attribut est requis lorsque des éléments de calendrier sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="fb641-116">This attribute is required when calendar items are deleted.</span></span> <span data-ttu-id="fb641-117">Cet attribut est facultatif si les éléments autres que du calendrier sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="fb641-117">This attribute is optional if non-calendar items are deleted.</span></span>  <br/> |
|<span data-ttu-id="fb641-118">**AffectedTaskOccurrences**</span><span class="sxs-lookup"><span data-stu-id="fb641-118">**AffectedTaskOccurrences**</span></span> <br/> |<span data-ttu-id="fb641-119">Indique si une instance de tâche ou une tâche maître est supprimée par une [opération DeleteItem](deleteitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="fb641-119">Describes whether a task instance or a task master is deleted by a [DeleteItem operation](deleteitem-operation.md).</span></span> <span data-ttu-id="fb641-120">Cet attribut est requis lors de la suppression des tâches.</span><span class="sxs-lookup"><span data-stu-id="fb641-120">This attribute is required when tasks are deleted.</span></span> <span data-ttu-id="fb641-121">Cet attribut est facultatif lorsque des éléments autres que des tâches sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="fb641-121">This attribute is optional when non-task items are deleted.</span></span>  <br/> |
|<span data-ttu-id="fb641-122">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="fb641-122">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="fb641-123">Indique si les confirmations de lecture pour l’élément supprimé sont supprimées.</span><span class="sxs-lookup"><span data-stu-id="fb641-123">Indicates whether read receipts for the deleted item are suppressed.</span></span> <span data-ttu-id="fb641-124">La valeur de texte **true**indique que les confirmations de lecture sont supprimées.</span><span class="sxs-lookup"><span data-stu-id="fb641-124">A text value of **true**, indicates that the read receipts are suppressed.</span></span> <span data-ttu-id="fb641-125">La valeur **false** indique que les confirmations de lecture sont envoyées à l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="fb641-125">A value of **false** indicates that the read receipts are sent to the sender.</span></span> <span data-ttu-id="fb641-126">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="fb641-126">This attribute is optional.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="fb641-127">Attribut DeleteType</span><span class="sxs-lookup"><span data-stu-id="fb641-127">DeleteType attribute</span></span>

|<span data-ttu-id="fb641-128">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="fb641-128">**Value**</span></span>|<span data-ttu-id="fb641-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb641-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb641-130">HardDelete</span><span class="sxs-lookup"><span data-stu-id="fb641-130">HardDelete</span></span>  <br/> |<span data-ttu-id="fb641-131">Un élément est définitivement supprimé de la Banque.</span><span class="sxs-lookup"><span data-stu-id="fb641-131">An item is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="fb641-132">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="fb641-132">SoftDelete</span></span>  <br/> |<span data-ttu-id="fb641-133">Un élément est déplacé vers la benne si la benne est activée.</span><span class="sxs-lookup"><span data-stu-id="fb641-133">An item is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="fb641-134">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="fb641-134">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="fb641-135">Un élément est déplacé vers le dossier Éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="fb641-135">An item is moved to the Deleted Items folder.</span></span>  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a><span data-ttu-id="fb641-136">Attribut SendMeetingCancellations</span><span class="sxs-lookup"><span data-stu-id="fb641-136">SendMeetingCancellations attribute</span></span>

|<span data-ttu-id="fb641-137">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="fb641-137">**Value**</span></span>|<span data-ttu-id="fb641-138">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb641-138">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb641-139">SendToNone</span><span class="sxs-lookup"><span data-stu-id="fb641-139">SendToNone</span></span>  <br/> |<span data-ttu-id="fb641-140">Un élément de calendrier est supprimé sans envoyer de message d’annulation.</span><span class="sxs-lookup"><span data-stu-id="fb641-140">A calendar item is deleted without sending a cancellation message.</span></span>  <br/> |
|<span data-ttu-id="fb641-141">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="fb641-141">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="fb641-142">Un élément de calendrier est supprimé et un message d’annulation est envoyé à tous les participants.</span><span class="sxs-lookup"><span data-stu-id="fb641-142">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span>  <br/> |
|<span data-ttu-id="fb641-143">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="fb641-143">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="fb641-144">Un élément de calendrier est supprimé et un message d’annulation est envoyé à tous les participants.</span><span class="sxs-lookup"><span data-stu-id="fb641-144">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span> <span data-ttu-id="fb641-145">Une copie du message d’annulation est enregistrée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="fb641-145">A copy of the cancellation message is saved in the Sent Items folder.</span></span>  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a><span data-ttu-id="fb641-146">Attribut AffectedTaskOccurrences</span><span class="sxs-lookup"><span data-stu-id="fb641-146">AffectedTaskOccurrences attribute</span></span>

|<span data-ttu-id="fb641-147">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="fb641-147">**Value**</span></span>|<span data-ttu-id="fb641-148">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb641-148">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb641-149">AllOccurrences</span><span class="sxs-lookup"><span data-stu-id="fb641-149">AllOccurrences</span></span>  <br/> |<span data-ttu-id="fb641-150">Une demande de suppression d’élément supprime la tâche principale, et par conséquent toutes les tâches périodiques qui sont associées à la tâche principale.</span><span class="sxs-lookup"><span data-stu-id="fb641-150">A delete item request deletes the master task, and therefore all recurring tasks that are associated with the master task.</span></span>  <br/> |
|<span data-ttu-id="fb641-151">SpecifiedOccurrenceOnly</span><span class="sxs-lookup"><span data-stu-id="fb641-151">SpecifiedOccurrenceOnly</span></span>  <br/> |<span data-ttu-id="fb641-152">Une demande de suppression d’élément supprime uniquement les occurrences spécifiques d’une tâche.</span><span class="sxs-lookup"><span data-stu-id="fb641-152">A delete item request deletes only specific occurrences of a task.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fb641-153">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fb641-153">Child elements</span></span>

|<span data-ttu-id="fb641-154">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fb641-154">**Element**</span></span>|<span data-ttu-id="fb641-155">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb641-155">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb641-156">ItemIds</span><span class="sxs-lookup"><span data-stu-id="fb641-156">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="fb641-157">Contient un tableau d’éléments, d’éléments d’occurrences et d’éléments principaux périodiques à supprimer d’une boîte aux lettres dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb641-157">Contains an array of items, occurrence items, and recurring master items to delete from a mailbox in the Exchange store.</span></span> <span data-ttu-id="fb641-158">L' [opération DeleteItem](deleteitem-operation.md) peut être effectuée sur n’importe quel type d’élément.</span><span class="sxs-lookup"><span data-stu-id="fb641-158">The [DeleteItem operation](deleteitem-operation.md) can be performed on any item type.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb641-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fb641-159">Parent elements</span></span>

<span data-ttu-id="fb641-160">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fb641-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb641-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="fb641-161">Remarks</span></span>

<span data-ttu-id="fb641-162">Les options **MoveToDeletedItems** et **HardDelete** sont transactionnelles, ce qui signifie qu’au moment de la fin d’un appel de service Web, la base de données a déplacé l’élément dans le dossier éléments supprimés ou a définitivement supprimé l’élément de la base de données Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb641-162">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="fb641-163">Ce comportement est le même pour MicrosoftExchange Server 2007 et Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="fb641-163">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="fb641-164">L’option **SoftDelete** fonctionne différemment pour différentes versions cibles d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb641-164">The **SoftDelete** option works differently for different target versions of Exchange.</span></span> <span data-ttu-id="fb641-165">**SoftDelete** pour Exchange 2007 définit un bit sur l’élément qui indique à la base de données Exchange que l’élément sera déplacé vers le dossier de la benne à un moment indéterminé à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="fb641-165">**SoftDelete** for Exchange 2007 sets a bit on the item that indicates to the Exchange database that the item will be moved to the dumpster folder at an indeterminate time in the future.</span></span> <span data-ttu-id="fb641-166">**SoftDelete** pour Exchange 2010 déplace immédiatement l’élément vers la benne.</span><span class="sxs-lookup"><span data-stu-id="fb641-166">**SoftDelete** for Exchange 2010 immediately moves the item to the dumpster.</span></span> <span data-ttu-id="fb641-167">**SoftDelete** n’est pas une option de suppression de dossier.</span><span class="sxs-lookup"><span data-stu-id="fb641-167">**SoftDelete** is not an option for folder deletion.</span></span> <span data-ttu-id="fb641-168">Les recherches de parcours **SoftDelete** pour les éléments et les dossiers ne renverront aucun résultat.</span><span class="sxs-lookup"><span data-stu-id="fb641-168">**SoftDelete** traversal searches for items and folders will not return any results.</span></span> 
  
<span data-ttu-id="fb641-169">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb641-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb641-170">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fb641-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb641-171">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fb641-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fb641-172">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fb641-172">Schema Name</span></span>  <br/> |<span data-ttu-id="fb641-173">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="fb641-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fb641-174">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fb641-174">Validation File</span></span>  <br/> |<span data-ttu-id="fb641-175">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fb641-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb641-176">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fb641-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb641-177">False</span><span class="sxs-lookup"><span data-stu-id="fb641-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb641-178">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fb641-178">See also</span></span>

- [<span data-ttu-id="fb641-179">Updateitemresponse</span><span class="sxs-lookup"><span data-stu-id="fb641-179">DeleteItemResponse</span></span>](deleteitemresponse.md)  
- [<span data-ttu-id="fb641-180">Opération DeleteItem</span><span class="sxs-lookup"><span data-stu-id="fb641-180">DeleteItem operation</span></span>](deleteitem-operation.md)

