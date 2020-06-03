---
title: ConversationNode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b7f7acd3-ed65-441e-9976-8b4ed5f12c0b
description: L’élément ConversationNode spécifie un nœud dans une conversation.
ms.openlocfilehash: 074209c1b5669db8dd1ea4ba7f9dea064628afbd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462702"
---
# <a name="conversationnode"></a><span data-ttu-id="bdbef-103">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="bdbef-103">ConversationNode</span></span>

<span data-ttu-id="bdbef-104">L’élément **ConversationNode** spécifie un nœud dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="bdbef-104">The **ConversationNode** element specifies a node in a conversation.</span></span> 
  
```XML
<ConversationNode>
    <InternetMessageId></InternetMessageId>
    <ParentInternetMessageId></ParentInternetMessageId>
    <Items></Items>
</ConversationNode>
```

 <span data-ttu-id="bdbef-105">**ConversationNodeType**</span><span class="sxs-lookup"><span data-stu-id="bdbef-105">**ConversationNodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bdbef-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bdbef-106">Attributes and elements</span></span>

<span data-ttu-id="bdbef-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bdbef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bdbef-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bdbef-108">Attributes</span></span>

<span data-ttu-id="bdbef-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bdbef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bdbef-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bdbef-110">Child elements</span></span>

|<span data-ttu-id="bdbef-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bdbef-111">**Element**</span></span>|<span data-ttu-id="bdbef-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="bdbef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bdbef-113">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="bdbef-113">InternetMessageId</span></span>](internetmessageid.md) <br/> |<span data-ttu-id="bdbef-114">Représente l’identificateur de message Internet d’un élément.</span><span class="sxs-lookup"><span data-stu-id="bdbef-114">Represents the Internet message identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="bdbef-115">ParentInternetMessageId</span><span class="sxs-lookup"><span data-stu-id="bdbef-115">ParentInternetMessageId</span></span>](parentinternetmessageid.md) <br/> |<span data-ttu-id="bdbef-116">Spécifie l’identificateur du message Internet parent.</span><span class="sxs-lookup"><span data-stu-id="bdbef-116">Specifies the identifier of the parent Internet message.</span></span>  <br/> |
|[<span data-ttu-id="bdbef-117">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="bdbef-117">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="bdbef-118">Spécifie tous les éléments du nœud conversation.</span><span class="sxs-lookup"><span data-stu-id="bdbef-118">Specifies all the items in the conversation node.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bdbef-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bdbef-119">Parent elements</span></span>

|<span data-ttu-id="bdbef-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bdbef-120">**Element**</span></span>|<span data-ttu-id="bdbef-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="bdbef-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bdbef-122">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="bdbef-122">ConversationNodes</span></span>](conversationnodes.md) <br/> |<span data-ttu-id="bdbef-123">Spécifie une collection de nœuds de conversation.</span><span class="sxs-lookup"><span data-stu-id="bdbef-123">Specifies a collection of conversation nodes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bdbef-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="bdbef-124">Remarks</span></span>

<span data-ttu-id="bdbef-125">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bdbef-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bdbef-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bdbef-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bdbef-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bdbef-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bdbef-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bdbef-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bdbef-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bdbef-129">Schema Name</span></span>  <br/> |<span data-ttu-id="bdbef-130">Schéma type</span><span class="sxs-lookup"><span data-stu-id="bdbef-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="bdbef-131">Validation File</span><span class="sxs-lookup"><span data-stu-id="bdbef-131">Validation File</span></span>  <br/> |<span data-ttu-id="bdbef-132">types. xsd</span><span class="sxs-lookup"><span data-stu-id="bdbef-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bdbef-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bdbef-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bdbef-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bdbef-134">See also</span></span>



- [<span data-ttu-id="bdbef-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bdbef-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

