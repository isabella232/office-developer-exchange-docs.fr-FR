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
description: L’élément ConversationAction contient une seule action à appliquer à une même conversation.
ms.openlocfilehash: 45cd6df3aba94062bd5aa0ddf9367e8cf118dc6b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755637"
---
# <a name="conversationaction"></a><span data-ttu-id="c9e56-103">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="c9e56-103">ConversationAction</span></span>

<span data-ttu-id="c9e56-104">L’élément **ConversationAction** contient une seule action à appliquer à une même conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-104">The **ConversationAction** element contains a single action to be applied to a single conversation.</span></span> 
  
[<span data-ttu-id="c9e56-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="c9e56-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="c9e56-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="c9e56-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="c9e56-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="c9e56-107">ConversationAction</span></span>](conversationaction.md)
  
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

 <span data-ttu-id="c9e56-108">**ConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="c9e56-108">**ConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9e56-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c9e56-109">Attributes and elements</span></span>

<span data-ttu-id="c9e56-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c9e56-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9e56-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="c9e56-111">Attributes</span></span>

<span data-ttu-id="c9e56-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c9e56-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9e56-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c9e56-113">Child elements</span></span>

|<span data-ttu-id="c9e56-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c9e56-114">**Element**</span></span>|<span data-ttu-id="c9e56-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="c9e56-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9e56-116">Action (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="c9e56-116">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md) <br/> |<span data-ttu-id="c9e56-117">Contient l’action à effectuer sur la conversation spécifiée par l’élément [ConversationId](conversationid.md) .</span><span class="sxs-lookup"><span data-stu-id="c9e56-117">Contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> <span data-ttu-id="c9e56-118">Cet élément doit être présent.</span><span class="sxs-lookup"><span data-stu-id="c9e56-118">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="c9e56-119">ConversationId</span><span class="sxs-lookup"><span data-stu-id="c9e56-119">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="c9e56-120">Contient l’identificateur de la conversation qui auront l’action spécifiée par l’élément [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) appliqué aux éléments de la conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-120">Contains the identifier of the conversation that will have the action specified by the [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) element applied to items in the conversation.</span></span> <span data-ttu-id="c9e56-121">Cet élément doit être présent.</span><span class="sxs-lookup"><span data-stu-id="c9e56-121">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="c9e56-122">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="c9e56-122">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="c9e56-123">Indique le dossier qui est ciblé pour les actions qui utilisent des dossiers.</span><span class="sxs-lookup"><span data-stu-id="c9e56-123">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="c9e56-124">Cet élément doit être présent lors de la copie, suppression, déplacement et en définissant l’état de lecture sur les éléments de conversation dans un dossier cible.</span><span class="sxs-lookup"><span data-stu-id="c9e56-124">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="c9e56-125">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="c9e56-125">ConversationLastSyncTime</span></span>](conversationlastsynctime.md) <br/> |<span data-ttu-id="c9e56-126">Contient la date et l’heure de dernière synchronisation une conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-126">Contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="c9e56-127">Cet élément doit être présent lorsque vous tentez de supprimer tous les éléments qui ont été reçus jusqu'à l’heure spécifiée dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-127">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span>  <br/> |
|[<span data-ttu-id="c9e56-128">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="c9e56-128">ProcessRightAway</span></span>](processrightaway.md) <br/> |<span data-ttu-id="c9e56-129">Indique si la réponse est envoyée dès que l’action démarre le traitement sur le serveur ou si la réponse est envoyée une fois l’action terminée.</span><span class="sxs-lookup"><span data-stu-id="c9e56-129">Indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="c9e56-130">Cet élément doit être présent pour la réponse à envoyer asynchrone à l’action demandée.</span><span class="sxs-lookup"><span data-stu-id="c9e56-130">This element must be present for the response to be sent asynchronous to the requested action.</span></span>  <br/> |
|[<span data-ttu-id="c9e56-131">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="c9e56-131">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="c9e56-132">Indique le dossier de destination de copie et les actions de déplacement.</span><span class="sxs-lookup"><span data-stu-id="c9e56-132">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="c9e56-133">Categories</span><span class="sxs-lookup"><span data-stu-id="c9e56-133">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c9e56-134">Contient une collection de chaînes qui identifient les catégories auquel appartiennent les éléments dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-134">Contains a collection of strings that identify the categories to which items in a conversation belong.</span></span>  <br/> |
|[<span data-ttu-id="c9e56-135">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="c9e56-135">EnableAlwaysDelete</span></span>](enablealwaysdelete.md) <br/> |<span data-ttu-id="c9e56-136">Spécifie un indicateur qui permet la suppression de tous les nouveaux éléments dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-136">Specifies a flag that enables deletion for all new items in a conversation.</span></span>  <br/> |
|[<span data-ttu-id="c9e56-137">Estlu</span><span class="sxs-lookup"><span data-stu-id="c9e56-137">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="c9e56-138">Indique si un message a été lu.</span><span class="sxs-lookup"><span data-stu-id="c9e56-138">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="c9e56-139">DeleType</span><span class="sxs-lookup"><span data-stu-id="c9e56-139">DeleteType</span></span>](deletetype.md) <br/> |<span data-ttu-id="c9e56-140">Indique comment les éléments dans une conversation sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="c9e56-140">Indicates how items in a conversation are deleted.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9e56-141">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c9e56-141">Parent elements</span></span>

|<span data-ttu-id="c9e56-142">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c9e56-142">**Element**</span></span>|<span data-ttu-id="c9e56-143">**Description**</span><span class="sxs-lookup"><span data-stu-id="c9e56-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9e56-144">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="c9e56-144">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="c9e56-145">Contient une collection des conversations et les actions à appliquer à leur.</span><span class="sxs-lookup"><span data-stu-id="c9e56-145">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c9e56-146">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c9e56-146">Text value</span></span>

<span data-ttu-id="c9e56-147">**Valeurs de texte des éléments ConversationAction**</span><span class="sxs-lookup"><span data-stu-id="c9e56-147">**ConversationAction element text values**</span></span>

|<span data-ttu-id="c9e56-148">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="c9e56-148">**Value**</span></span>|<span data-ttu-id="c9e56-149">**Description**</span><span class="sxs-lookup"><span data-stu-id="c9e56-149">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c9e56-150">AlwaysCategorize</span><span class="sxs-lookup"><span data-stu-id="c9e56-150">AlwaysCategorize</span></span>  <br/> |<span data-ttu-id="c9e56-151">Toujours classer la conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-151">Always categorize the conversation.</span></span>  <br/> |
|<span data-ttu-id="c9e56-152">AlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="c9e56-152">AlwaysDelete</span></span>  <br/> |<span data-ttu-id="c9e56-153">Toujours supprimer la conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-153">Always delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="c9e56-154">AlwaysMove</span><span class="sxs-lookup"><span data-stu-id="c9e56-154">AlwaysMove</span></span>  <br/> |<span data-ttu-id="c9e56-155">Toujours déplacer la conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-155">Always move the conversation.</span></span>  <br/> |
|<span data-ttu-id="c9e56-156">Suppression</span><span class="sxs-lookup"><span data-stu-id="c9e56-156">Delete</span></span>  <br/> |<span data-ttu-id="c9e56-157">Supprimer la conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-157">Delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="c9e56-158">Déplacer</span><span class="sxs-lookup"><span data-stu-id="c9e56-158">Move</span></span>  <br/> |<span data-ttu-id="c9e56-159">Déplacer la conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-159">Move the conversation.</span></span>  <br/> |
|<span data-ttu-id="c9e56-160">Copier</span><span class="sxs-lookup"><span data-stu-id="c9e56-160">Copy</span></span>  <br/> |<span data-ttu-id="c9e56-161">Copiez la conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-161">Copy the conversation.</span></span>  <br/> |
|<span data-ttu-id="c9e56-162">SetReadState</span><span class="sxs-lookup"><span data-stu-id="c9e56-162">SetReadState</span></span>  <br/> |<span data-ttu-id="c9e56-163">Définir l’état de lecture de la conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-163">Set the read state of the conversation.</span></span>  <br/> |
|<span data-ttu-id="c9e56-164">SetRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="c9e56-164">SetRetentionPolicy</span></span>  <br/> |<span data-ttu-id="c9e56-165">Définir la stratégie de rétention pour la conversation.</span><span class="sxs-lookup"><span data-stu-id="c9e56-165">Set the retention policy for the conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c9e56-166">Remarques</span><span class="sxs-lookup"><span data-stu-id="c9e56-166">Remarks</span></span>

<span data-ttu-id="c9e56-167">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c9e56-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9e56-168">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c9e56-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9e56-169">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c9e56-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9e56-170">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c9e56-170">Schema Name</span></span>  <br/> |<span data-ttu-id="c9e56-171">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c9e56-171">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9e56-172">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c9e56-172">Validation File</span></span>  <br/> |<span data-ttu-id="c9e56-173">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c9e56-173">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9e56-174">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c9e56-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9e56-175">False</span><span class="sxs-lookup"><span data-stu-id="c9e56-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9e56-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c9e56-176">See also</span></span>



[<span data-ttu-id="c9e56-177">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="c9e56-177">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="c9e56-178">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c9e56-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

