---
title: Action (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: L’élément Action contient l’action à effectuer sur la conversation spécifiée par l’élément ConversationId.
ms.openlocfilehash: b468eeaf0c2509bfa53cbd83f497f0bae20a7f68
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755149"
---
# <a name="action-conversationactiontypetype"></a><span data-ttu-id="f208e-103">Action (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="f208e-103">Action (ConversationActionTypeType)</span></span>

<span data-ttu-id="f208e-104">L’élément **Action** contient l’action à effectuer sur la conversation spécifiée par l’élément [ConversationId](conversationid.md) .</span><span class="sxs-lookup"><span data-stu-id="f208e-104">The **Action** element contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> 
  
- [<span data-ttu-id="f208e-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f208e-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
- [<span data-ttu-id="f208e-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="f208e-106">ConversationActions</span></span>](conversationactions.md)
  
- [<span data-ttu-id="f208e-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f208e-107">ConversationAction</span></span>](conversationaction.md)
  
- [<span data-ttu-id="f208e-108">Action (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="f208e-108">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 <span data-ttu-id="f208e-109">**ConversationActionTypeType**</span><span class="sxs-lookup"><span data-stu-id="f208e-109">**ConversationActionTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f208e-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f208e-110">Attributes and elements</span></span>

<span data-ttu-id="f208e-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f208e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f208e-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="f208e-112">Attributes</span></span>

<span data-ttu-id="f208e-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f208e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f208e-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f208e-114">Child elements</span></span>

<span data-ttu-id="f208e-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f208e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f208e-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f208e-116">Parent elements</span></span>

|<span data-ttu-id="f208e-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f208e-117">**Element**</span></span>|<span data-ttu-id="f208e-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="f208e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f208e-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f208e-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="f208e-120">Contient une seule action à appliquer à une même conversation.</span><span class="sxs-lookup"><span data-stu-id="f208e-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f208e-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="f208e-121">Text value</span></span>

<span data-ttu-id="f208e-122">La valeur de texte de l’élément **Action** indique l’action qui sera effectuée sur une conversation.</span><span class="sxs-lookup"><span data-stu-id="f208e-122">The text value of the **Action** element indicates which action will be performed on a conversation.</span></span> <span data-ttu-id="f208e-123">Voici les valeurs possibles de texte et les actions correspondantes :</span><span class="sxs-lookup"><span data-stu-id="f208e-123">The following are the possible text values and the corresponding actions:</span></span> 
  
- <span data-ttu-id="f208e-124">**AlwaysCategorize** - les éléments en cours et les nouveaux éléments de la conversation sera automatiquement défini avec les catégories identifiés dans l’élément de [catégories](categories-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="f208e-124">**AlwaysCategorize** - The current items and new items in the conversation will automatically be set with the categories identified in the [Categories](categories-ex15websvcsotherref.md) element.</span></span> 
    
- <span data-ttu-id="f208e-125">**AlwaysDelete** - les éléments en cours et les nouveaux éléments de la conversation seront automatiquement supprimés.</span><span class="sxs-lookup"><span data-stu-id="f208e-125">**AlwaysDelete** - The current items and new items in the conversation will automatically be deleted.</span></span> <span data-ttu-id="f208e-126">Le mode de suppression est défini par l’élément [DeleType](deletetype.md) .</span><span class="sxs-lookup"><span data-stu-id="f208e-126">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="f208e-127">**AlwaysMove** - les éléments en cours et les nouveaux éléments de la conversation seront automatiquement déplacées vers le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="f208e-127">**AlwaysMove** - The current items and new items in the conversation will automatically be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> 
    
- <span data-ttu-id="f208e-128">**Supprimer** : les éléments en cours de la conversation seront supprimés.</span><span class="sxs-lookup"><span data-stu-id="f208e-128">**Delete** - The current items in the conversation will be deleted.</span></span> <span data-ttu-id="f208e-129">Les éléments suivants dans la conversation ne seront pas supprimés.</span><span class="sxs-lookup"><span data-stu-id="f208e-129">Subsequent items in the conversation will not be deleted.</span></span> <span data-ttu-id="f208e-130">Le mode de suppression est défini par l’élément [DeleType](deletetype.md) .</span><span class="sxs-lookup"><span data-stu-id="f208e-130">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="f208e-131">**Déplacer** - les éléments en cours de la conversation seront déplacées vers le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="f208e-131">**Move** - The current items in the conversation will be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="f208e-132">Les éléments suivants dans la conversation ne seront déplacées.</span><span class="sxs-lookup"><span data-stu-id="f208e-132">Subsequent items in the conversation will not be moved.</span></span> 
    
- <span data-ttu-id="f208e-133">**Copie** - les éléments en cours de la conversation sont copiées dans le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="f208e-133">**Copy** - The current items in the conversation will be copied to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="f208e-134">Dans la conversation, les éléments suivants ne sont pas copiés.</span><span class="sxs-lookup"><span data-stu-id="f208e-134">Subsequent items in the conversation will not be copied.</span></span> 
    
- <span data-ttu-id="f208e-135">**SetReadState** - les éléments de la conversation en cours aura leur état en lecture à définir.</span><span class="sxs-lookup"><span data-stu-id="f208e-135">**SetReadState** - The current items in the conversation will have their read state set.</span></span> <span data-ttu-id="f208e-136">L’état de lecture est défini par l’élément [estlu](isread.md) .</span><span class="sxs-lookup"><span data-stu-id="f208e-136">The read state is set by the [IsRead](isread.md) element.</span></span> 
    
- <span data-ttu-id="f208e-137">**Indicateur** : les éléments de la conversation en cours aura un indicateur tel que défini par l’élément [indicateur](flag.md) .</span><span class="sxs-lookup"><span data-stu-id="f208e-137">**Flag** - The current items in the conversation will have a flag set as defined by the [Flag](flag.md) element.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="f208e-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="f208e-138">Remarks</span></span>

<span data-ttu-id="f208e-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f208e-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f208e-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f208e-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f208e-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f208e-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f208e-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f208e-142">Schema Name</span></span>  <br/> |<span data-ttu-id="f208e-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f208e-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="f208e-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f208e-144">Validation File</span></span>  <br/> |<span data-ttu-id="f208e-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f208e-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f208e-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f208e-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="f208e-147">False</span><span class="sxs-lookup"><span data-stu-id="f208e-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f208e-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f208e-148">See also</span></span>

- [<span data-ttu-id="f208e-149">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f208e-149">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="f208e-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f208e-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

