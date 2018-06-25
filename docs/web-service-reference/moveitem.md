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
description: L’élément MoveItem définit une demande de déplacement d’un élément dans la banque d’informations Exchange.
ms.openlocfilehash: cd7f35bdabe8a596f4c186df1c8cd54e0ea1c540
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828486"
---
# <a name="moveitem"></a><span data-ttu-id="b17cc-103">MoveItem</span><span class="sxs-lookup"><span data-stu-id="b17cc-103">MoveItem</span></span>

<span data-ttu-id="b17cc-104">L’élément **MoveItem** définit une demande de déplacement d’un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="b17cc-104">The **MoveItem** element defines a request to move an item in the Exchange store.</span></span> 
  
```XML
<MoveItem>
   <ToFolderId/>
   <ItemIds/>
   <ReturnNewItemIds/>
</MoveItem>
```

 <span data-ttu-id="b17cc-105">**MoveItemType**</span><span class="sxs-lookup"><span data-stu-id="b17cc-105">**MoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b17cc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b17cc-106">Attributes and elements</span></span>

<span data-ttu-id="b17cc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b17cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b17cc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b17cc-108">Attributes</span></span>

<span data-ttu-id="b17cc-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b17cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b17cc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b17cc-110">Child elements</span></span>

|<span data-ttu-id="b17cc-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b17cc-111">**Element**</span></span>|<span data-ttu-id="b17cc-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="b17cc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b17cc-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="b17cc-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="b17cc-114">Représente le dossier de destination pour un élément déplacé.</span><span class="sxs-lookup"><span data-stu-id="b17cc-114">Represents the destination folder for a moved item.</span></span>  <br/> |
|[<span data-ttu-id="b17cc-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="b17cc-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="b17cc-116">Contient un tableau d’éléments identifiés à déplacer vers le dossier représenté par l’élément [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="b17cc-116">Contains an array of identified items to move to the folder represented by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="b17cc-117">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="b17cc-117">ReturnNewItemIds</span></span>](returnnewitemids.md) <br/> |<span data-ttu-id="b17cc-118">Indique si les identificateurs d’élément de nouveaux éléments sont renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="b17cc-118">Indicates whether the item identifiers of new items are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b17cc-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b17cc-119">Parent elements</span></span>

<span data-ttu-id="b17cc-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b17cc-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b17cc-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b17cc-121">Text value</span></span>

<span data-ttu-id="b17cc-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b17cc-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b17cc-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="b17cc-123">Remarks</span></span>

<span data-ttu-id="b17cc-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b17cc-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b17cc-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b17cc-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b17cc-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b17cc-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b17cc-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b17cc-127">Schema Name</span></span>  <br/> |<span data-ttu-id="b17cc-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b17cc-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b17cc-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b17cc-129">Validation File</span></span>  <br/> |<span data-ttu-id="b17cc-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b17cc-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b17cc-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b17cc-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="b17cc-132">False</span><span class="sxs-lookup"><span data-stu-id="b17cc-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b17cc-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b17cc-133">See also</span></span>



[<span data-ttu-id="b17cc-134">Opération MoveItem</span><span class="sxs-lookup"><span data-stu-id="b17cc-134">MoveItem operation</span></span>](moveitem-operation.md)


- [<span data-ttu-id="b17cc-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b17cc-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

