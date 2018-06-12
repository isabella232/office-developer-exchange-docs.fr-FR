---
title: CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: ffb4c13e-e7ea-4e6b-87a0-509ce5371100
description: L’élément CopyItem définit une demande pour copier un élément dans une boîte aux lettres dans la banque d’informations Exchange.
ms.openlocfilehash: 08cc1b67f7c7d369263acfc4b3d13e8aa70d2d5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755668"
---
# <a name="copyitem"></a><span data-ttu-id="1497e-103">CopyItem</span><span class="sxs-lookup"><span data-stu-id="1497e-103">CopyItem</span></span>

<span data-ttu-id="1497e-104">L’élément **CopyItem** définit une demande pour copier un élément dans une boîte aux lettres dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1497e-104">The **CopyItem** element defines a request to copy an item in a mailbox in the Exchange store.</span></span> 
  
```XML
<CopyItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</CopyItem>
```

 <span data-ttu-id="1497e-105">**CopyItemType**</span><span class="sxs-lookup"><span data-stu-id="1497e-105">**CopyItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1497e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1497e-106">Attributes and elements</span></span>

<span data-ttu-id="1497e-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1497e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1497e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1497e-108">Attributes</span></span>

<span data-ttu-id="1497e-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1497e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1497e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1497e-110">Child elements</span></span>

|<span data-ttu-id="1497e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1497e-111">**Element**</span></span>|<span data-ttu-id="1497e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1497e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1497e-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="1497e-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="1497e-114">Représente le dossier de destination pour un élément copié.</span><span class="sxs-lookup"><span data-stu-id="1497e-114">Represents the destination folder for a copied item.</span></span>  <br/> |
|[<span data-ttu-id="1497e-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="1497e-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="1497e-116">Contient un tableau d’éléments identifiés à copier dans le dossier représenté par l’élément [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="1497e-116">Contains an array of identified items to copy to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="1497e-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="1497e-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="1497e-118">Indique si les identificateurs d’élément de nouveaux éléments sont renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="1497e-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1497e-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1497e-119">Parent elements</span></span>

<span data-ttu-id="1497e-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1497e-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1497e-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="1497e-121">Remarks</span></span>

<span data-ttu-id="1497e-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1497e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1497e-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1497e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1497e-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1497e-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1497e-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1497e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1497e-126">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1497e-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1497e-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1497e-127">Validation File</span></span>  <br/> |<span data-ttu-id="1497e-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1497e-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1497e-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1497e-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="1497e-130">False</span><span class="sxs-lookup"><span data-stu-id="1497e-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1497e-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1497e-131">See also</span></span>



[<span data-ttu-id="1497e-132">Opération CopyItem</span><span class="sxs-lookup"><span data-stu-id="1497e-132">CopyItem operation</span></span>](copyitem-operation.md)


- [<span data-ttu-id="1497e-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1497e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

