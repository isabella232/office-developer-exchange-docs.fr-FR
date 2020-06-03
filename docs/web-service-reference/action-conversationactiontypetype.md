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
description: L’élément action contient l’action à effectuer sur la conversation spécifiée par l’élément ConversationId.
ms.openlocfilehash: f97b04b98cdc29bee9aff5fa1fc6f37400b8314c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527543"
---
# <a name="action-conversationactiontypetype"></a><span data-ttu-id="f0724-103">Action (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="f0724-103">Action (ConversationActionTypeType)</span></span>

<span data-ttu-id="f0724-104">L’élément **action** contient l’action à effectuer sur la conversation spécifiée par l’élément [ConversationId](conversationid.md) .</span><span class="sxs-lookup"><span data-stu-id="f0724-104">The **Action** element contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> 
  
- [<span data-ttu-id="f0724-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f0724-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
- [<span data-ttu-id="f0724-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="f0724-106">ConversationActions</span></span>](conversationactions.md)
  
- [<span data-ttu-id="f0724-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f0724-107">ConversationAction</span></span>](conversationaction.md)
  
- [<span data-ttu-id="f0724-108">Action (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="f0724-108">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 <span data-ttu-id="f0724-109">**ConversationActionTypeType**</span><span class="sxs-lookup"><span data-stu-id="f0724-109">**ConversationActionTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0724-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f0724-110">Attributes and elements</span></span>

<span data-ttu-id="f0724-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f0724-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0724-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="f0724-112">Attributes</span></span>

<span data-ttu-id="f0724-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f0724-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0724-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f0724-114">Child elements</span></span>

<span data-ttu-id="f0724-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f0724-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f0724-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f0724-116">Parent elements</span></span>

|<span data-ttu-id="f0724-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f0724-117">**Element**</span></span>|<span data-ttu-id="f0724-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="f0724-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0724-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f0724-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="f0724-120">Contient une seule action à appliquer à une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="f0724-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f0724-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f0724-121">Text value</span></span>

<span data-ttu-id="f0724-122">La valeur de texte de l’élément **action** indique l’action à effectuer sur une conversation.</span><span class="sxs-lookup"><span data-stu-id="f0724-122">The text value of the **Action** element indicates which action will be performed on a conversation.</span></span> <span data-ttu-id="f0724-123">Voici les valeurs de texte possibles et les actions correspondantes :</span><span class="sxs-lookup"><span data-stu-id="f0724-123">The following are the possible text values and the corresponding actions:</span></span> 
  
- <span data-ttu-id="f0724-124">**AlwaysCategorize** : les éléments actifs et les nouveaux éléments de la conversation seront automatiquement définis avec les catégories identifiées dans l’élément [categories](categories-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="f0724-124">**AlwaysCategorize** - The current items and new items in the conversation will automatically be set with the categories identified in the [Categories](categories-ex15websvcsotherref.md) element.</span></span> 
    
- <span data-ttu-id="f0724-125">**AlwaysDelete** : les éléments actifs et les nouveaux éléments de la conversation seront automatiquement supprimés.</span><span class="sxs-lookup"><span data-stu-id="f0724-125">**AlwaysDelete** - The current items and new items in the conversation will automatically be deleted.</span></span> <span data-ttu-id="f0724-126">Le mode de suppression est défini par l’élément [DeleteType](deletetype.md) .</span><span class="sxs-lookup"><span data-stu-id="f0724-126">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="f0724-127">**AlwaysMove** : les éléments actifs et les nouveaux éléments de la conversation seront automatiquement déplacés vers le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="f0724-127">**AlwaysMove** - The current items and new items in the conversation will automatically be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> 
    
- <span data-ttu-id="f0724-128">**Supprimer** : les éléments actuels de la conversation seront supprimés.</span><span class="sxs-lookup"><span data-stu-id="f0724-128">**Delete** - The current items in the conversation will be deleted.</span></span> <span data-ttu-id="f0724-129">Les éléments suivants de la conversation ne seront pas supprimés.</span><span class="sxs-lookup"><span data-stu-id="f0724-129">Subsequent items in the conversation will not be deleted.</span></span> <span data-ttu-id="f0724-130">Le mode de suppression est défini par l’élément [DeleteType](deletetype.md) .</span><span class="sxs-lookup"><span data-stu-id="f0724-130">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="f0724-131">**Move** : les éléments actuels de la conversation seront déplacés vers le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="f0724-131">**Move** - The current items in the conversation will be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="f0724-132">Les éléments suivants de la conversation ne seront pas déplacés.</span><span class="sxs-lookup"><span data-stu-id="f0724-132">Subsequent items in the conversation will not be moved.</span></span> 
    
- <span data-ttu-id="f0724-133">**Copier** : les éléments actuels de la conversation seront copiés dans le dossier identifié par l’élément [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="f0724-133">**Copy** - The current items in the conversation will be copied to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="f0724-134">Les éléments suivants de la conversation ne seront pas copiés.</span><span class="sxs-lookup"><span data-stu-id="f0724-134">Subsequent items in the conversation will not be copied.</span></span> 
    
- <span data-ttu-id="f0724-135">**SetReadState** : l’état de lecture est défini pour les éléments actuels de la conversation.</span><span class="sxs-lookup"><span data-stu-id="f0724-135">**SetReadState** - The current items in the conversation will have their read state set.</span></span> <span data-ttu-id="f0724-136">L’état de lecture est défini par l’élément [IsRead](isread.md) .</span><span class="sxs-lookup"><span data-stu-id="f0724-136">The read state is set by the [IsRead](isread.md) element.</span></span> 
    
- <span data-ttu-id="f0724-137">**Flag** : les éléments actuels de la conversation auront un indicateur défini par l’élément [Flag](flag.md) .</span><span class="sxs-lookup"><span data-stu-id="f0724-137">**Flag** - The current items in the conversation will have a flag set as defined by the [Flag](flag.md) element.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="f0724-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="f0724-138">Remarks</span></span>

<span data-ttu-id="f0724-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f0724-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0724-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f0724-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0724-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f0724-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f0724-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f0724-142">Schema Name</span></span>  <br/> |<span data-ttu-id="f0724-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f0724-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="f0724-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f0724-144">Validation File</span></span>  <br/> |<span data-ttu-id="f0724-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f0724-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f0724-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f0724-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0724-147">False</span><span class="sxs-lookup"><span data-stu-id="f0724-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0724-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f0724-148">See also</span></span>

- [<span data-ttu-id="f0724-149">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f0724-149">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="f0724-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f0724-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

