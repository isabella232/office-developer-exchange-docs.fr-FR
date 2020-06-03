---
title: BlockStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 08556ee9-0923-437c-99a4-bb630f04e973
description: L’élément BlockStatus spécifie l’état de blocage d’un élément.
ms.openlocfilehash: e88236274bfa70216e872025c2a94231f837df1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462275"
---
# <a name="blockstatus"></a><span data-ttu-id="0a3b8-103">BlockStatus</span><span class="sxs-lookup"><span data-stu-id="0a3b8-103">BlockStatus</span></span>

<span data-ttu-id="0a3b8-104">L’élément **BlockStatus** spécifie l’état de blocage d’un élément.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-104">The **BlockStatus** element specifies the block status of an item.</span></span> 
  
```XML
<BlockStatus> true | false </BlockStatus
```

 <span data-ttu-id="0a3b8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="0a3b8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a3b8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0a3b8-106">Attributes and elements</span></span>

<span data-ttu-id="0a3b8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a3b8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0a3b8-108">Attributes</span></span>

<span data-ttu-id="0a3b8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a3b8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0a3b8-110">Child elements</span></span>

<span data-ttu-id="0a3b8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0a3b8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0a3b8-112">Parent elements</span></span>

|<span data-ttu-id="0a3b8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0a3b8-113">**Element**</span></span>|<span data-ttu-id="0a3b8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0a3b8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a3b8-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="0a3b8-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="0a3b8-116">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="0a3b8-117">Contact</span><span class="sxs-lookup"><span data-stu-id="0a3b8-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="0a3b8-118">Représente un élément de contact dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0a3b8-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="0a3b8-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="0a3b8-120">Représente une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-120">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="0a3b8-121">Élément</span><span class="sxs-lookup"><span data-stu-id="0a3b8-121">Item</span></span>](item.md) <br/> |<span data-ttu-id="0a3b8-122">Représente un élément générique dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-122">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0a3b8-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0a3b8-123">Text value</span></span>

<span data-ttu-id="0a3b8-124">Une valeur de texte de **true** pour l’élément **BlockStatus** indique qu’un élément est bloqué.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-124">A text value of **true** for the **BlockStatus** element indicates that an item is blocked.</span></span> <span data-ttu-id="0a3b8-125">La valeur **false** indique qu’un élément n’est pas bloqué.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-125">A value of **false** indicates that an item is not blocked.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0a3b8-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="0a3b8-126">Remarks</span></span>

<span data-ttu-id="0a3b8-127">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0a3b8-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a3b8-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a3b8-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0a3b8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a3b8-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0a3b8-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0a3b8-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0a3b8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="0a3b8-132">Schéma type</span><span class="sxs-lookup"><span data-stu-id="0a3b8-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="0a3b8-133">Validation File</span><span class="sxs-lookup"><span data-stu-id="0a3b8-133">Validation File</span></span>  <br/> |<span data-ttu-id="0a3b8-134">types. xsd</span><span class="sxs-lookup"><span data-stu-id="0a3b8-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0a3b8-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0a3b8-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0a3b8-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0a3b8-136">See also</span></span>



- [<span data-ttu-id="0a3b8-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0a3b8-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

