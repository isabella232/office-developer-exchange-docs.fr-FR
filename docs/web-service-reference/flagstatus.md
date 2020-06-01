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
description: L’élément FlagStatus contient l’état de l’indicateur agrégé pour les éléments de conversation dans le dossier actif.
ms.openlocfilehash: e65849c4909292c07450f8578fe7a7065c98ab44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466212"
---
# <a name="flagstatus"></a><span data-ttu-id="1e2d0-103">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="1e2d0-103">FlagStatus</span></span>

<span data-ttu-id="1e2d0-104">L’élément **FlagStatus** contient l’état de l’indicateur agrégé pour les éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="1e2d0-104">The **FlagStatus** element contains the aggregated flag status for conversation items in the current folder.</span></span> 
  
[<span data-ttu-id="1e2d0-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="1e2d0-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="1e2d0-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="1e2d0-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="1e2d0-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="1e2d0-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="1e2d0-108">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="1e2d0-108">FlagStatus</span></span>](flagstatus.md)
  
```XML
<FlagStatus> NotFlagged | Flagged | Complete </FlagStatus>
```

 <span data-ttu-id="1e2d0-109">**FlagStatusType**</span><span class="sxs-lookup"><span data-stu-id="1e2d0-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e2d0-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1e2d0-110">Attributes and elements</span></span>

<span data-ttu-id="1e2d0-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1e2d0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e2d0-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="1e2d0-112">Attributes</span></span>

<span data-ttu-id="1e2d0-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1e2d0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e2d0-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1e2d0-114">Child elements</span></span>

<span data-ttu-id="1e2d0-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1e2d0-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1e2d0-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1e2d0-116">Parent elements</span></span>

|<span data-ttu-id="1e2d0-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1e2d0-117">**Element**</span></span>|<span data-ttu-id="1e2d0-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="1e2d0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e2d0-119">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="1e2d0-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="1e2d0-120">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="1e2d0-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1e2d0-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="1e2d0-121">Text value</span></span>

<span data-ttu-id="1e2d0-122">La valeur de texte de l’élément **FlagStatus** est l’état d’indicateur d’agrégation pour les éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="1e2d0-122">The text value of the **FlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="1e2d0-123">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="1e2d0-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="1e2d0-124">**NotFlagged** -indique l’État sans indicateur.</span><span class="sxs-lookup"><span data-stu-id="1e2d0-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="1e2d0-125">**Indicateur** -indique l’état de l’indicateur.</span><span class="sxs-lookup"><span data-stu-id="1e2d0-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="1e2d0-126">**Complete** -indique l’état complet de l’indicateur.</span><span class="sxs-lookup"><span data-stu-id="1e2d0-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="1e2d0-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="1e2d0-127">Remarks</span></span>

<span data-ttu-id="1e2d0-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="1e2d0-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e2d0-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1e2d0-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e2d0-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1e2d0-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1e2d0-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1e2d0-131">Schema name</span></span>  <br/> |<span data-ttu-id="1e2d0-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1e2d0-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="1e2d0-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1e2d0-133">Validation file</span></span>  <br/> |<span data-ttu-id="1e2d0-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1e2d0-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1e2d0-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1e2d0-135">Can be empty</span></span>  <br/> |<span data-ttu-id="1e2d0-136">False</span><span class="sxs-lookup"><span data-stu-id="1e2d0-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e2d0-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1e2d0-137">See also</span></span>



[<span data-ttu-id="1e2d0-138">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="1e2d0-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="1e2d0-139">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="1e2d0-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="1e2d0-140">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="1e2d0-140">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

