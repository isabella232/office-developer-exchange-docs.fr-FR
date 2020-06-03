---
title: Condition (RestrictionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdb373e-bf1b-4cb0-bbfb-444c6c6cec50
description: L’élément condition spécifie la condition qui est utilisée pour identifier la fin d’une recherche pour une opération FindItem ou FindConversation.
ms.openlocfilehash: 00c5b5e615ed9b253c79dae9dc2b89c797853089
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463936"
---
# <a name="condition-restrictiontype"></a><span data-ttu-id="d6684-103">Condition (RestrictionType)</span><span class="sxs-lookup"><span data-stu-id="d6684-103">Condition (RestrictionType)</span></span>

<span data-ttu-id="d6684-104">L’élément **condition** spécifie la condition qui est utilisée pour identifier la fin d’une recherche pour une opération **FindItem** ou **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="d6684-104">The **Condition** element specifies the condition that is used to identify the end of a search for a **FindItem** or a **FindConversation** operation.</span></span> 
  
```XML
<Condition>
    <SearchExpression></SearchExpression>
</Condition>
```

 <span data-ttu-id="d6684-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="d6684-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6684-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d6684-106">Attributes and elements</span></span>

<span data-ttu-id="d6684-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d6684-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6684-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d6684-108">Attributes</span></span>

<span data-ttu-id="d6684-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d6684-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6684-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d6684-110">Child elements</span></span>

|<span data-ttu-id="d6684-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d6684-111">**Element**</span></span>|<span data-ttu-id="d6684-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d6684-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6684-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="d6684-113">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="d6684-114">Élément abstrait qui représente l’élément substitué dans une restriction.</span><span class="sxs-lookup"><span data-stu-id="d6684-114">Abstract element that represents the substituted element within a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d6684-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d6684-115">Parent elements</span></span>

|<span data-ttu-id="d6684-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d6684-116">**Element**</span></span>|<span data-ttu-id="d6684-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d6684-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6684-118">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="d6684-118">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="d6684-119">Identifie la condition qui est utilisée pour identifier la fin d’une recherche, l’index de départ d’une recherche, les entrées maximales à renvoyer et l’orientation de la recherche pour une opération **FindItem** ou **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="d6684-119">Identifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or a **FindConversation** operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d6684-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="d6684-120">Remarks</span></span>

<span data-ttu-id="d6684-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d6684-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d6684-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d6684-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6684-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d6684-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6684-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d6684-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6684-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d6684-125">Schema Name</span></span>  <br/> |<span data-ttu-id="d6684-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="d6684-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="d6684-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="d6684-127">Validation File</span></span>  <br/> |<span data-ttu-id="d6684-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="d6684-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6684-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d6684-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d6684-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d6684-130">See also</span></span>



- [<span data-ttu-id="d6684-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d6684-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

