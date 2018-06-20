---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: L’élément MovedItemId Spécifie l’identificateur de l’élément a été déplacé par l’opération MarkAsJunk.
ms.openlocfilehash: 17e20e8ca81f97b419fc4a2b413e21322e828ec9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828484"
---
# <a name="moveditemid"></a><span data-ttu-id="6537b-103">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="6537b-103">MovedItemId</span></span>

<span data-ttu-id="6537b-104">L’élément **MovedItemId** Spécifie l’identificateur de l’élément a été déplacé par l’opération **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="6537b-104">The **MovedItemId** element specifies the identifier of the item that was moved by the **MarkAsJunk** operation.</span></span> 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="6537b-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="6537b-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6537b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6537b-106">Attributes and elements</span></span>

<span data-ttu-id="6537b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6537b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6537b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6537b-108">Attributes</span></span>

|<span data-ttu-id="6537b-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="6537b-109">**Attribute**</span></span>|<span data-ttu-id="6537b-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="6537b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6537b-111">ID</span><span class="sxs-lookup"><span data-stu-id="6537b-111">Id</span></span>  <br/> |<span data-ttu-id="6537b-112">La valeur de l’attribut **Id** est l’identificateur d’élément de l’élément est déplacé par l’opération **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="6537b-112">The value of the **Id** attribute is the item identifier of the item that is moved by the **MarkAsJunk** operation.</span></span> <span data-ttu-id="6537b-113">L’identificateur d’élément restent les mêmes après le déplacement.</span><span class="sxs-lookup"><span data-stu-id="6537b-113">The item identifier will remain the same after the move.</span></span>  <br/> |
|<span data-ttu-id="6537b-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="6537b-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="6537b-115">La valeur de l’attribut **ChangeKey** est la clé de modification de l’élément déplacé.</span><span class="sxs-lookup"><span data-stu-id="6537b-115">The value of the **ChangeKey** attribute is the change key of the moved item.</span></span> <span data-ttu-id="6537b-116">Modifier la clé modifie une fois que l’élément est déplacé par l’opération **MarkAsJunk** .</span><span class="sxs-lookup"><span data-stu-id="6537b-116">The change key changes after the item is moved by the **MarkAsJunk** operation.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6537b-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6537b-117">Child elements</span></span>

<span data-ttu-id="6537b-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6537b-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6537b-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6537b-119">Parent elements</span></span>

[<span data-ttu-id="6537b-120">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6537b-120">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="6537b-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="6537b-121">Remarks</span></span>

<span data-ttu-id="6537b-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6537b-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6537b-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6537b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6537b-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6537b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6537b-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6537b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6537b-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6537b-126">Schema name</span></span>  <br/> |<span data-ttu-id="6537b-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6537b-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6537b-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6537b-128">Validation file</span></span>  <br/> |<span data-ttu-id="6537b-129">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6537b-129">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6537b-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6537b-130">Can be empty</span></span>  <br/> ||
   

