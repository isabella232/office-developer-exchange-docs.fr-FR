---
title: ParentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb7aaa46-3a04-4197-aebb-8881ff10603f
description: L’élément ParentId spécifie l’identificateur de l’élément parent dans un aperçu de la recherche.
ms.openlocfilehash: e09b5f9e463c7ecdfc595c87a84584f69cab3f2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529020"
---
# <a name="parentid"></a><span data-ttu-id="98003-103">ParentId</span><span class="sxs-lookup"><span data-stu-id="98003-103">ParentId</span></span>

<span data-ttu-id="98003-104">L’élément **ParentId** spécifie l’identificateur de l’élément parent dans un aperçu de la recherche.</span><span class="sxs-lookup"><span data-stu-id="98003-104">The **ParentId** element specifies the identifier of the parent item in a search preview.</span></span> 
  
```XML
<ParentId Id="" ChangeKey=""/>
```

<span data-ttu-id="98003-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="98003-105">**ItemIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="98003-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="98003-106">Attributes and elements</span></span>

<span data-ttu-id="98003-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="98003-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98003-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="98003-108">Attributes</span></span>

|<span data-ttu-id="98003-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="98003-109">**Attribute**</span></span>|<span data-ttu-id="98003-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="98003-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="98003-111">ID</span><span class="sxs-lookup"><span data-stu-id="98003-111">Id</span></span>  <br/> |<span data-ttu-id="98003-112">La valeur de texte de l’attribut **ID** est l’identificateur de l’élément parent.</span><span class="sxs-lookup"><span data-stu-id="98003-112">The text value of the **Id** attribute is the identifier of the parent item.</span></span>  <br/> |
|<span data-ttu-id="98003-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="98003-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="98003-114">La valeur de texte de l’attribut **ChangeKey** est la clé de modification de l’élément parent.</span><span class="sxs-lookup"><span data-stu-id="98003-114">The text value of the **ChangeKey** attribute is the change key of the parent item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="98003-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="98003-115">Child elements</span></span>

<span data-ttu-id="98003-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="98003-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98003-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="98003-117">Parent elements</span></span>

[<span data-ttu-id="98003-118">SearchPreviewItem</span><span class="sxs-lookup"><span data-stu-id="98003-118">SearchPreviewItem</span></span>](searchpreviewitem.md)
  
## <a name="remarks"></a><span data-ttu-id="98003-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="98003-119">Remarks</span></span>

<span data-ttu-id="98003-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="98003-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="98003-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="98003-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98003-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="98003-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98003-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="98003-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="98003-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="98003-124">Schema name</span></span>  <br/> |<span data-ttu-id="98003-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="98003-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="98003-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="98003-126">Validation file</span></span>  <br/> |<span data-ttu-id="98003-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="98003-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="98003-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="98003-128">Can be empty</span></span>  <br/> |<span data-ttu-id="98003-129">true</span><span class="sxs-lookup"><span data-stu-id="98003-129">true</span></span>  <br/> |
   

