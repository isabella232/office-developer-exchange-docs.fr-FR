---
title: FlagStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FlagStatus
api_type:
- schema
ms.assetid: d5907ec5-3a60-4d83-bf85-406c54f95eb7
description: L’élément FlagStatus contient l’état de l’indicateur agrégées pour les éléments de conversation dans le dossier actif.
ms.openlocfilehash: 59e071cbd402c49f4dcc4370059883f3f45409ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756438"
---
# <a name="flagstatus"></a><span data-ttu-id="bd90c-103">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="bd90c-103">FlagStatus</span></span>

<span data-ttu-id="bd90c-104">L’élément **FlagStatus** contient l’état de l’indicateur agrégées pour les éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="bd90c-104">The **FlagStatus** element contains the aggregated flag status for conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="bd90c-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="bd90c-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="bd90c-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="bd90c-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="bd90c-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="bd90c-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="bd90c-108">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="bd90c-108">FlagStatus</span></span>](flagstatus.md)
  
```XML
<FlagStatus> NotFlagged | Flagged | Complete </FlagStatus>
```

 <span data-ttu-id="bd90c-109">**FlagStatusType**</span><span class="sxs-lookup"><span data-stu-id="bd90c-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd90c-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bd90c-110">Attributes and elements</span></span>

<span data-ttu-id="bd90c-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bd90c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd90c-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="bd90c-112">Attributes</span></span>

<span data-ttu-id="bd90c-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bd90c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd90c-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bd90c-114">Child elements</span></span>

<span data-ttu-id="bd90c-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bd90c-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bd90c-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bd90c-116">Parent elements</span></span>

|<span data-ttu-id="bd90c-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bd90c-117">**Element**</span></span>|<span data-ttu-id="bd90c-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="bd90c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd90c-119">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="bd90c-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="bd90c-120">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="bd90c-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bd90c-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bd90c-121">Text value</span></span>

<span data-ttu-id="bd90c-122">La valeur de texte de l’élément **FlagStatus** est l’état de l’indicateur agrégées pour les éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="bd90c-122">The text value of the **FlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="bd90c-123">Les valeurs de texte possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="bd90c-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="bd90c-124">**NotFlagged** - indique l’état n’est pas marqué d’un indicateur.</span><span class="sxs-lookup"><span data-stu-id="bd90c-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="bd90c-125">**Avec indicateur** - indique l’état avec indicateur.</span><span class="sxs-lookup"><span data-stu-id="bd90c-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="bd90c-126">**Complète** - indique l’état de l’indicateur terminée.</span><span class="sxs-lookup"><span data-stu-id="bd90c-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="bd90c-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="bd90c-127">Remarks</span></span>

<span data-ttu-id="bd90c-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="bd90c-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd90c-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bd90c-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd90c-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bd90c-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd90c-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bd90c-131">Schema name</span></span>  <br/> |<span data-ttu-id="bd90c-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bd90c-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd90c-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bd90c-133">Validation file</span></span>  <br/> |<span data-ttu-id="bd90c-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bd90c-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd90c-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bd90c-135">Can be empty</span></span>  <br/> |<span data-ttu-id="bd90c-136">False</span><span class="sxs-lookup"><span data-stu-id="bd90c-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd90c-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bd90c-137">See also</span></span>



[<span data-ttu-id="bd90c-138">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="bd90c-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="bd90c-139">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="bd90c-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="bd90c-140">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="bd90c-140">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)
