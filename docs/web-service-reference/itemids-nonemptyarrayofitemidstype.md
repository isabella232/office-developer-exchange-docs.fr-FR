---
title: ItemId (NonEmptyArrayOfItemIdsType)
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
description: L’élément ItemId contient un tableau d’identificateurs d’élément qui identifient les éléments à exporter à partir d’une boîte aux lettres.
ms.openlocfilehash: c6d48832c5435080c7cec8e43093ea60825b604a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828151"
---
# <a name="itemids-nonemptyarrayofitemidstype"></a><span data-ttu-id="54789-103">ItemId (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="54789-103">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>

<span data-ttu-id="54789-104">L’élément **ItemId** contient un tableau d’identificateurs d’élément qui identifient les éléments à exporter à partir d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="54789-104">The **ItemIds** element contains an array of item identifiers that identify the items to export from a mailbox.</span></span> 
  
[<span data-ttu-id="54789-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="54789-105">ExportItems</span></span>](exportitems.md)
  
[<span data-ttu-id="54789-106">ItemId (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="54789-106">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
  
```XML
<ItemIds>
   <ItemId/>
</ItemIds>
```

 <span data-ttu-id="54789-107">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="54789-107">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54789-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="54789-108">Attributes and elements</span></span>

<span data-ttu-id="54789-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="54789-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54789-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="54789-110">Attributes</span></span>

<span data-ttu-id="54789-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="54789-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54789-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="54789-112">Child elements</span></span>

|<span data-ttu-id="54789-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="54789-113">**Element**</span></span>|<span data-ttu-id="54789-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="54789-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54789-115">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="54789-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="54789-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="54789-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54789-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="54789-117">Parent elements</span></span>

|<span data-ttu-id="54789-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="54789-118">**Element**</span></span>|<span data-ttu-id="54789-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="54789-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54789-120">ExportItems</span><span class="sxs-lookup"><span data-stu-id="54789-120">ExportItems</span></span>](exportitems.md) <br/> |<span data-ttu-id="54789-121">Représente une demande pour exporter les éléments à partir d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="54789-121">Represents a request to export items from a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="54789-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="54789-122">Text value</span></span>

<span data-ttu-id="54789-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="54789-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="54789-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="54789-124">Remarks</span></span>

<span data-ttu-id="54789-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="54789-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54789-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="54789-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54789-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="54789-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54789-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="54789-128">Schema Name</span></span>  <br/> |<span data-ttu-id="54789-129">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="54789-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="54789-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="54789-130">Validation File</span></span>  <br/> |<span data-ttu-id="54789-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="54789-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54789-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="54789-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="54789-133">False</span><span class="sxs-lookup"><span data-stu-id="54789-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54789-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="54789-134">See also</span></span>



[<span data-ttu-id="54789-135">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="54789-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="54789-136">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="54789-136">UploadItems operation</span></span>](uploaditems-operation.md)

