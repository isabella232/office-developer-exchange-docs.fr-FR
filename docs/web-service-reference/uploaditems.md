---
title: UploadItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItems
api_type:
- schema
ms.assetid: fd2b9545-7213-4427-95ae-71a155b75971
description: L’élément UploadItems représente une demande de télécharger des éléments dans une boîte aux lettres.
ms.openlocfilehash: d3cd69cdb744431daeede736c2e156c8ab92a79b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838924"
---
# <a name="uploaditems"></a><span data-ttu-id="9a144-103">UploadItems</span><span class="sxs-lookup"><span data-stu-id="9a144-103">UploadItems</span></span>

<span data-ttu-id="9a144-104">L’élément **UploadItems** représente une demande de télécharger des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9a144-104">The **UploadItems** element represents a request to upload items into a mailbox.</span></span> 
  
[<span data-ttu-id="9a144-105">UploadItems</span><span class="sxs-lookup"><span data-stu-id="9a144-105">UploadItems</span></span>](uploaditems.md)
  
```XML
<UploadItems>
   <Items/>
</UploadItems>
```

 <span data-ttu-id="9a144-106">**UploadItemsType**</span><span class="sxs-lookup"><span data-stu-id="9a144-106">**UploadItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a144-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9a144-107">Attributes and elements</span></span>

<span data-ttu-id="9a144-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9a144-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a144-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="9a144-109">Attributes</span></span>

<span data-ttu-id="9a144-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9a144-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a144-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9a144-111">Child elements</span></span>

|<span data-ttu-id="9a144-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a144-112">**Element**</span></span>|<span data-ttu-id="9a144-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a144-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a144-114">Éléments (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="9a144-114">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md) <br/> |<span data-ttu-id="9a144-115">Contient un tableau d’éléments à charger dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="9a144-115">Contains an array of items to upload into a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a144-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9a144-116">Parent elements</span></span>

<span data-ttu-id="9a144-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9a144-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9a144-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="9a144-118">Text value</span></span>

<span data-ttu-id="9a144-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9a144-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a144-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="9a144-120">Remarks</span></span>

<span data-ttu-id="9a144-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9a144-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a144-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9a144-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a144-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9a144-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9a144-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9a144-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9a144-125">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="9a144-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="9a144-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9a144-126">Validation File</span></span>  <br/> |<span data-ttu-id="9a144-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9a144-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9a144-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9a144-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a144-129">False</span><span class="sxs-lookup"><span data-stu-id="9a144-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a144-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9a144-130">See also</span></span>



[<span data-ttu-id="9a144-131">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="9a144-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="9a144-132">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="9a144-132">UploadItems operation</span></span>](uploaditems-operation.md)

