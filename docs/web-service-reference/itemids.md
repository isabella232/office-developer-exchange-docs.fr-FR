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
description: L’élément ItemIds contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Banque d’Exchange.
ms.openlocfilehash: bbd594ce2610bd625b0e16a0383fda552ee9eb19
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460602"
---
# <a name="itemids"></a><span data-ttu-id="f1105-103">ItemIds</span><span class="sxs-lookup"><span data-stu-id="f1105-103">ItemIds</span></span>
  
<span data-ttu-id="f1105-104">L’élément **ItemIds** contient les identités uniques des éléments, des éléments d’occurrence et des éléments principaux périodiques qui sont utilisés pour supprimer, envoyer, obtenir, déplacer ou copier des éléments dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1105-104">The **ItemIds** element contains the unique identities of items, occurrence items, and recurring master items that are used to delete, send, get, move, or copy items in the Exchange store.</span></span>
  
```xml
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

<span data-ttu-id="f1105-105">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="f1105-105">**NonEmptyArrayOfBaseItemIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f1105-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f1105-106">Attributes and elements</span></span>

<span data-ttu-id="f1105-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f1105-107">The following sections describe attributes, child elements, and parent elements.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="f1105-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f1105-108">Attributes</span></span>

<span data-ttu-id="f1105-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f1105-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1105-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f1105-110">Child elements</span></span>

|<span data-ttu-id="f1105-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1105-111">**Element**</span></span>|<span data-ttu-id="f1105-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1105-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1105-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="f1105-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="f1105-114">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1105-114">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f1105-115">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="f1105-115">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="f1105-116">Identifie une seule occurrence d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="f1105-116">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="f1105-117">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="f1105-117">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="f1105-118">Identifie un élément de la forme de base de récurrence en identifiant l’un de ses éléments d’occurrences associés.</span><span class="sxs-lookup"><span data-stu-id="f1105-118">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1105-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f1105-119">Parent elements</span></span>

|<span data-ttu-id="f1105-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1105-120">**Element**</span></span>|<span data-ttu-id="f1105-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1105-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1105-122">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f1105-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="f1105-123">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="f1105-123">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="f1105-124">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="f1105-124">DeleteItem</span></span>](deleteitem.md) <br/> |<span data-ttu-id="f1105-125">Définit une demande de suppression d’éléments dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1105-125">Defines a request to delete items in the Exchange store.</span></span>  <br/> <span data-ttu-id="f1105-126">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="f1105-126">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteItem` <br/> |
|[<span data-ttu-id="f1105-127">SendItem</span><span class="sxs-lookup"><span data-stu-id="f1105-127">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="f1105-128">Élément racine qui définit une demande d’envoi d’éléments dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1105-128">The root element that defines a request to send items in the Exchange store.</span></span>  <br/> <span data-ttu-id="f1105-129">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="f1105-129">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
|[<span data-ttu-id="f1105-130">GetItem</span><span class="sxs-lookup"><span data-stu-id="f1105-130">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="f1105-131">Définit une demande d’obtention d’éléments à partir de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1105-131">Defines a request to get items from the Exchange store.</span></span>  <br/> <span data-ttu-id="f1105-132">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="f1105-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="f1105-133">MoveItem</span><span class="sxs-lookup"><span data-stu-id="f1105-133">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="f1105-134">Définit une demande de déplacement d’éléments dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1105-134">Defines a request to move items in the Exchange store.</span></span>  <br/> <span data-ttu-id="f1105-135">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="f1105-135">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="f1105-136">CopyItem</span><span class="sxs-lookup"><span data-stu-id="f1105-136">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="f1105-137">Définit une demande de copie des éléments dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1105-137">Defines a request to copy items in the Exchange store.</span></span>  <br/> <span data-ttu-id="f1105-138">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="f1105-138">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f1105-139">Remarques</span><span class="sxs-lookup"><span data-stu-id="f1105-139">Remarks</span></span>

<span data-ttu-id="f1105-140">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1105-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1105-141">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f1105-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1105-142">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f1105-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f1105-143">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f1105-143">Schema Name</span></span>  <br/> |<span data-ttu-id="f1105-144">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="f1105-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f1105-145">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f1105-145">Validation File</span></span>  <br/> |<span data-ttu-id="f1105-146">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f1105-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f1105-147">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f1105-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1105-148">False</span><span class="sxs-lookup"><span data-stu-id="f1105-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1105-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1105-149">See also</span></span>

- [<span data-ttu-id="f1105-150">Opération DeleteItem</span><span class="sxs-lookup"><span data-stu-id="f1105-150">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="f1105-151">Opération SendItem</span><span class="sxs-lookup"><span data-stu-id="f1105-151">SendItem operation</span></span>](senditem-operation.md) 
- [<span data-ttu-id="f1105-152">Opération GetItem</span><span class="sxs-lookup"><span data-stu-id="f1105-152">GetItem operation</span></span>](getitem-operation.md)
- [<span data-ttu-id="f1105-153">Opération MoveItem</span><span class="sxs-lookup"><span data-stu-id="f1105-153">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="f1105-154">Opération CopyItem</span><span class="sxs-lookup"><span data-stu-id="f1105-154">CopyItem operation</span></span>](copyitem-operation.md)
- [<span data-ttu-id="f1105-155">Opération FindConversation</span><span class="sxs-lookup"><span data-stu-id="f1105-155">FindConversation operation</span></span>](findconversation-operation.md)

