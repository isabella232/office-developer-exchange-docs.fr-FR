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
description: L’élément GlobalImportance contient l’importance agrégée de tous les éléments de conversation d’une boîte aux lettres.
ms.openlocfilehash: c760168afa3edac20ca0ae7bc677610d8456d178
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459446"
---
# <a name="globalimportance"></a><span data-ttu-id="445c4-103">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="445c4-103">GlobalImportance</span></span>

<span data-ttu-id="445c4-104">L’élément **GlobalImportance** contient l’importance agrégée de tous les éléments de conversation d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="445c4-104">The **GlobalImportance** element contains the aggregated importance for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="445c4-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="445c4-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="445c4-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="445c4-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="445c4-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="445c4-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="445c4-108">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="445c4-108">GlobalImportance</span></span>](globalimportance.md)
  
```XML
<GlobalImportance> Low | Normal | High </GlobalImportance>
```

 <span data-ttu-id="445c4-109">**ImportanceChoicesType**</span><span class="sxs-lookup"><span data-stu-id="445c4-109">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="445c4-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="445c4-110">Attributes and elements</span></span>

<span data-ttu-id="445c4-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="445c4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="445c4-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="445c4-112">Attributes</span></span>

<span data-ttu-id="445c4-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="445c4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="445c4-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="445c4-114">Child elements</span></span>

<span data-ttu-id="445c4-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="445c4-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="445c4-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="445c4-116">Parent elements</span></span>

|<span data-ttu-id="445c4-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="445c4-117">**Element**</span></span>|<span data-ttu-id="445c4-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="445c4-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="445c4-119">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="445c4-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="445c4-120">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="445c4-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="445c4-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="445c4-121">Text value</span></span>

<span data-ttu-id="445c4-122">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="445c4-122">A text value is required.</span></span> <span data-ttu-id="445c4-123">Les valeurs possibles pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="445c4-123">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="445c4-124">Faible</span><span class="sxs-lookup"><span data-stu-id="445c4-124">Low</span></span>
    
- <span data-ttu-id="445c4-125">Normal</span><span class="sxs-lookup"><span data-stu-id="445c4-125">Normal</span></span>
    
- <span data-ttu-id="445c4-126">Importante</span><span class="sxs-lookup"><span data-stu-id="445c4-126">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="445c4-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="445c4-127">Remarks</span></span>

<span data-ttu-id="445c4-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="445c4-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="445c4-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="445c4-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="445c4-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="445c4-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="445c4-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="445c4-131">Schema name</span></span>  <br/> |<span data-ttu-id="445c4-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="445c4-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="445c4-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="445c4-133">Validation file</span></span>  <br/> |<span data-ttu-id="445c4-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="445c4-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="445c4-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="445c4-135">Can be empty</span></span>  <br/> |<span data-ttu-id="445c4-136">False</span><span class="sxs-lookup"><span data-stu-id="445c4-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="445c4-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="445c4-137">See also</span></span>



[<span data-ttu-id="445c4-138">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="445c4-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="445c4-139">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="445c4-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="445c4-140">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="445c4-140">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

