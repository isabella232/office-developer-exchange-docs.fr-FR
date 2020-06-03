---
title: Items (NonEmptyArrayOfUploadItemsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: 402bfa6d-11d7-4547-b8bd-197e9922ab49
description: L’élément ITEMS contient un tableau d’éléments à télécharger dans une boîte aux lettres.
ms.openlocfilehash: 5c69134c1613b0a4595a6aa876fa09fde63043ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44441547"
---
# <a name="items-nonemptyarrayofuploaditemstype"></a><span data-ttu-id="5ba50-103">Items (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="5ba50-103">Items (NonEmptyArrayOfUploadItemsType)</span></span>

<span data-ttu-id="5ba50-104">L’élément **Items** contient un tableau d’éléments à télécharger dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5ba50-104">The **Items** element contains an array of items to upload into a mailbox.</span></span> 
  
[<span data-ttu-id="5ba50-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="5ba50-105">UploadItems</span></span>](uploaditems.md)
  
[<span data-ttu-id="5ba50-106">Items (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="5ba50-106">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
  
```XML
<Items>
   <Item/>
</Items>
```

 <span data-ttu-id="5ba50-107">**NonEmptyArrayOfUploadItemsType**</span><span class="sxs-lookup"><span data-stu-id="5ba50-107">**NonEmptyArrayOfUploadItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ba50-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5ba50-108">Attributes and elements</span></span>

<span data-ttu-id="5ba50-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5ba50-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ba50-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="5ba50-110">Attributes</span></span>

<span data-ttu-id="5ba50-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5ba50-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ba50-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5ba50-112">Child elements</span></span>

|<span data-ttu-id="5ba50-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5ba50-113">**Element**</span></span>|<span data-ttu-id="5ba50-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ba50-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ba50-115">Élément (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="5ba50-115">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="5ba50-116">Représente un élément unique à télécharger dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5ba50-116">Represents a single item to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5ba50-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5ba50-117">Parent elements</span></span>

|<span data-ttu-id="5ba50-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5ba50-118">**Element**</span></span>|<span data-ttu-id="5ba50-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ba50-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ba50-120">UploadItems</span><span class="sxs-lookup"><span data-stu-id="5ba50-120">UploadItems</span></span>](uploaditems.md) <br/> |<span data-ttu-id="5ba50-121">Représente une demande de téléchargement d’éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5ba50-121">Represents a request to upload items into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5ba50-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5ba50-122">Text value</span></span>

<span data-ttu-id="5ba50-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5ba50-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5ba50-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="5ba50-124">Remarks</span></span>

<span data-ttu-id="5ba50-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5ba50-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ba50-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5ba50-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ba50-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5ba50-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5ba50-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5ba50-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5ba50-129">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="5ba50-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="5ba50-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5ba50-130">Validation File</span></span>  <br/> |<span data-ttu-id="5ba50-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5ba50-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5ba50-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5ba50-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ba50-133">False</span><span class="sxs-lookup"><span data-stu-id="5ba50-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ba50-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5ba50-134">See also</span></span>



[<span data-ttu-id="5ba50-135">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="5ba50-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="5ba50-136">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="5ba50-136">UploadItems operation</span></span>](uploaditems-operation.md)

