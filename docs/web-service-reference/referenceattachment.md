---
title: ReferenceAttachment
ms.date: 7/7/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b9bde862-6b75-4a81-8033-00a47be4dc2f
description: L’élément ReferenceAttachment spécifie XXX.
ms.openlocfilehash: 10f6cd1e007514300eeefaf5cc9f212cee32f516
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829029"
---
# <a name="referenceattachment"></a><span data-ttu-id="d4bfb-103">ReferenceAttachment</span><span class="sxs-lookup"><span data-stu-id="d4bfb-103">ReferenceAttachment</span></span>

<span data-ttu-id="d4bfb-104">L’élément **ReferenceAttachment** spécifie XXX.</span><span class="sxs-lookup"><span data-stu-id="d4bfb-104">The **ReferenceAttachment** element specifies XXX.</span></span> 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 <span data-ttu-id="d4bfb-105">**ReferenceAttachmen**</span><span class="sxs-lookup"><span data-stu-id="d4bfb-105">**ReferenceAttachmen**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4bfb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4bfb-106">Attributes and elements</span></span>

<span data-ttu-id="d4bfb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4bfb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4bfb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4bfb-108">Attributes</span></span>

|<span data-ttu-id="d4bfb-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="d4bfb-109">**Attribute**</span></span>|<span data-ttu-id="d4bfb-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4bfb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4bfb-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="d4bfb-111">**Id**</span></span> <br/> |<span data-ttu-id="d4bfb-112">La valeur de texte de l’attribut **Id** est l’identificateur unique d’un rendez-vous périodique.</span><span class="sxs-lookup"><span data-stu-id="d4bfb-112">The text value of the **Id** attribute is a recurring master item's unique identifier.</span></span> <span data-ttu-id="d4bfb-113">Il s’agit d’une valeur de **type string** .</span><span class="sxs-lookup"><span data-stu-id="d4bfb-113">This is a **string** value.</span></span>  <br/> |
|<span data-ttu-id="d4bfb-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="d4bfb-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="d4bfb-115">La valeur de texte de l’attribut **ChangeKey** est modifier la clé de l’élément maître périodique.</span><span class="sxs-lookup"><span data-stu-id="d4bfb-115">The text value of the **ChangeKey** attribute is the recurring master item's change key.</span></span> <span data-ttu-id="d4bfb-116">Il s’agit d’une valeur de **type string** .</span><span class="sxs-lookup"><span data-stu-id="d4bfb-116">This is a **string** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d4bfb-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4bfb-117">Child elements</span></span>

<span data-ttu-id="d4bfb-118">Plages</span><span class="sxs-lookup"><span data-stu-id="d4bfb-118">Ranges</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4bfb-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4bfb-119">Parent elements</span></span>

<span data-ttu-id="d4bfb-120">ItemId | GlobalItemIds | DraftItemIds | ContactIds | GroupID</span><span class="sxs-lookup"><span data-stu-id="d4bfb-120">ItemIds | GlobalItemIds | DraftItemIds| ContactIds | GroupIds</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d4bfb-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="d4bfb-121">Remarks</span></span>

<span data-ttu-id="d4bfb-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d4bfb-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d4bfb-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4bfb-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4bfb-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4bfb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4bfb-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4bfb-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4bfb-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4bfb-126">Schema name</span></span>  <br/> |<span data-ttu-id="d4bfb-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d4bfb-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4bfb-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4bfb-128">Validation file</span></span>  <br/> |<span data-ttu-id="d4bfb-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4bfb-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4bfb-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4bfb-130">Can be empty</span></span>  <br/> ||
   

