---
title: GlobalItemClasses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalItemClasses
api_type:
- schema
ms.assetid: 72634700-6d75-44c0-80b7-8c31743c04d6
description: L’élément GlobalItemClasses contient une liste de classes d’éléments qui représente toutes les classes d’éléments des éléments de conversation dans une boîte aux lettres.
ms.openlocfilehash: e4cb8a8886f8262e8cb4a550b054e81ea18a5e11
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459432"
---
# <a name="globalitemclasses"></a><span data-ttu-id="6361e-103">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="6361e-103">GlobalItemClasses</span></span>

<span data-ttu-id="6361e-104">L’élément **GlobalItemClasses** contient une liste de classes d’éléments qui représente toutes les classes d’éléments des éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6361e-104">The **GlobalItemClasses** element contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="6361e-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="6361e-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="6361e-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="6361e-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="6361e-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6361e-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="6361e-108">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="6361e-108">GlobalItemClasses</span></span>](globalitemclasses.md)
  
```XML
<GlobalItemClasses>
    <String/>
</GlobalItemClasses>
```

 <span data-ttu-id="6361e-109">**ArrayOfItemClassType**</span><span class="sxs-lookup"><span data-stu-id="6361e-109">**ArrayOfItemClassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6361e-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6361e-110">Attributes and elements</span></span>

<span data-ttu-id="6361e-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6361e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6361e-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="6361e-112">Attributes</span></span>

<span data-ttu-id="6361e-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6361e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6361e-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6361e-114">Child elements</span></span>

|<span data-ttu-id="6361e-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6361e-115">**Element**</span></span>|<span data-ttu-id="6361e-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="6361e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6361e-117">ItemClass</span><span class="sxs-lookup"><span data-stu-id="6361e-117">ItemClass</span></span>](itemclass.md) <br/> |<span data-ttu-id="6361e-118">Représente la classe de message d'un élément.</span><span class="sxs-lookup"><span data-stu-id="6361e-118">Represents the message class of an item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6361e-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6361e-119">Parent elements</span></span>

|<span data-ttu-id="6361e-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6361e-120">**Element**</span></span>|<span data-ttu-id="6361e-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="6361e-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6361e-122">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="6361e-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="6361e-123">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="6361e-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6361e-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6361e-124">Text value</span></span>

<span data-ttu-id="6361e-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6361e-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6361e-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="6361e-126">Remarks</span></span>

<span data-ttu-id="6361e-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6361e-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6361e-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6361e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6361e-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6361e-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6361e-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6361e-130">Schema name</span></span>  <br/> |<span data-ttu-id="6361e-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6361e-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="6361e-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6361e-132">Validation file</span></span>  <br/> |<span data-ttu-id="6361e-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6361e-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6361e-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6361e-134">Can be empty</span></span>  <br/> |<span data-ttu-id="6361e-135">False</span><span class="sxs-lookup"><span data-stu-id="6361e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6361e-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6361e-136">See also</span></span>



[<span data-ttu-id="6361e-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="6361e-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="6361e-138">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="6361e-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="6361e-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="6361e-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

