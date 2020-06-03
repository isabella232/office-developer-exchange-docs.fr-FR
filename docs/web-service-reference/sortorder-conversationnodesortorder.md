---
title: OrdreTri (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: L’élément SortOrder spécifie l’ordre de tri utilisé pour le résultat d’une demande GetConversationItems.
ms.openlocfilehash: 69d362b9f769749bcc9692825b64ff486e8b60a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530964"
---
# <a name="sortorder-conversationnodesortorder"></a><span data-ttu-id="26fd8-103">OrdreTri (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="26fd8-103">SortOrder (ConversationNodeSortOrder)</span></span>

<span data-ttu-id="26fd8-104">L’élément **SortOrder** spécifie l’ordre de tri utilisé pour le résultat d’une demande **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="26fd8-104">The **SortOrder** element specifies the sort order used for the result of a **GetConversationItems** request.</span></span> 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 <span data-ttu-id="26fd8-105">**ConversationNodeSortOrder**</span><span class="sxs-lookup"><span data-stu-id="26fd8-105">**ConversationNodeSortOrder**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26fd8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="26fd8-106">Attributes and elements</span></span>

<span data-ttu-id="26fd8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="26fd8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26fd8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="26fd8-108">Attributes</span></span>

<span data-ttu-id="26fd8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="26fd8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26fd8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="26fd8-110">Child elements</span></span>

<span data-ttu-id="26fd8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="26fd8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26fd8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="26fd8-112">Parent elements</span></span>

[<span data-ttu-id="26fd8-113">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="26fd8-113">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="text-value"></a><span data-ttu-id="26fd8-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="26fd8-114">Text value</span></span>

<span data-ttu-id="26fd8-115">La valeur de texte de l’élément **SortOrder** est l’ordre dans lequel les conversations sont ordonnées.</span><span class="sxs-lookup"><span data-stu-id="26fd8-115">The text value of the **SortOrder** element is the order in which conversations ordered.</span></span> <span data-ttu-id="26fd8-116">Une valeur de texte de **TreeOrderAscending** indique que les conversations sont classées en fonction de l’arborescence de conversation dans l’ordre croissant.</span><span class="sxs-lookup"><span data-stu-id="26fd8-116">A text value of **TreeOrderAscending** indicates that the conversations are ordered according to the conversation tree in ascending order.</span></span> <span data-ttu-id="26fd8-117">Une valeur de texte de **TreeOrderDescending** indique que les conversations sont classées en fonction de l’arborescence de conversation dans l’ordre décroissant.</span><span class="sxs-lookup"><span data-stu-id="26fd8-117">A text value of **TreeOrderDescending** indicates that the conversations are ordered according to the conversation tree in descending order.</span></span> <span data-ttu-id="26fd8-118">Une valeur de texte de **DateOrderAscending** indique que les conversations sont classées en fonction de la date de conversation dans l’ordre croissant.</span><span class="sxs-lookup"><span data-stu-id="26fd8-118">A text value of **DateOrderAscending** indicates that the conversations are ordered according to the conversation date in ascending order.</span></span> <span data-ttu-id="26fd8-119">Une valeur de texte de **DateOrderDescending** indique que les conversations sont classées en fonction de la date de conversation dans l’ordre décroissant.</span><span class="sxs-lookup"><span data-stu-id="26fd8-119">A text value of **DateOrderDescending** indicates that the conversations are ordered according to the conversation date in descending order.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="26fd8-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="26fd8-120">Remarks</span></span>

<span data-ttu-id="26fd8-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="26fd8-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="26fd8-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="26fd8-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26fd8-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="26fd8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26fd8-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="26fd8-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="26fd8-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="26fd8-125">Schema name</span></span>  <br/> |<span data-ttu-id="26fd8-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="26fd8-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="26fd8-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="26fd8-127">Validation file</span></span>  <br/> |<span data-ttu-id="26fd8-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="26fd8-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="26fd8-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="26fd8-129">Can be empty</span></span>  <br/> ||
   

