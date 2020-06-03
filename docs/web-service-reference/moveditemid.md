---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: L’élément MovedItemId spécifie l’identificateur de l’élément qui a été déplacé par l’opération MarkAsJunk.
ms.openlocfilehash: 5cf8800ec672278691348bbcd8c6c8cc7a12905b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468613"
---
# <a name="moveditemid"></a><span data-ttu-id="34b2d-103">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="34b2d-103">MovedItemId</span></span>

<span data-ttu-id="34b2d-104">L’élément **MovedItemId** spécifie l’identificateur de l’élément qui a été déplacé par l’opération **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="34b2d-104">The **MovedItemId** element specifies the identifier of the item that was moved by the **MarkAsJunk** operation.</span></span> 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="34b2d-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="34b2d-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34b2d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="34b2d-106">Attributes and elements</span></span>

<span data-ttu-id="34b2d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="34b2d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34b2d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="34b2d-108">Attributes</span></span>

|<span data-ttu-id="34b2d-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="34b2d-109">**Attribute**</span></span>|<span data-ttu-id="34b2d-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="34b2d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="34b2d-111">ID</span><span class="sxs-lookup"><span data-stu-id="34b2d-111">Id</span></span>  <br/> |<span data-ttu-id="34b2d-112">La valeur de l’attribut **ID** est l’identificateur d’élément de l’élément qui est déplacé par l’opération **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="34b2d-112">The value of the **Id** attribute is the item identifier of the item that is moved by the **MarkAsJunk** operation.</span></span> <span data-ttu-id="34b2d-113">L’identificateur de l’élément reste le même après le déplacement.</span><span class="sxs-lookup"><span data-stu-id="34b2d-113">The item identifier will remain the same after the move.</span></span>  <br/> |
|<span data-ttu-id="34b2d-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="34b2d-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="34b2d-115">La valeur de l’attribut **ChangeKey** est la clé de modification de l’élément déplacé.</span><span class="sxs-lookup"><span data-stu-id="34b2d-115">The value of the **ChangeKey** attribute is the change key of the moved item.</span></span> <span data-ttu-id="34b2d-116">La modification de la clé change après le déplacement de l’élément par l’opération **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="34b2d-116">The change key changes after the item is moved by the **MarkAsJunk** operation.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="34b2d-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="34b2d-117">Child elements</span></span>

<span data-ttu-id="34b2d-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="34b2d-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34b2d-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="34b2d-119">Parent elements</span></span>

[<span data-ttu-id="34b2d-120">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="34b2d-120">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="34b2d-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="34b2d-121">Remarks</span></span>

<span data-ttu-id="34b2d-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="34b2d-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="34b2d-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="34b2d-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34b2d-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="34b2d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34b2d-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="34b2d-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="34b2d-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="34b2d-126">Schema name</span></span>  <br/> |<span data-ttu-id="34b2d-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="34b2d-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="34b2d-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="34b2d-128">Validation file</span></span>  <br/> |<span data-ttu-id="34b2d-129">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="34b2d-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="34b2d-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="34b2d-130">Can be empty</span></span>  <br/> ||
   

