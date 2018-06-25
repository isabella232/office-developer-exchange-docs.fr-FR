---
title: ItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: 6b82122b-5544-4adf-91b7-ef2db7d5046f
description: L’élément ItemId contient l’identité unique des éléments, des éléments d’occurrence et éléments périodiques maîtres qui servent à supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la banque d’informations Exchange.
ms.openlocfilehash: 1bd4d6f4593a7c3b418561269d8b29707cc6030c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828155"
---
# <a name="itemids"></a><span data-ttu-id="78569-103">ItemIds</span><span class="sxs-lookup"><span data-stu-id="78569-103">ItemIds</span></span>
  
<span data-ttu-id="78569-104">L’élément **ItemId** contient l’identité unique des éléments, des éléments d’occurrence et éléments périodiques maîtres qui servent à supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="78569-104">The **ItemIds** element contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

<span data-ttu-id="78569-105">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="78569-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="78569-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="78569-106">Attributes and elements</span></span>

<span data-ttu-id="78569-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="78569-107">The following sections describe attributes, child elements, and parent elements.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="78569-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="78569-108">Attributes</span></span>

<span data-ttu-id="78569-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="78569-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="78569-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="78569-110">Child elements</span></span>

|<span data-ttu-id="78569-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="78569-111">**Element**</span></span>|<span data-ttu-id="78569-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="78569-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78569-113">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="78569-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="78569-114">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="78569-114">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="78569-115">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="78569-115">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="78569-116">Identifie une seule occurrence d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="78569-116">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="78569-117">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="78569-117">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="78569-118">Identifie un élément de gabarit périodicité en identifiant un des identificateurs des éléments de son occurrence connexes.</span><span class="sxs-lookup"><span data-stu-id="78569-118">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="78569-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="78569-119">Parent elements</span></span>

|<span data-ttu-id="78569-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="78569-120">**Element**</span></span>|<span data-ttu-id="78569-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="78569-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="78569-122">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="78569-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="78569-123">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="78569-123">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="78569-124">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="78569-124">DeleteItem</span></span>](deleteitem.md) <br/> |<span data-ttu-id="78569-125">Définit une demande pour supprimer des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="78569-125">Defines a request to delete items in the Exchange store.</span></span>  <br/> <span data-ttu-id="78569-126">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="78569-126">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteItem` <br/> |
|[<span data-ttu-id="78569-127">SendItem</span><span class="sxs-lookup"><span data-stu-id="78569-127">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="78569-128">L’élément racine qui définit une demande pour envoyer des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="78569-128">The root element that defines a request to send items in the Exchange store.</span></span>  <br/> <span data-ttu-id="78569-129">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="78569-129">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
|[<span data-ttu-id="78569-130">GetItem</span><span class="sxs-lookup"><span data-stu-id="78569-130">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="78569-131">Définit une requête pour obtenir des éléments de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="78569-131">Defines a request to get items from the Exchange store.</span></span>  <br/> <span data-ttu-id="78569-132">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="78569-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="78569-133">MoveItem</span><span class="sxs-lookup"><span data-stu-id="78569-133">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="78569-134">Définit une demande de déplacement d’éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="78569-134">Defines a request to move items in the Exchange store.</span></span>  <br/> <span data-ttu-id="78569-135">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="78569-135">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="78569-136">CopyItem</span><span class="sxs-lookup"><span data-stu-id="78569-136">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="78569-137">Définit une demande pour copier des éléments dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="78569-137">Defines a request to copy items in the Exchange store.</span></span>  <br/> <span data-ttu-id="78569-138">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="78569-138">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="78569-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="78569-139">Remarks</span></span>

<span data-ttu-id="78569-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="78569-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="78569-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="78569-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="78569-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="78569-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="78569-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="78569-143">Schema Name</span></span>  <br/> |<span data-ttu-id="78569-144">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="78569-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="78569-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="78569-145">Validation File</span></span>  <br/> |<span data-ttu-id="78569-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="78569-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="78569-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="78569-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="78569-148">False</span><span class="sxs-lookup"><span data-stu-id="78569-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="78569-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="78569-149">See also</span></span>

- [<span data-ttu-id="78569-150">Opération DeleteItem</span><span class="sxs-lookup"><span data-stu-id="78569-150">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="78569-151">Opération SendItem</span><span class="sxs-lookup"><span data-stu-id="78569-151">SendItem operation</span></span>](senditem-operation.md) 
- [<span data-ttu-id="78569-152">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="78569-152">GetItem operation</span></span>](getitem-operation.md)
- [<span data-ttu-id="78569-153">Opération MoveItem</span><span class="sxs-lookup"><span data-stu-id="78569-153">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="78569-154">Opération CopyItem</span><span class="sxs-lookup"><span data-stu-id="78569-154">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="78569-155">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="78569-155">FindConversation operation</span></span>](findconversation-operation.md)

