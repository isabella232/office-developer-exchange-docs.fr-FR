---
title: ConversationNodes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c8a35b8-a940-4b3e-8768-9ba95766fd79
description: L’élément ConversationNodes spécifie une collection de nœuds de la conversation.
ms.openlocfilehash: 62ec061f6d03abb9db7e511722e5570e70d65772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755656"
---
# <a name="conversationnodes"></a><span data-ttu-id="b8441-103">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="b8441-103">ConversationNodes</span></span>

<span data-ttu-id="b8441-104">L’élément **ConversationNodes** spécifie une collection de nœuds de la conversation.</span><span class="sxs-lookup"><span data-stu-id="b8441-104">The **ConversationNodes** element specifies a collection of conversation nodes.</span></span> 
  
```XML
<ConversationNodes>
    <ConversationNode></ConversationNode>
</ConversationNodes>
```

 <span data-ttu-id="b8441-105">**ArrayOfConversationNodesType**</span><span class="sxs-lookup"><span data-stu-id="b8441-105">**ArrayOfConversationNodesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8441-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b8441-106">Attributes and elements</span></span>

<span data-ttu-id="b8441-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b8441-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8441-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b8441-108">Attributes</span></span>

<span data-ttu-id="b8441-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b8441-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8441-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b8441-110">Child elements</span></span>

|<span data-ttu-id="b8441-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b8441-111">**Element**</span></span>|<span data-ttu-id="b8441-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b8441-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8441-113">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="b8441-113">ConversationNode</span></span>](conversationnode.md) <br/> |<span data-ttu-id="b8441-114">Spécifie un nœud dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="b8441-114">Specifies a node in a conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b8441-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b8441-115">Parent elements</span></span>

|<span data-ttu-id="b8441-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b8441-116">**Element**</span></span>|<span data-ttu-id="b8441-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b8441-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8441-118">Conversation (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="b8441-118">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="b8441-119">Représente une seule conversation renvoyée dans une réponse **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="b8441-119">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b8441-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="b8441-120">Remarks</span></span>

<span data-ttu-id="b8441-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b8441-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b8441-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b8441-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8441-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b8441-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8441-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b8441-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b8441-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b8441-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b8441-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="b8441-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b8441-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="b8441-127">Validation File</span></span>  <br/> |<span data-ttu-id="b8441-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="b8441-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b8441-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b8441-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b8441-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b8441-130">See also</span></span>



- [<span data-ttu-id="b8441-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b8441-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

