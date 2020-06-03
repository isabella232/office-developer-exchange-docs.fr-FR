---
title: MoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItem
api_type:
- schema
ms.assetid: a4593377-22dd-415f-b01d-387389ef650f
description: L’élément MoveItem définit une demande de déplacement d’un élément dans la Banque d’Exchange.
ms.openlocfilehash: 61dbb91cc20a71f50999241b3daa21bf8ebfbcc8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530400"
---
# <a name="moveitem"></a><span data-ttu-id="3605a-103">MoveItem</span><span class="sxs-lookup"><span data-stu-id="3605a-103">MoveItem</span></span>

<span data-ttu-id="3605a-104">L’élément **MoveItem** définit une demande de déplacement d’un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="3605a-104">The **MoveItem** element defines a request to move an item in the Exchange store.</span></span> 
  
```XML
<MoveItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</MoveItem>
```

 <span data-ttu-id="3605a-105">**MoveItemType**</span><span class="sxs-lookup"><span data-stu-id="3605a-105">**MoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3605a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3605a-106">Attributes and elements</span></span>

<span data-ttu-id="3605a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3605a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3605a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3605a-108">Attributes</span></span>

<span data-ttu-id="3605a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3605a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3605a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3605a-110">Child elements</span></span>

|<span data-ttu-id="3605a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3605a-111">**Element**</span></span>|<span data-ttu-id="3605a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3605a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3605a-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="3605a-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="3605a-114">Représente le dossier de destination d’un élément déplacé.</span><span class="sxs-lookup"><span data-stu-id="3605a-114">Represents the destination folder for a moved item.</span></span>  <br/> |
|[<span data-ttu-id="3605a-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="3605a-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="3605a-116">Contient un tableau d’éléments identifiés à déplacer vers le dossier représenté par l’élément [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="3605a-116">Contains an array of identified items to move to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="3605a-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="3605a-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="3605a-118">Indique si les identificateurs d’élément de nouveaux éléments sont renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="3605a-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3605a-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3605a-119">Parent elements</span></span>

<span data-ttu-id="3605a-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3605a-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3605a-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3605a-121">Text value</span></span>

<span data-ttu-id="3605a-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3605a-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3605a-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="3605a-123">Remarks</span></span>

<span data-ttu-id="3605a-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3605a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3605a-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3605a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3605a-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3605a-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3605a-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3605a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3605a-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3605a-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3605a-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3605a-129">Validation File</span></span>  <br/> |<span data-ttu-id="3605a-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3605a-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3605a-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3605a-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="3605a-132">False</span><span class="sxs-lookup"><span data-stu-id="3605a-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3605a-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3605a-133">See also</span></span>



[<span data-ttu-id="3605a-134">Opération MoveItem</span><span class="sxs-lookup"><span data-stu-id="3605a-134">MoveItem operation</span></span>](moveitem-operation.md)


- [<span data-ttu-id="3605a-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3605a-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

