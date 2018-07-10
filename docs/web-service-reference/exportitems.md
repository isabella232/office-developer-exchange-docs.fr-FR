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
description: L’élément ExportItems représente une demande pour exporter les éléments à partir d’une boîte aux lettres.
ms.openlocfilehash: 055012166bb125dfcf86070f2e23496bf0209b51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756261"
---
# <a name="exportitems"></a><span data-ttu-id="14a6b-103">ExportItems</span><span class="sxs-lookup"><span data-stu-id="14a6b-103">ExportItems</span></span>

<span data-ttu-id="14a6b-104">L’élément **ExportItems** représente une demande pour exporter les éléments à partir d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="14a6b-104">The **ExportItems** element represents a request to export items from a mailbox.</span></span> 
  
[<span data-ttu-id="14a6b-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="14a6b-105">ExportItems</span></span>](exportitems.md)
  
```XML
<ExportItems>
   <ItemIds/>
</ExportItems>
```

 <span data-ttu-id="14a6b-106">**ExportItemsType**</span><span class="sxs-lookup"><span data-stu-id="14a6b-106">**ExportItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14a6b-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="14a6b-107">Attributes and elements</span></span>

<span data-ttu-id="14a6b-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="14a6b-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14a6b-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="14a6b-109">Attributes</span></span>

<span data-ttu-id="14a6b-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="14a6b-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14a6b-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="14a6b-111">Child elements</span></span>

|<span data-ttu-id="14a6b-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="14a6b-112">**Element**</span></span>|<span data-ttu-id="14a6b-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="14a6b-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14a6b-114">ItemId (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="14a6b-114">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md) <br/> |<span data-ttu-id="14a6b-115">Contient un tableau d’identificateurs d’élément qui identifient les éléments à exporter à partir d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="14a6b-115">Contains an array of item identifiers that identify the items to export from a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="14a6b-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="14a6b-116">Parent elements</span></span>

<span data-ttu-id="14a6b-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="14a6b-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="14a6b-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="14a6b-118">Text value</span></span>

<span data-ttu-id="14a6b-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="14a6b-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="14a6b-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="14a6b-120">Remarks</span></span>

<span data-ttu-id="14a6b-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="14a6b-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14a6b-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="14a6b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14a6b-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="14a6b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="14a6b-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="14a6b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="14a6b-125">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="14a6b-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="14a6b-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="14a6b-126">Validation File</span></span>  <br/> |<span data-ttu-id="14a6b-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="14a6b-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="14a6b-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="14a6b-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="14a6b-129">False</span><span class="sxs-lookup"><span data-stu-id="14a6b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14a6b-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="14a6b-130">See also</span></span>



[<span data-ttu-id="14a6b-131">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="14a6b-131">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="14a6b-132">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="14a6b-132">UploadItems operation</span></span>](uploaditems-operation.md)
