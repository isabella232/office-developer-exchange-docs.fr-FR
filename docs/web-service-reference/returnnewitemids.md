---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: L’élément ReturnNewItemIds indique si les identificateurs d’élément de nouveaux éléments sont renvoyés dans la réponse.
ms.openlocfilehash: 6d3bc83c05a82d6e448041167676f41c2620dcd4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829232"
---
# <a name="returnnewitemids"></a><span data-ttu-id="0375a-103">ReturnNewItemIds</span><span class="sxs-lookup"><span data-stu-id="0375a-103">ReturnNewItemIds</span></span>

<span data-ttu-id="0375a-104">L’élément **ReturnNewItemIds** indique si les identificateurs d’élément de nouveaux éléments sont renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="0375a-104">The **ReturnNewItemIds** element indicates whether the item identifiers of new items are returned in the response.</span></span> 
  
```XML
<ReturnNewItemIds/>
```

 <span data-ttu-id="0375a-105">**xs : Boolean**</span><span class="sxs-lookup"><span data-stu-id="0375a-105">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0375a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0375a-106">Attributes and elements</span></span>

<span data-ttu-id="0375a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0375a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0375a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0375a-108">Attributes</span></span>

<span data-ttu-id="0375a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0375a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0375a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0375a-110">Child elements</span></span>

<span data-ttu-id="0375a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0375a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0375a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0375a-112">Parent elements</span></span>

|<span data-ttu-id="0375a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0375a-113">**Element**</span></span>|<span data-ttu-id="0375a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0375a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0375a-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="0375a-115">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="0375a-116">Définit une demande pour copier un élément dans une boîte aux lettres dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0375a-116">Defines a request to copy an item in a mailbox in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0375a-117">MoveItem</span><span class="sxs-lookup"><span data-stu-id="0375a-117">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="0375a-118">Définit une demande de déplacement d’un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0375a-118">Defines a request to move an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0375a-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0375a-119">Text value</span></span>

<span data-ttu-id="0375a-120">Une valeur de texte de **la valeur true** pour l’élément **ReturnNewItemIds** indique que les nouveaux identificateurs d’élément sont retournés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="0375a-120">A text value of **true** for the **ReturnNewItemIds** element indicates that the new item identifiers are returned in the response.</span></span> <span data-ttu-id="0375a-121">La valeur **false** indique que les nouveaux identificateurs d’élément ne sont pas renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="0375a-121">A value of **false** indicates that the new item identifiers are not returned in the response.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0375a-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="0375a-122">Remarks</span></span>

<span data-ttu-id="0375a-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0375a-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0375a-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0375a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0375a-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0375a-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0375a-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0375a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="0375a-127">Schéma des messages</span><span class="sxs-lookup"><span data-stu-id="0375a-127">Message schema</span></span>  <br/> |
|<span data-ttu-id="0375a-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0375a-128">Validation File</span></span>  <br/> |<span data-ttu-id="0375a-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0375a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0375a-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0375a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="0375a-131">False</span><span class="sxs-lookup"><span data-stu-id="0375a-131">False</span></span>  <br/> |
   

