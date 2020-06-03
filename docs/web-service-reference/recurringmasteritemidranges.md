---
title: RecurringMasterItemIdRanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c9c89b5-4ce8-437b-a332-fa7ed35c8388
description: L’élément RecurringMasterItemIdRanges spécifie un tableau de plages d’occurrences.
ms.openlocfilehash: 784676844c5c58c65b8cc6177843bf26d351b7d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528754"
---
# <a name="recurringmasteritemidranges"></a><span data-ttu-id="95e36-103">RecurringMasterItemIdRanges</span><span class="sxs-lookup"><span data-stu-id="95e36-103">RecurringMasterItemIdRanges</span></span>

<span data-ttu-id="95e36-104">L’élément **RecurringMasterItemIdRanges** spécifie un tableau de plages d’occurrences.</span><span class="sxs-lookup"><span data-stu-id="95e36-104">The **RecurringMasterItemIdRanges** element specifies an array of occurrence ranges.</span></span> 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 <span data-ttu-id="95e36-105">**RecurringMasterItemIdRangesType**</span><span class="sxs-lookup"><span data-stu-id="95e36-105">**RecurringMasterItemIdRangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95e36-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="95e36-106">Attributes and elements</span></span>

<span data-ttu-id="95e36-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="95e36-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95e36-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="95e36-108">Attributes</span></span>

|<span data-ttu-id="95e36-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="95e36-109">**Attribute**</span></span>|<span data-ttu-id="95e36-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="95e36-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="95e36-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="95e36-111">**Id**</span></span> <br/> |<span data-ttu-id="95e36-112">La valeur de texte de l’attribut **ID** est l’identificateur unique de l’élément principal périodique.</span><span class="sxs-lookup"><span data-stu-id="95e36-112">The text value of the **Id** attribute is a recurring master item's unique identifier.</span></span> <span data-ttu-id="95e36-113">Il s’agit d’une valeur de **chaîne** .</span><span class="sxs-lookup"><span data-stu-id="95e36-113">This is a **string** value.</span></span>  <br/> |
|<span data-ttu-id="95e36-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="95e36-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="95e36-115">La valeur de texte de l’attribut **ChangeKey** est la clé de modification de l’élément principal périodique.</span><span class="sxs-lookup"><span data-stu-id="95e36-115">The text value of the **ChangeKey** attribute is the recurring master item's change key.</span></span> <span data-ttu-id="95e36-116">Il s’agit d’une valeur de **chaîne** .</span><span class="sxs-lookup"><span data-stu-id="95e36-116">This is a **string** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="95e36-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="95e36-117">Child elements</span></span>

[<span data-ttu-id="95e36-118">Ranges</span><span class="sxs-lookup"><span data-stu-id="95e36-118">Ranges</span></span>](ranges.md)
  
### <a name="parent-elements"></a><span data-ttu-id="95e36-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="95e36-119">Parent elements</span></span>

<span data-ttu-id="95e36-120">[ItemIds](itemids.md)  |  [GlobalItemIds](globalitemids.md)  |  [DraftItemIds](draftitemids.md)  |  [ContactIds](contactids.md)  |  [ID](groupids.md)</span><span class="sxs-lookup"><span data-stu-id="95e36-120">[ItemIds](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [GroupIds](groupids.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="95e36-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="95e36-121">Remarks</span></span>

<span data-ttu-id="95e36-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="95e36-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="95e36-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="95e36-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95e36-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="95e36-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95e36-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="95e36-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95e36-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="95e36-126">Schema name</span></span>  <br/> |<span data-ttu-id="95e36-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="95e36-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="95e36-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="95e36-128">Validation file</span></span>  <br/> |<span data-ttu-id="95e36-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="95e36-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="95e36-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="95e36-130">Can be empty</span></span>  <br/> ||
   

