---
title: SortOrder (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: L’élément SortOrder Spécifie l’ordre de tri pour le résultat d’une demande GetConversationItems.
ms.openlocfilehash: 397aead62d32e72f991af783bff02e79a6e4b0fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829520"
---
# <a name="sortorder-conversationnodesortorder"></a><span data-ttu-id="488af-103">SortOrder (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="488af-103">SortOrder (ConversationNodeSortOrder)</span></span>

<span data-ttu-id="488af-104">L’élément **SortOrder** Spécifie l’ordre de tri pour le résultat d’une demande **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="488af-104">The **SortOrder** element specifies the sort order used for the result of a **GetConversationItems** request.</span></span> 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 <span data-ttu-id="488af-105">**ConversationNodeSortOrder**</span><span class="sxs-lookup"><span data-stu-id="488af-105">**ConversationNodeSortOrder**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="488af-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="488af-106">Attributes and elements</span></span>

<span data-ttu-id="488af-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="488af-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="488af-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="488af-108">Attributes</span></span>

<span data-ttu-id="488af-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="488af-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="488af-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="488af-110">Child elements</span></span>

<span data-ttu-id="488af-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="488af-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="488af-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="488af-112">Parent elements</span></span>

[<span data-ttu-id="488af-113">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="488af-113">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="text-value"></a><span data-ttu-id="488af-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="488af-114">Text value</span></span>

<span data-ttu-id="488af-115">La valeur de texte de l’élément **SortOrder** est l’ordre dans lequel les conversations commandée.</span><span class="sxs-lookup"><span data-stu-id="488af-115">The text value of the **SortOrder** element is the order in which conversations ordered.</span></span> <span data-ttu-id="488af-116">Une valeur texte **TreeOrderAscending** indique que les conversations sont triées en fonction de l’arborescence de la conversation dans l’ordre croissant.</span><span class="sxs-lookup"><span data-stu-id="488af-116">A text value of **TreeOrderAscending** indicates that the conversations are ordered according to the conversation tree in ascending order.</span></span> <span data-ttu-id="488af-117">Une valeur texte **TreeOrderDescending** indique que les conversations sont triées en fonction de l’arborescence de la conversation dans l’ordre décroissant.</span><span class="sxs-lookup"><span data-stu-id="488af-117">A text value of **TreeOrderDescending** indicates that the conversations are ordered according to the conversation tree in descending order.</span></span> <span data-ttu-id="488af-118">Une valeur texte **DateOrderAscending** indique que les conversations sont triées en fonction de la date de la conversation dans l’ordre croissant.</span><span class="sxs-lookup"><span data-stu-id="488af-118">A text value of **DateOrderAscending** indicates that the conversations are ordered according to the conversation date in ascending order.</span></span> <span data-ttu-id="488af-119">Une valeur texte **DateOrderDescending** indique que les conversations sont triées en fonction de la date de la conversation dans l’ordre décroissant.</span><span class="sxs-lookup"><span data-stu-id="488af-119">A text value of **DateOrderDescending** indicates that the conversations are ordered according to the conversation date in descending order.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="488af-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="488af-120">Remarks</span></span>

<span data-ttu-id="488af-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="488af-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="488af-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="488af-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="488af-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="488af-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="488af-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="488af-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="488af-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="488af-125">Schema name</span></span>  <br/> |<span data-ttu-id="488af-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="488af-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="488af-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="488af-127">Validation file</span></span>  <br/> |<span data-ttu-id="488af-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="488af-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="488af-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="488af-129">Can be empty</span></span>  <br/> ||
   

