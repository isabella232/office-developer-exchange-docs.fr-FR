---
title: Condition (RestrictionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdb373e-bf1b-4cb0-bbfb-444c6c6cec50
description: L’élément Condition spécifie la condition qui sert à identifier la fin d’une recherche pour un FindItem ou une opération FindConversation.
ms.openlocfilehash: 513fc21be52a90698f1c292d6d20d7cdaab07371
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755530"
---
# <a name="condition-restrictiontype"></a><span data-ttu-id="94aef-103">Condition (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="94aef-103">Condition (RestrictionType)</span></span>

<span data-ttu-id="94aef-104">L’élément **Condition** spécifie la condition qui sert à identifier la fin d’une recherche pour un **FindItem** ou une opération **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="94aef-104">The **Condition** element specifies the condition that is used to identify the end of a search for a **FindItem** or a **FindConversation** operation.</span></span> 
  
```XML
<Condition>
    <SearchExpression></SearchExpression>
</Condition>
```

 <span data-ttu-id="94aef-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="94aef-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94aef-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="94aef-106">Attributes and elements</span></span>

<span data-ttu-id="94aef-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="94aef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94aef-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="94aef-108">Attributes</span></span>

<span data-ttu-id="94aef-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="94aef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94aef-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="94aef-110">Child elements</span></span>

|<span data-ttu-id="94aef-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="94aef-111">**Element**</span></span>|<span data-ttu-id="94aef-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="94aef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94aef-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="94aef-113">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="94aef-114">Élément abstraite qui représente l’élément substitué au sein d’une restriction.</span><span class="sxs-lookup"><span data-stu-id="94aef-114">Abstract element that represents the substituted element within a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="94aef-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="94aef-115">Parent elements</span></span>

|<span data-ttu-id="94aef-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="94aef-116">**Element**</span></span>|<span data-ttu-id="94aef-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="94aef-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94aef-118">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="94aef-118">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="94aef-119">Identifie la condition est utilisée pour identifier la fin d’une recherche, l’index de début d’une recherche, les entrées maximum pour renvoyer et les instructions de recherche pour une **FindItem** ou une opération **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="94aef-119">Identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or a **FindConversation** operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="94aef-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="94aef-120">Remarks</span></span>

<span data-ttu-id="94aef-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="94aef-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="94aef-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="94aef-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94aef-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="94aef-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94aef-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="94aef-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94aef-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="94aef-125">Schema Name</span></span>  <br/> |<span data-ttu-id="94aef-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="94aef-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="94aef-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="94aef-127">Validation File</span></span>  <br/> |<span data-ttu-id="94aef-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="94aef-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="94aef-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="94aef-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="94aef-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="94aef-130">See also</span></span>



- [<span data-ttu-id="94aef-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="94aef-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

