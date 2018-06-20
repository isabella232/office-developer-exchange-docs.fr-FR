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
description: L’élément DeleteItem définit une demande pour supprimer un élément d’une boîte aux lettres dans la banque d’informations Exchange.
ms.openlocfilehash: de64787750c88c8a47bb69daddc0a1d2ebe8bde9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755874"
---
# <a name="deleteitem"></a><span data-ttu-id="4f1a9-103">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="4f1a9-103">DeleteItem</span></span>

<span data-ttu-id="4f1a9-104">L’élément **DeleteItem** définit une demande pour supprimer un élément d’une boîte aux lettres dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-104">The **DeleteItem** element defines a request to delete an item from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 <span data-ttu-id="4f1a9-105">**DeleteItemType**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-105">**DeleteItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f1a9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4f1a9-106">Attributes and elements</span></span>

<span data-ttu-id="4f1a9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f1a9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4f1a9-108">Attributes</span></span>

|<span data-ttu-id="4f1a9-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-109">**Attribute**</span></span>|<span data-ttu-id="4f1a9-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4f1a9-111">**DeleType**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="4f1a9-112">Décrit comment un élément est supprimé.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-112">Describes how an item is deleted.</span></span> <span data-ttu-id="4f1a9-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="4f1a9-114">**SendMeetingCancellations**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-114">**SendMeetingCancellations**</span></span> <br/> |<span data-ttu-id="4f1a9-115">Indique si une suppression de l’élément calendrier est communiquée aux participants.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-115">Describes whether a calendar item deletion is communicated to attendees.</span></span> <span data-ttu-id="4f1a9-116">Cet attribut est requis lorsque des éléments de calendrier sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-116">This attribute is required when calendar items are deleted.</span></span> <span data-ttu-id="4f1a9-117">Cet attribut est facultatif si les éléments de calendrier non sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-117">This attribute is optional if non-calendar items are deleted.</span></span>  <br/> |
|<span data-ttu-id="4f1a9-118">**AffectedTaskOccurrences**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-118">**AffectedTaskOccurrences**</span></span> <br/> |<span data-ttu-id="4f1a9-119">Indique si une instance de tâche ou d’un masque de tâche est supprimé par une [opération DeleteItem](deleteitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4f1a9-119">Describes whether a task instance or a task master is deleted by a [DeleteItem operation](deleteitem-operation.md).</span></span> <span data-ttu-id="4f1a9-120">Cet attribut est requis lorsque les tâches sont supprimées.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-120">This attribute is required when tasks are deleted.</span></span> <span data-ttu-id="4f1a9-121">Cet attribut est facultatif lors d’une tâche non sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-121">This attribute is optional when non-task items are deleted.</span></span>  <br/> |
|<span data-ttu-id="4f1a9-122">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-122">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="4f1a9-123">Indique si les confirmations de lecture de l’élément supprimé sont supprimées.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-123">Indicates whether read receipts for the deleted item are suppressed.</span></span> <span data-ttu-id="4f1a9-124">Une valeur de texte de **la valeur true**, indique que les confirmations de lecture sont supprimées.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-124">A text value of **true**, indicates that the read receipts are suppressed.</span></span> <span data-ttu-id="4f1a9-125">La valeur **false** indique que les confirmations de lecture sont envoyées à l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-125">A value of **false** indicates that the read receipts are sent to the sender.</span></span> <span data-ttu-id="4f1a9-126">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-126">This attribute is optional.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="4f1a9-127">Attribut DeleType</span><span class="sxs-lookup"><span data-stu-id="4f1a9-127">DeleteType attribute</span></span>

|<span data-ttu-id="4f1a9-128">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-128">**Value**</span></span>|<span data-ttu-id="4f1a9-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4f1a9-130">HardDelete</span><span class="sxs-lookup"><span data-stu-id="4f1a9-130">HardDelete</span></span>  <br/> |<span data-ttu-id="4f1a9-131">Un élément est définitivement supprimé de la banque.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-131">An item is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="4f1a9-132">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="4f1a9-132">SoftDelete</span></span>  <br/> |<span data-ttu-id="4f1a9-133">Un élément est déplacé vers la benne si la benne est activé.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-133">An item is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="4f1a9-134">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="4f1a9-134">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="4f1a9-135">Un élément est déplacé vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-135">An item is moved to the Deleted Items folder.</span></span>  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a><span data-ttu-id="4f1a9-136">Attribut SendMeetingCancellations</span><span class="sxs-lookup"><span data-stu-id="4f1a9-136">SendMeetingCancellations attribute</span></span>

|<span data-ttu-id="4f1a9-137">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-137">**Value**</span></span>|<span data-ttu-id="4f1a9-138">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-138">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4f1a9-139">SendToNone</span><span class="sxs-lookup"><span data-stu-id="4f1a9-139">SendToNone</span></span>  <br/> |<span data-ttu-id="4f1a9-140">Un élément de calendrier est supprimé sans envoyer un message d’annulation.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-140">A calendar item is deleted without sending a cancellation message.</span></span>  <br/> |
|<span data-ttu-id="4f1a9-141">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="4f1a9-141">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="4f1a9-142">Suppression d’un élément de calendrier et un message d’annulation est envoyé à tous les participants.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-142">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span>  <br/> |
|<span data-ttu-id="4f1a9-143">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="4f1a9-143">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="4f1a9-144">Suppression d’un élément de calendrier et un message d’annulation est envoyé à tous les participants.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-144">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span> <span data-ttu-id="4f1a9-145">Une copie du message l’annulation est enregistrée dans le dossier éléments envoyés.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-145">A copy of the cancellation message is saved in the Sent Items folder.</span></span>  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a><span data-ttu-id="4f1a9-146">Attribut AffectedTaskOccurrences</span><span class="sxs-lookup"><span data-stu-id="4f1a9-146">AffectedTaskOccurrences attribute</span></span>

|<span data-ttu-id="4f1a9-147">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-147">**Value**</span></span>|<span data-ttu-id="4f1a9-148">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-148">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4f1a9-149">AllOccurrences</span><span class="sxs-lookup"><span data-stu-id="4f1a9-149">AllOccurrences</span></span>  <br/> |<span data-ttu-id="4f1a9-150">Une requête d’élément delete Supprime la tâche principale et par conséquent, toutes les tâches périodiques qui sont associés à la tâche principale.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-150">A delete item request deletes the master task, and therefore all recurring tasks that are associated with the master task.</span></span>  <br/> |
|<span data-ttu-id="4f1a9-151">SpecifiedOccurrenceOnly</span><span class="sxs-lookup"><span data-stu-id="4f1a9-151">SpecifiedOccurrenceOnly</span></span>  <br/> |<span data-ttu-id="4f1a9-152">Une requête d’élément delete Supprime uniquement des occurrences spécifiques d’une tâche.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-152">A delete item request deletes only specific occurrences of a task.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4f1a9-153">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4f1a9-153">Child elements</span></span>

|<span data-ttu-id="4f1a9-154">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-154">**Element**</span></span>|<span data-ttu-id="4f1a9-155">**Description**</span><span class="sxs-lookup"><span data-stu-id="4f1a9-155">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f1a9-156">ItemId</span><span class="sxs-lookup"><span data-stu-id="4f1a9-156">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="4f1a9-157">Contient un tableau d’éléments, des éléments d’occurrence et des éléments de gabarit périodiques pour supprimer une boîte aux lettres dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-157">Contains an array of items, occurrence items, and recurring master items to delete from a mailbox in the Exchange store.</span></span> <span data-ttu-id="4f1a9-158">L' [opération DeleteItem](deleteitem-operation.md) peuvent être effectuées sur n’importe quel type d’élément.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-158">The [DeleteItem operation](deleteitem-operation.md) can be performed on any item type.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4f1a9-159">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4f1a9-159">Parent elements</span></span>

<span data-ttu-id="4f1a9-160">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4f1a9-161">Remarques</span><span class="sxs-lookup"><span data-stu-id="4f1a9-161">Remarks</span></span>

<span data-ttu-id="4f1a9-162">Les options **MoveToDeletedItems** et **HardDelete** sont transactionnelles, ce qui signifie qu’au moment où un appel au service Web est terminée, la base de données a déplacé l’élément vers le dossier éléments supprimés ou définitivement supprimé l’élément de la base de données Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-162">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="4f1a9-163">Ce comportement est la même valeur MicrosoftExchange Server 2007 et Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-163">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="4f1a9-164">L’option **SoftDelete** fonctionne différemment pour cible différentes versions d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-164">The **SoftDelete** option works differently for different target versions of Exchange.</span></span> <span data-ttu-id="4f1a9-165">**SoftDelete** pour Exchange 2007 définit un bit sur l’élément qui indique à la base de données Exchange qui est déplacée vers l’élément de la benne de dossier à un moment indéterminé, à l’avenir.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-165">**SoftDelete** for Exchange 2007 sets a bit on the item that indicates to the Exchange database that the item will be moved to the dumpster folder at an indeterminate time in the future.</span></span> <span data-ttu-id="4f1a9-166">**SoftDelete** pour Exchange 2010 déplace immédiatement l’élément à la benne.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-166">**SoftDelete** for Exchange 2010 immediately moves the item to the dumpster.</span></span> <span data-ttu-id="4f1a9-167">**SoftDelete** n’est pas une option de suppression du dossier.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-167">**SoftDelete** is not an option for folder deletion.</span></span> <span data-ttu-id="4f1a9-168">**SoftDelete** des recherches de traversée du contenu pour les éléments et les dossiers ne renvoie aucun résultat.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-168">**SoftDelete** traversal searches for items and folders will not return any results.</span></span> 
  
<span data-ttu-id="4f1a9-169">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f1a9-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f1a9-170">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4f1a9-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f1a9-171">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4f1a9-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4f1a9-172">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4f1a9-172">Schema Name</span></span>  <br/> |<span data-ttu-id="4f1a9-173">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4f1a9-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4f1a9-174">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4f1a9-174">Validation File</span></span>  <br/> |<span data-ttu-id="4f1a9-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4f1a9-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4f1a9-176">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4f1a9-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="4f1a9-177">False</span><span class="sxs-lookup"><span data-stu-id="4f1a9-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f1a9-178">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4f1a9-178">See also</span></span>

- [<span data-ttu-id="4f1a9-179">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="4f1a9-179">DeleteItemResponse</span></span>](deleteitemresponse.md)  
- [<span data-ttu-id="4f1a9-180">Opération DeleteItem</span><span class="sxs-lookup"><span data-stu-id="4f1a9-180">DeleteItem operation</span></span>](deleteitem-operation.md)

