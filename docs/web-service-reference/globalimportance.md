---
title: GlobalImportance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalImportance
api_type:
- schema
ms.assetid: 8bcec699-e771-4f38-b7d9-61f324af1b4e
description: L’élément GlobalImportance contient l’importance agrégée pour tous les éléments de conversation dans une boîte aux lettres.
ms.openlocfilehash: c9cdcf20fd3e6eca9ab501cbc747544a4d7b7ded
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827731"
---
# <a name="globalimportance"></a><span data-ttu-id="8b020-103">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="8b020-103">GlobalImportance</span></span>

<span data-ttu-id="8b020-104">L’élément **GlobalImportance** contient l’importance agrégée pour tous les éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="8b020-104">The **GlobalImportance** element contains the aggregated importance for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="8b020-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="8b020-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="8b020-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="8b020-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="8b020-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="8b020-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="8b020-108">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="8b020-108">GlobalImportance</span></span>](globalimportance.md)
  
```XML
<GlobalImportance> Low | Normal | High </GlobalImportance>
```

 <span data-ttu-id="8b020-109">**ImportanceChoicesType**</span><span class="sxs-lookup"><span data-stu-id="8b020-109">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b020-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8b020-110">Attributes and elements</span></span>

<span data-ttu-id="8b020-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8b020-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b020-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="8b020-112">Attributes</span></span>

<span data-ttu-id="8b020-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8b020-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b020-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8b020-114">Child elements</span></span>

<span data-ttu-id="8b020-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8b020-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8b020-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8b020-116">Parent elements</span></span>

|<span data-ttu-id="8b020-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8b020-117">**Element**</span></span>|<span data-ttu-id="8b020-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="8b020-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b020-119">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="8b020-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="8b020-120">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="8b020-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8b020-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8b020-121">Text value</span></span>

<span data-ttu-id="8b020-122">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="8b020-122">A text value is required.</span></span> <span data-ttu-id="8b020-123">Les valeurs possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="8b020-123">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="8b020-124">Low</span><span class="sxs-lookup"><span data-stu-id="8b020-124">Low</span></span>
    
- <span data-ttu-id="8b020-125">Normal</span><span class="sxs-lookup"><span data-stu-id="8b020-125">Normal</span></span>
    
- <span data-ttu-id="8b020-126">High</span><span class="sxs-lookup"><span data-stu-id="8b020-126">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="8b020-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="8b020-127">Remarks</span></span>

<span data-ttu-id="8b020-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8b020-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b020-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8b020-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b020-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8b020-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b020-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8b020-131">Schema name</span></span>  <br/> |<span data-ttu-id="8b020-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8b020-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b020-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8b020-133">Validation file</span></span>  <br/> |<span data-ttu-id="8b020-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8b020-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b020-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8b020-135">Can be empty</span></span>  <br/> |<span data-ttu-id="8b020-136">False</span><span class="sxs-lookup"><span data-stu-id="8b020-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b020-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8b020-137">See also</span></span>



[<span data-ttu-id="8b020-138">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="8b020-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="8b020-139">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="8b020-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="8b020-140">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="8b020-140">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

