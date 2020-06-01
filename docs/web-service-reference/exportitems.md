---
title: ExportItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItems
api_type:
- schema
ms.assetid: bbbc56e4-8cc1-43ae-b70a-9a8d6bb0f399
description: L’élément ExportItems représente une demande d’exportation d’éléments à partir d’une boîte aux lettres.
ms.openlocfilehash: 6e4996f62ea5051e6dc235ee7255057f16b3855b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457269"
---
# <a name="exportitems"></a><span data-ttu-id="a52f1-103">ExportItems</span><span class="sxs-lookup"><span data-stu-id="a52f1-103">ExportItems</span></span>

<span data-ttu-id="a52f1-104">L’élément **ExportItems** représente une demande d’exportation d’éléments à partir d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a52f1-104">The **ExportItems** element represents a request to export items from a mailbox.</span></span> 
  
[<span data-ttu-id="a52f1-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="a52f1-105">ExportItems</span></span>](exportitems.md)
  
```XML
<ExportItems>
   <ItemIds/>
</ExportItems>
```

 <span data-ttu-id="a52f1-106">**ExportItemsType**</span><span class="sxs-lookup"><span data-stu-id="a52f1-106">**ExportItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a52f1-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a52f1-107">Attributes and elements</span></span>

<span data-ttu-id="a52f1-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a52f1-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a52f1-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="a52f1-109">Attributes</span></span>

<span data-ttu-id="a52f1-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a52f1-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a52f1-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a52f1-111">Child elements</span></span>

|<span data-ttu-id="a52f1-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a52f1-112">**Element**</span></span>|<span data-ttu-id="a52f1-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="a52f1-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a52f1-114">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="a52f1-114">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="a52f1-115">Contient un tableau d’identificateurs d’élément qui identifient les éléments à exporter à partir d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a52f1-115">Contains an array of item identifiers that identify the items to export from a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a52f1-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a52f1-116">Parent elements</span></span>

<span data-ttu-id="a52f1-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a52f1-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a52f1-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a52f1-118">Text value</span></span>

<span data-ttu-id="a52f1-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a52f1-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a52f1-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="a52f1-120">Remarks</span></span>

<span data-ttu-id="a52f1-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a52f1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a52f1-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a52f1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a52f1-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a52f1-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a52f1-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a52f1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a52f1-125">Schéma de message</span><span class="sxs-lookup"><span data-stu-id="a52f1-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="a52f1-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a52f1-126">Validation File</span></span>  <br/> |<span data-ttu-id="a52f1-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a52f1-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a52f1-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a52f1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a52f1-129">False</span><span class="sxs-lookup"><span data-stu-id="a52f1-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a52f1-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a52f1-130">See also</span></span>



[<span data-ttu-id="a52f1-131">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="a52f1-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="a52f1-132">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="a52f1-132">UploadItems operation</span></span>](uploaditems-operation.md)

