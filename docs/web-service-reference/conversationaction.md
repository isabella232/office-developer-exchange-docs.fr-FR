---
title: ConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: L’élément ConversationAction contient une action unique à appliquer à une conversation unique.
ms.openlocfilehash: cb7d874f787b105d5185749dfaf1e940d2411d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529251"
---
# <a name="conversationaction"></a><span data-ttu-id="9ee30-103">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="9ee30-103">ConversationAction</span></span>

<span data-ttu-id="9ee30-104">L’élément **ConversationAction** contient une action unique à appliquer à une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="9ee30-104">The **ConversationAction** element contains a single action to be applied to a single conversation.</span></span> 
  
[<span data-ttu-id="9ee30-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="9ee30-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="9ee30-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="9ee30-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="9ee30-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="9ee30-107">ConversationAction</span></span>](conversationaction.md)
  
```XML
<ConversationAction>
   <Action/>
   <ConversationId/>
   <ContextFolderId/>
   <ConversationLastSyncTime/>
   <ProcessRightAway/>
   <DestinationFolderId/>
   <Categories/>
   <EnableAlwaysDelete/>
   <IsRead/>
   <DeleteType/>
</ConversationAction>
```

 <span data-ttu-id="9ee30-108">**ConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="9ee30-108">**ConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ee30-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9ee30-109">Attributes and elements</span></span>

<span data-ttu-id="9ee30-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9ee30-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ee30-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="9ee30-111">Attributes</span></span>

<span data-ttu-id="9ee30-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9ee30-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ee30-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9ee30-113">Child elements</span></span>

|<span data-ttu-id="9ee30-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9ee30-114">**Element**</span></span>|<span data-ttu-id="9ee30-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="9ee30-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ee30-116">Action (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="9ee30-116">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md) <br/> |<span data-ttu-id="9ee30-117">Contient l’action à effectuer sur la conversation spécifiée par l’élément [ConversationId](conversationid.md) .</span><span class="sxs-lookup"><span data-stu-id="9ee30-117">Contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> <span data-ttu-id="9ee30-118">Cet élément doit être présent.</span><span class="sxs-lookup"><span data-stu-id="9ee30-118">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="9ee30-119">ConversationId</span><span class="sxs-lookup"><span data-stu-id="9ee30-119">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="9ee30-120">Contient l’identificateur de la conversation pour laquelle l’action spécifiée par l’élément [action (ConversationActionTypeType)](action-conversationactiontypetype.md) est appliquée aux éléments de la conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-120">Contains the identifier of the conversation that will have the action specified by the [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) element applied to items in the conversation.</span></span> <span data-ttu-id="9ee30-121">Cet élément doit être présent.</span><span class="sxs-lookup"><span data-stu-id="9ee30-121">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="9ee30-122">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="9ee30-122">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="9ee30-123">Indique le dossier ciblé pour les actions qui utilisent des dossiers.</span><span class="sxs-lookup"><span data-stu-id="9ee30-123">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="9ee30-124">Cet élément doit être présent lors de la copie, la suppression, le mouvement et la définition de l’état de lecture des éléments de conversation dans un dossier cible.</span><span class="sxs-lookup"><span data-stu-id="9ee30-124">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="9ee30-125">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="9ee30-125">ConversationLastSyncTime</span></span>](conversationlastsynctime.md) <br/> |<span data-ttu-id="9ee30-126">Contient la date et l’heure de la dernière synchronisation d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-126">Contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="9ee30-127">Cet élément doit être présent lors de la tentative de suppression de tous les éléments d’une conversation qui ont été reçus pendant la durée spécifiée.</span><span class="sxs-lookup"><span data-stu-id="9ee30-127">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span>  <br/> |
|[<span data-ttu-id="9ee30-128">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="9ee30-128">ProcessRightAway</span></span>](processrightaway.md) <br/> |<span data-ttu-id="9ee30-129">Indique si la réponse est envoyée dès que l’action commence à traiter sur le serveur ou si la réponse est envoyée une fois l’action terminée.</span><span class="sxs-lookup"><span data-stu-id="9ee30-129">Indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="9ee30-130">Cet élément doit être présent pour que la réponse soit envoyée de manière asynchrone à l’action demandée.</span><span class="sxs-lookup"><span data-stu-id="9ee30-130">This element must be present for the response to be sent asynchronous to the requested action.</span></span>  <br/> |
|[<span data-ttu-id="9ee30-131">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="9ee30-131">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="9ee30-132">Indique le dossier de destination pour les actions de copie et de déplacement.</span><span class="sxs-lookup"><span data-stu-id="9ee30-132">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="9ee30-133">Catégories</span><span class="sxs-lookup"><span data-stu-id="9ee30-133">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9ee30-134">Contient une collection de chaînes qui identifient les catégories auxquelles appartiennent les éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-134">Contains a collection of strings that identify the categories to which items in a conversation belong.</span></span>  <br/> |
|[<span data-ttu-id="9ee30-135">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="9ee30-135">EnableAlwaysDelete</span></span>](enablealwaysdelete.md) <br/> |<span data-ttu-id="9ee30-136">Spécifie un indicateur qui active la suppression de tous les nouveaux éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-136">Specifies a flag that enables deletion for all new items in a conversation.</span></span>  <br/> |
|[<span data-ttu-id="9ee30-137">IsRead</span><span class="sxs-lookup"><span data-stu-id="9ee30-137">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="9ee30-138">Indique si un message a été lu.</span><span class="sxs-lookup"><span data-stu-id="9ee30-138">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="9ee30-139">DeleteType</span><span class="sxs-lookup"><span data-stu-id="9ee30-139">DeleteType</span></span>](deletetype.md) <br/> |<span data-ttu-id="9ee30-140">Indique le mode de suppression des éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-140">Indicates how items in a conversation are deleted.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ee30-141">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9ee30-141">Parent elements</span></span>

|<span data-ttu-id="9ee30-142">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9ee30-142">**Element**</span></span>|<span data-ttu-id="9ee30-143">**Description**</span><span class="sxs-lookup"><span data-stu-id="9ee30-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ee30-144">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="9ee30-144">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="9ee30-145">Contient une collection de conversations et les actions à leur appliquer.</span><span class="sxs-lookup"><span data-stu-id="9ee30-145">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9ee30-146">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="9ee30-146">Text value</span></span>

<span data-ttu-id="9ee30-147">**Valeurs de texte de l’élément ConversationAction**</span><span class="sxs-lookup"><span data-stu-id="9ee30-147">**ConversationAction element text values**</span></span>

|<span data-ttu-id="9ee30-148">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="9ee30-148">**Value**</span></span>|<span data-ttu-id="9ee30-149">**Description**</span><span class="sxs-lookup"><span data-stu-id="9ee30-149">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9ee30-150">AlwaysCategorize</span><span class="sxs-lookup"><span data-stu-id="9ee30-150">AlwaysCategorize</span></span>  <br/> |<span data-ttu-id="9ee30-151">Toujours catégoriser la conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-151">Always categorize the conversation.</span></span>  <br/> |
|<span data-ttu-id="9ee30-152">AlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="9ee30-152">AlwaysDelete</span></span>  <br/> |<span data-ttu-id="9ee30-153">Supprimez toujours la conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-153">Always delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="9ee30-154">AlwaysMove</span><span class="sxs-lookup"><span data-stu-id="9ee30-154">AlwaysMove</span></span>  <br/> |<span data-ttu-id="9ee30-155">Toujours déplacer la conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-155">Always move the conversation.</span></span>  <br/> |
|<span data-ttu-id="9ee30-156">Supprimer</span><span class="sxs-lookup"><span data-stu-id="9ee30-156">Delete</span></span>  <br/> |<span data-ttu-id="9ee30-157">Supprimez la conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-157">Delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="9ee30-158">Move</span><span class="sxs-lookup"><span data-stu-id="9ee30-158">Move</span></span>  <br/> |<span data-ttu-id="9ee30-159">Déplacer la conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-159">Move the conversation.</span></span>  <br/> |
|<span data-ttu-id="9ee30-160">Copy</span><span class="sxs-lookup"><span data-stu-id="9ee30-160">Copy</span></span>  <br/> |<span data-ttu-id="9ee30-161">Copiez la conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-161">Copy the conversation.</span></span>  <br/> |
|<span data-ttu-id="9ee30-162">SetReadState</span><span class="sxs-lookup"><span data-stu-id="9ee30-162">SetReadState</span></span>  <br/> |<span data-ttu-id="9ee30-163">Définir l’état de lecture de la conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-163">Set the read state of the conversation.</span></span>  <br/> |
|<span data-ttu-id="9ee30-164">SetRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="9ee30-164">SetRetentionPolicy</span></span>  <br/> |<span data-ttu-id="9ee30-165">Définir la stratégie de rétention pour la conversation.</span><span class="sxs-lookup"><span data-stu-id="9ee30-165">Set the retention policy for the conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9ee30-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="9ee30-166">Remarks</span></span>

<span data-ttu-id="9ee30-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9ee30-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ee30-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9ee30-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ee30-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9ee30-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ee30-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9ee30-170">Schema Name</span></span>  <br/> |<span data-ttu-id="9ee30-171">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9ee30-171">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ee30-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9ee30-172">Validation File</span></span>  <br/> |<span data-ttu-id="9ee30-173">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9ee30-173">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ee30-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9ee30-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ee30-175">False</span><span class="sxs-lookup"><span data-stu-id="9ee30-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ee30-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9ee30-176">See also</span></span>



[<span data-ttu-id="9ee30-177">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="9ee30-177">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="9ee30-178">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9ee30-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

