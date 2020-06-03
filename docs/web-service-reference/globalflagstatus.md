---
title: GlobalFlagStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalFlagStatus
api_type:
- schema
ms.assetid: 3ba300f3-3355-4cab-9e77-0dcc2902e712
description: L’élément GlobalFlagStatus contient l’état de l’indicateur agrégé pour tous les éléments de conversation dans une boîte aux lettres.
ms.openlocfilehash: f9984a1bb7e8205a98dd3ef91f841b48a7ab9389
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459503"
---
# <a name="globalflagstatus"></a><span data-ttu-id="4e633-103">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="4e633-103">GlobalFlagStatus</span></span>

<span data-ttu-id="4e633-104">L’élément **GlobalFlagStatus** contient l’état de l’indicateur agrégé pour tous les éléments de conversation dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4e633-104">The **GlobalFlagStatus** element contains the aggregated flag status for all conversation items in a mailbox.</span></span> 
  
[<span data-ttu-id="4e633-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="4e633-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="4e633-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="4e633-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="4e633-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="4e633-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="4e633-108">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="4e633-108">GlobalFlagStatus</span></span>](globalflagstatus.md)
  
```XML
<GlobalFlagStatus> NotFlagged | Flagged | Complete </GlobalFlagStatus>
```

 <span data-ttu-id="4e633-109">**FlagStatusType**</span><span class="sxs-lookup"><span data-stu-id="4e633-109">**FlagStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4e633-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4e633-110">Attributes and elements</span></span>

<span data-ttu-id="4e633-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4e633-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e633-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="4e633-112">Attributes</span></span>

<span data-ttu-id="4e633-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4e633-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4e633-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4e633-114">Child elements</span></span>

<span data-ttu-id="4e633-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4e633-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4e633-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4e633-116">Parent elements</span></span>

|<span data-ttu-id="4e633-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4e633-117">**Element**</span></span>|<span data-ttu-id="4e633-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="4e633-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e633-119">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="4e633-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="4e633-120">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="4e633-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4e633-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4e633-121">Text value</span></span>

<span data-ttu-id="4e633-122">La valeur de texte de l’élément **GlobalFlagStatus** est l’état d’indicateur d’agrégation pour les éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="4e633-122">The text value of the **GlobalFlagStatus** element is the aggregated flag status for conversation items in the current folder.</span></span> <span data-ttu-id="4e633-123">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="4e633-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="4e633-124">**NotFlagged** -indique l’État sans indicateur.</span><span class="sxs-lookup"><span data-stu-id="4e633-124">**NotFlagged** - Indicates the not-flagged status.</span></span> 
    
- <span data-ttu-id="4e633-125">**Indicateur** -indique l’état de l’indicateur.</span><span class="sxs-lookup"><span data-stu-id="4e633-125">**Flagged** - Indicates the flagged status.</span></span> 
    
- <span data-ttu-id="4e633-126">**Complete** -indique l’état complet de l’indicateur.</span><span class="sxs-lookup"><span data-stu-id="4e633-126">**Complete** - Indicates the complete flag status.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="4e633-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="4e633-127">Remarks</span></span>

<span data-ttu-id="4e633-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4e633-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4e633-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4e633-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e633-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4e633-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4e633-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4e633-131">Schema name</span></span>  <br/> |<span data-ttu-id="4e633-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4e633-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="4e633-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4e633-133">Validation file</span></span>  <br/> |<span data-ttu-id="4e633-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4e633-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4e633-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4e633-135">Can be empty</span></span>  <br/> |<span data-ttu-id="4e633-136">False</span><span class="sxs-lookup"><span data-stu-id="4e633-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e633-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4e633-137">See also</span></span>



[<span data-ttu-id="4e633-138">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="4e633-138">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="4e633-139">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="4e633-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="4e633-140">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="4e633-140">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

