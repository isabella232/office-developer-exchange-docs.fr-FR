---
title: ConversationNodes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c8a35b8-a940-4b3e-8768-9ba95766fd79
description: L’élément ConversationNodes spécifie une collection de nœuds de conversation.
ms.openlocfilehash: 39ffb97f1004535e2fc70b58f8d56afe129e8ee2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461393"
---
# <a name="conversationnodes"></a><span data-ttu-id="2cf82-103">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="2cf82-103">ConversationNodes</span></span>

<span data-ttu-id="2cf82-104">L’élément **ConversationNodes** spécifie une collection de nœuds de conversation.</span><span class="sxs-lookup"><span data-stu-id="2cf82-104">The **ConversationNodes** element specifies a collection of conversation nodes.</span></span> 
  
```XML
<ConversationNodes>
    <ConversationNode></ConversationNode>
</ConversationNodes>
```

 <span data-ttu-id="2cf82-105">**ArrayOfConversationNodesType**</span><span class="sxs-lookup"><span data-stu-id="2cf82-105">**ArrayOfConversationNodesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2cf82-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2cf82-106">Attributes and elements</span></span>

<span data-ttu-id="2cf82-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2cf82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cf82-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2cf82-108">Attributes</span></span>

<span data-ttu-id="2cf82-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2cf82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2cf82-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2cf82-110">Child elements</span></span>

|<span data-ttu-id="2cf82-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2cf82-111">**Element**</span></span>|<span data-ttu-id="2cf82-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2cf82-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cf82-113">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="2cf82-113">ConversationNode</span></span>](conversationnode.md) <br/> |<span data-ttu-id="2cf82-114">Spécifie un nœud dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="2cf82-114">Specifies a node in a conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2cf82-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2cf82-115">Parent elements</span></span>

|<span data-ttu-id="2cf82-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2cf82-116">**Element**</span></span>|<span data-ttu-id="2cf82-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="2cf82-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cf82-118">Conversation (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="2cf82-118">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md) <br/> |<span data-ttu-id="2cf82-119">Représente une conversation unique renvoyée dans une réponse **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="2cf82-119">Represents a single conversation returned in a **GetConversationItems** response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2cf82-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="2cf82-120">Remarks</span></span>

<span data-ttu-id="2cf82-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2cf82-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2cf82-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2cf82-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2cf82-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2cf82-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cf82-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2cf82-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2cf82-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2cf82-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2cf82-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="2cf82-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2cf82-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="2cf82-127">Validation File</span></span>  <br/> |<span data-ttu-id="2cf82-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="2cf82-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2cf82-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2cf82-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2cf82-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2cf82-130">See also</span></span>



- [<span data-ttu-id="2cf82-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2cf82-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

