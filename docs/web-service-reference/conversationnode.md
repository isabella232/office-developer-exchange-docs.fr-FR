---
title: ConversationNode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b7f7acd3-ed65-441e-9976-8b4ed5f12c0b
description: L’élément ConversationNode indique un nœud dans une conversation.
ms.openlocfilehash: c8289e5f30bfd25eb12d54e3be0c561786308dc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755647"
---
# <a name="conversationnode"></a><span data-ttu-id="bcd14-103">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="bcd14-103">ConversationNode</span></span>

<span data-ttu-id="bcd14-104">L’élément **ConversationNode** indique un nœud dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="bcd14-104">The **ConversationNode** element specifies a node in a conversation.</span></span> 
  
```XML
<ConversationNode>
    <InternetMessageId></InternetMessageId>
    <ParentInternetMessageId></ParentInternetMessageId>
    <Items></Items>
</ConversationNode>
```

 <span data-ttu-id="bcd14-105">**ConversationNodeType**</span><span class="sxs-lookup"><span data-stu-id="bcd14-105">**ConversationNodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bcd14-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bcd14-106">Attributes and elements</span></span>

<span data-ttu-id="bcd14-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bcd14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bcd14-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bcd14-108">Attributes</span></span>

<span data-ttu-id="bcd14-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bcd14-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bcd14-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bcd14-110">Child elements</span></span>

|<span data-ttu-id="bcd14-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bcd14-111">**Element**</span></span>|<span data-ttu-id="bcd14-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="bcd14-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcd14-113">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="bcd14-113">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="bcd14-114">Représente l’identificateur de message Internet d’un élément.</span><span class="sxs-lookup"><span data-stu-id="bcd14-114">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="bcd14-115">ParentInternetMessageId</span><span class="sxs-lookup"><span data-stu-id="bcd14-115">ParentInternetMessageId</span></span>](parentinternetmessageid.md) <br/> |<span data-ttu-id="bcd14-116">Spécifie l’identificateur du message Internet parent.</span><span class="sxs-lookup"><span data-stu-id="bcd14-116">Specifies the identifier of the parent Internet message.</span></span>  <br/> |
|[<span data-ttu-id="bcd14-117">ItemId (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="bcd14-117">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="bcd14-118">Spécifie tous les éléments dans le nœud de la conversation.</span><span class="sxs-lookup"><span data-stu-id="bcd14-118">Specifies all the items in the conversation node.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bcd14-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bcd14-119">Parent elements</span></span>

|<span data-ttu-id="bcd14-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bcd14-120">**Element**</span></span>|<span data-ttu-id="bcd14-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="bcd14-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcd14-122">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="bcd14-122">ConversationNodes</span></span>](conversationnodes.md) <br/> |<span data-ttu-id="bcd14-123">Spécifie une collection de nœuds de la conversation.</span><span class="sxs-lookup"><span data-stu-id="bcd14-123">Specifies a collection of conversation nodes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bcd14-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="bcd14-124">Remarks</span></span>

<span data-ttu-id="bcd14-125">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bcd14-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bcd14-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcd14-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bcd14-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bcd14-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bcd14-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bcd14-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bcd14-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bcd14-129">Schema Name</span></span>  <br/> |<span data-ttu-id="bcd14-130">Schéma type</span><span class="sxs-lookup"><span data-stu-id="bcd14-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="bcd14-131">Validation File</span><span class="sxs-lookup"><span data-stu-id="bcd14-131">Validation File</span></span>  <br/> |<span data-ttu-id="bcd14-132">types.xsd</span><span class="sxs-lookup"><span data-stu-id="bcd14-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bcd14-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bcd14-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bcd14-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bcd14-134">See also</span></span>



- [<span data-ttu-id="bcd14-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bcd14-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

