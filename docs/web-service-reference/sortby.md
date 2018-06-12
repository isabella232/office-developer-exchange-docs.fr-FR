---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: L’élément SortBy contient une propriété d’élément utilisée pour trier le résultat de recherche.
ms.openlocfilehash: 357958e393ba9331d23ee48661f21e2afe00cf01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829518"
---
# <a name="sortby"></a><span data-ttu-id="c8db4-103">SortBy</span><span class="sxs-lookup"><span data-stu-id="c8db4-103">SortBy</span></span>

<span data-ttu-id="c8db4-104">L’élément **SortBy** contient une propriété d’élément utilisée pour trier le résultat de recherche.</span><span class="sxs-lookup"><span data-stu-id="c8db4-104">The **SortBy** element contains an item property used for sorting the search result.</span></span> 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 <span data-ttu-id="c8db4-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="c8db4-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8db4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c8db4-106">Attributes and elements</span></span>

<span data-ttu-id="c8db4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c8db4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8db4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c8db4-108">Attributes</span></span>

|<span data-ttu-id="c8db4-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="c8db4-109">**Attribute**</span></span>|<span data-ttu-id="c8db4-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="c8db4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c8db4-111">Order</span><span class="sxs-lookup"><span data-stu-id="c8db4-111">Order</span></span>  <br/> |<span data-ttu-id="c8db4-112">La valeur de texte de l’attribut **ordre** est l’ordre de tri.</span><span class="sxs-lookup"><span data-stu-id="c8db4-112">The text value of the **Order** attribute is the sort order.</span></span> <span data-ttu-id="c8db4-113">Une valeur texte **croissant** indique que les résultats sont dans l’ordre croissant.</span><span class="sxs-lookup"><span data-stu-id="c8db4-113">A text value of **Ascending** indicates that the results are in ascending order.</span></span> <span data-ttu-id="c8db4-114">Une valeur texte **décroissant** indique que les résultats sont dans l’ordre décroissant.</span><span class="sxs-lookup"><span data-stu-id="c8db4-114">A text value of **Descending** indicates that the results are in descending order.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c8db4-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c8db4-115">Child elements</span></span>

<span data-ttu-id="c8db4-116">[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)</span><span class="sxs-lookup"><span data-stu-id="c8db4-116">[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8db4-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c8db4-117">Parent elements</span></span>

[<span data-ttu-id="c8db4-118">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="c8db4-118">SearchMailboxes</span></span>](searchmailboxes.md)
  
## <a name="remarks"></a><span data-ttu-id="c8db4-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="c8db4-119">Remarks</span></span>

<span data-ttu-id="c8db4-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c8db4-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c8db4-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c8db4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8db4-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c8db4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8db4-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c8db4-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c8db4-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c8db4-124">Schema name</span></span>  <br/> |<span data-ttu-id="c8db4-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c8db4-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c8db4-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c8db4-126">Validation file</span></span>  <br/> |<span data-ttu-id="c8db4-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c8db4-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c8db4-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c8db4-128">Can be empty</span></span>  <br/> ||
   

