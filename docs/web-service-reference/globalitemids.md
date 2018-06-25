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
ms.openlocfilehash: 064ebc4c612aaf569eafa56e57a27cf7153f2130
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827737"
---
# <a name="globalitemids"></a><span data-ttu-id="3c9b1-103">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="3c9b1-103">GlobalItemIds</span></span>

<span data-ttu-id="3c9b1-104">L’élément **GlobalItemIds** contient la collection d’identificateurs d’élément pour tous les éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3c9b1-104">The **GlobalItemIds** element contains the collection of item identifiers for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="3c9b1-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="3c9b1-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="3c9b1-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="3c9b1-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="3c9b1-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3c9b1-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="3c9b1-108">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="3c9b1-108">GlobalItemIds</span></span>](globalitemids.md)
  
```XML
<ItemIds>
   <ItemId/>
   <OccurrenceItemId/>
   <RecurringMasterItemId/>
</ItemIds>
```

 <span data-ttu-id="3c9b1-109">**NonEmptyArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="3c9b1-109">**NonEmptyArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c9b1-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3c9b1-110">Attributes and elements</span></span>

<span data-ttu-id="3c9b1-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3c9b1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c9b1-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="3c9b1-112">Attributes</span></span>

<span data-ttu-id="3c9b1-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3c9b1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c9b1-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3c9b1-114">Child elements</span></span>

|<span data-ttu-id="3c9b1-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3c9b1-115">**Element**</span></span>|<span data-ttu-id="3c9b1-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="3c9b1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c9b1-117">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="3c9b1-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3c9b1-118">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c9b1-118">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3c9b1-119">OccurrenceItemId</span><span class="sxs-lookup"><span data-stu-id="3c9b1-119">OccurrenceItemId</span></span>](occurrenceitemid.md) <br/> |<span data-ttu-id="3c9b1-120">Identifie une seule occurrence d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="3c9b1-120">Identifies a single occurrence of a recurring item.</span></span>  <br/> |
|[<span data-ttu-id="3c9b1-121">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="3c9b1-121">RecurringMasterItemId</span></span>](recurringmasteritemid.md) <br/> |<span data-ttu-id="3c9b1-122">Identifie un élément de gabarit périodicité en identifiant un des identificateurs des éléments de son occurrence connexes.</span><span class="sxs-lookup"><span data-stu-id="3c9b1-122">Identifies a recurrence master item by identifying one of its related occurrence items' identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3c9b1-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3c9b1-123">Parent elements</span></span>

|<span data-ttu-id="3c9b1-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3c9b1-124">**Element**</span></span>|<span data-ttu-id="3c9b1-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="3c9b1-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3c9b1-126">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3c9b1-126">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="3c9b1-127">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="3c9b1-127">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3c9b1-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3c9b1-128">Text value</span></span>

<span data-ttu-id="3c9b1-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3c9b1-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3c9b1-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="3c9b1-130">Remarks</span></span>

<span data-ttu-id="3c9b1-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3c9b1-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c9b1-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3c9b1-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c9b1-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3c9b1-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c9b1-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3c9b1-134">Schema name</span></span>  <br/> |<span data-ttu-id="3c9b1-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3c9b1-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="3c9b1-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3c9b1-136">Validation file</span></span>  <br/> |<span data-ttu-id="3c9b1-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3c9b1-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c9b1-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3c9b1-138">Can be empty</span></span>  <br/> |<span data-ttu-id="3c9b1-139">False</span><span class="sxs-lookup"><span data-stu-id="3c9b1-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c9b1-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3c9b1-140">See also</span></span>



[<span data-ttu-id="3c9b1-141">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="3c9b1-141">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="3c9b1-142">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="3c9b1-142">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="3c9b1-143">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="3c9b1-143">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

