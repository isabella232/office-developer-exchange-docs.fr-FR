---
title: ItemIds (NonEmptyArrayOfItemIdsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: e895782a-74fe-4216-8ac2-c3c88c4b232d
description: L’élément ItemIds contient un tableau d’identificateurs d’éléments qui identifient les éléments à exporter à partir d’une boîte aux lettres.
ms.openlocfilehash: 16c2633528e2ecbc863cfdde645e0f431b4c4297
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468592"
---
# <a name="itemids-nonemptyarrayofitemidstype"></a><span data-ttu-id="65a4a-103">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="65a4a-103">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>

<span data-ttu-id="65a4a-104">L’élément **ItemIds** contient un tableau d’identificateurs d’éléments qui identifient les éléments à exporter à partir d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="65a4a-104">The **ItemIds** element contains an array of item identifiers that identify the items to export from a mailbox.</span></span> 
  
[<span data-ttu-id="65a4a-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="65a4a-105">ExportItems</span></span>](exportitems.md)
  
[<span data-ttu-id="65a4a-106">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="65a4a-106">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
  
```XML
<ItemIds>
   <ItemId/>
</ItemIds>
```

 <span data-ttu-id="65a4a-107">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="65a4a-107">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65a4a-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="65a4a-108">Attributes and elements</span></span>

<span data-ttu-id="65a4a-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="65a4a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65a4a-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="65a4a-110">Attributes</span></span>

<span data-ttu-id="65a4a-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="65a4a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65a4a-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="65a4a-112">Child elements</span></span>

|<span data-ttu-id="65a4a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65a4a-113">**Element**</span></span>|<span data-ttu-id="65a4a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="65a4a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65a4a-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="65a4a-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="65a4a-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="65a4a-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65a4a-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="65a4a-117">Parent elements</span></span>

|<span data-ttu-id="65a4a-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65a4a-118">**Element**</span></span>|<span data-ttu-id="65a4a-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="65a4a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65a4a-120">ExportItems</span><span class="sxs-lookup"><span data-stu-id="65a4a-120">ExportItems</span></span>](exportitems.md) <br/> |<span data-ttu-id="65a4a-121">Représente une demande d’exportation d’éléments à partir d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="65a4a-121">Represents a request to export items from a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="65a4a-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="65a4a-122">Text value</span></span>

<span data-ttu-id="65a4a-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="65a4a-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="65a4a-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="65a4a-124">Remarks</span></span>

<span data-ttu-id="65a4a-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="65a4a-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65a4a-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="65a4a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65a4a-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="65a4a-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="65a4a-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="65a4a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="65a4a-129">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="65a4a-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="65a4a-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="65a4a-130">Validation File</span></span>  <br/> |<span data-ttu-id="65a4a-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="65a4a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="65a4a-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="65a4a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="65a4a-133">False</span><span class="sxs-lookup"><span data-stu-id="65a4a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65a4a-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65a4a-134">See also</span></span>



[<span data-ttu-id="65a4a-135">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="65a4a-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="65a4a-136">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="65a4a-136">UploadItems operation</span></span>](uploaditems-operation.md)

