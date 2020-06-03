---
title: SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d8c367a-67e9-43b3-8be0-6362d2152431
description: L’élément SearchMailboxes indique le début de la demande SearchMailboxes.
ms.openlocfilehash: 7ccc94157ef6bde7b6ba86e70c16ef6e90d712fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456800"
---
# <a name="searchmailboxes"></a><span data-ttu-id="09d2e-103">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="09d2e-103">SearchMailboxes</span></span>

<span data-ttu-id="09d2e-104">L’élément **SearchMailboxes** indique le début de la demande **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="09d2e-104">The **SearchMailboxes** element indicates the beginning of the **SearchMailboxes** request.</span></span> 
  
```XML
<SearchMailboxes>
   <SearchQueries/>
   <ResultType/>
   <PreviewItemResponseShape/>
   <SortBy/>
   <Language/>
   <Deduplication/>
   <PageSize/>
   <PageItemReference/>
   <PageDirection/>
</SearchMailboxes>
```

 <span data-ttu-id="09d2e-105">**SearchMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="09d2e-105">**SearchMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09d2e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="09d2e-106">Attributes and elements</span></span>

<span data-ttu-id="09d2e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="09d2e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09d2e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="09d2e-108">Attributes</span></span>

<span data-ttu-id="09d2e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="09d2e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09d2e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="09d2e-110">Child elements</span></span>

<span data-ttu-id="09d2e-111">[SearchQueries](searchqueries.md)  |  [ResultType](resulttype.md)  |  [PreviewItemResponseShape](previewitemresponseshape.md)  |  [SortBy](sortby.md)  |  [Langue](language.md)  |  [Déduplication](deduplication.md)  |  [PageSize](pagesize.md)  |  [PageItemReference](pageitemreference.md)  |  [PageDirection](pagedirection.md)</span><span class="sxs-lookup"><span data-stu-id="09d2e-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [PreviewItemResponseShape](previewitemresponseshape.md) | [SortBy](sortby.md) | [Language](language.md) | [Deduplication](deduplication.md) | [PageSize](pagesize.md) | [PageItemReference](pageitemreference.md) | [PageDirection](pagedirection.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="09d2e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="09d2e-112">Parent elements</span></span>

<span data-ttu-id="09d2e-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="09d2e-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09d2e-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="09d2e-114">Remarks</span></span>

<span data-ttu-id="09d2e-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="09d2e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="09d2e-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="09d2e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09d2e-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="09d2e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09d2e-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="09d2e-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="09d2e-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="09d2e-119">Schema name</span></span>  <br/> |<span data-ttu-id="09d2e-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="09d2e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="09d2e-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="09d2e-121">Validation file</span></span>  <br/> |<span data-ttu-id="09d2e-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="09d2e-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="09d2e-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="09d2e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="09d2e-124">false</span><span class="sxs-lookup"><span data-stu-id="09d2e-124">false</span></span>  <br/> |
   

