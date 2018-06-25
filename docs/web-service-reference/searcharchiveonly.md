---
title: SearchArchiveOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: L’élément SearchArchiveOnly indique si uniquement la boîte aux lettres de l’archive est non indexables éléments recherché.
ms.openlocfilehash: ac9d3262784d8052486c631ef3e99e650d4757c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829293"
---
# <a name="searcharchiveonly"></a><span data-ttu-id="865bb-103">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="865bb-103">SearchArchiveOnly</span></span>

<span data-ttu-id="865bb-104">L’élément **SearchArchiveOnly** indique si uniquement la boîte aux lettres de l’archive est non indexables éléments recherché.</span><span class="sxs-lookup"><span data-stu-id="865bb-104">The **SearchArchiveOnly** element indicates whether only the archive mailbox is searched for non-indexable items.</span></span> 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 <span data-ttu-id="865bb-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="865bb-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="865bb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="865bb-106">Attributes and elements</span></span>

<span data-ttu-id="865bb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="865bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="865bb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="865bb-108">Attributes</span></span>

<span data-ttu-id="865bb-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="865bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="865bb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="865bb-110">Child elements</span></span>

<span data-ttu-id="865bb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="865bb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="865bb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="865bb-112">Parent elements</span></span>

<span data-ttu-id="865bb-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span><span class="sxs-lookup"><span data-stu-id="865bb-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="865bb-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="865bb-114">Text value</span></span>

<span data-ttu-id="865bb-115">Une valeur de texte de **la valeur true** pour l’élément **SearchArchiveOnly** indique que la recherche non indexables élément porte uniquement sur la boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="865bb-115">A text value of **true** for the **SearchArchiveOnly** element indicates that non-indexable item search is only performed on the archive mailbox.</span></span> <span data-ttu-id="865bb-116">Texte la valeur **false** indique que la recherche est effectuée sur la boîte aux lettres principale et une boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="865bb-116">A text value of **false** indicates that the search is performed against the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="865bb-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="865bb-117">Remarks</span></span>

<span data-ttu-id="865bb-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="865bb-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="865bb-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="865bb-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="865bb-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="865bb-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="865bb-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="865bb-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="865bb-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="865bb-122">Schema name</span></span>  <br/> |<span data-ttu-id="865bb-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="865bb-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="865bb-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="865bb-124">Validation file</span></span>  <br/> |<span data-ttu-id="865bb-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="865bb-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="865bb-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="865bb-126">Can be empty</span></span>  <br/> ||
   

