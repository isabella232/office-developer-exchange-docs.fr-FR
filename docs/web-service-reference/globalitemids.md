---
title: GlobalItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalItemIds
api_type:
- schema
ms.assetid: b0f03ce0-a4c3-47de-9360-a880a3606e42
description: L’élément GlobalItemIds contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.
ms.openlocfilehash: aa656e7f2fb78dafe5bf6013c1f7ad14e2372ba1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459425"
---
# <a name="globalitemids"></a><span data-ttu-id="0ebb3-103">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="0ebb3-103">GlobalItemIds</span></span>

<span data-ttu-id="0ebb3-104">L’élément **GlobalItemIds** contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0ebb3-104">The **GlobalItemIds** element contains the collection of item identifiers for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="0ebb3-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="0ebb3-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="0ebb3-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="0ebb3-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="0ebb3-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="0ebb3-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="0ebb3-108">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="0ebb3-108">GlobalItemIds</span></span>](globalitemids.md)
  
```XML
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

 <span data-ttu-id="0ebb3-109">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="0ebb3-109">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ebb3-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0ebb3-110">Attributes and elements</span></span>

<span data-ttu-id="0ebb3-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0ebb3-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ebb3-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="0ebb3-112">Attributes</span></span>

<span data-ttu-id="0ebb3-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0ebb3-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ebb3-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0ebb3-114">Child elements</span></span>

|<span data-ttu-id="0ebb3-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ebb3-115">**Element**</span></span>|<span data-ttu-id="0ebb3-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ebb3-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ebb3-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="0ebb3-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0ebb3-118">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ebb3-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0ebb3-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="0ebb3-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="0ebb3-120">Identifie une seule occurrence d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="0ebb3-120">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="0ebb3-121">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="0ebb3-121">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="0ebb3-122">Identifie un élément de la forme de base de récurrence en identifiant l’un de ses éléments d’occurrences associés.</span><span class="sxs-lookup"><span data-stu-id="0ebb3-122">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ebb3-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0ebb3-123">Parent elements</span></span>

|<span data-ttu-id="0ebb3-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ebb3-124">**Element**</span></span>|<span data-ttu-id="0ebb3-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ebb3-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ebb3-126">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="0ebb3-126">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="0ebb3-127">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="0ebb3-127">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0ebb3-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0ebb3-128">Text value</span></span>

<span data-ttu-id="0ebb3-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0ebb3-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ebb3-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="0ebb3-130">Remarks</span></span>

<span data-ttu-id="0ebb3-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0ebb3-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ebb3-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0ebb3-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ebb3-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0ebb3-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0ebb3-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0ebb3-134">Schema name</span></span>  <br/> |<span data-ttu-id="0ebb3-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0ebb3-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="0ebb3-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0ebb3-136">Validation file</span></span>  <br/> |<span data-ttu-id="0ebb3-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0ebb3-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0ebb3-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0ebb3-138">Can be empty</span></span>  <br/> |<span data-ttu-id="0ebb3-139">False</span><span class="sxs-lookup"><span data-stu-id="0ebb3-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ebb3-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0ebb3-140">See also</span></span>



[<span data-ttu-id="0ebb3-141">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="0ebb3-141">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="0ebb3-142">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="0ebb3-142">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="0ebb3-143">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="0ebb3-143">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

