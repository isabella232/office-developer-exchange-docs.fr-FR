---
title: Déduplication
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a38acc3d-29a8-4466-81a4-73cb30fe5e80
description: L’élément Deduplication indique si le résultat de la recherche doit supprimer les éléments en double.
ms.openlocfilehash: c39f980658aba7036cfabb3b51af5a41005f97b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463712"
---
# <a name="deduplication"></a><span data-ttu-id="192aa-103">Déduplication</span><span class="sxs-lookup"><span data-stu-id="192aa-103">Deduplication</span></span>

<span data-ttu-id="192aa-104">L’élément **Deduplication** indique si le résultat de la recherche doit supprimer les éléments en double.</span><span class="sxs-lookup"><span data-stu-id="192aa-104">The **Deduplication** element indicates whether the search result should remove duplicate items.</span></span> 
  
```XML
<Deduplication> true | false </Deduplication>
```

<span data-ttu-id="192aa-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="192aa-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="192aa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="192aa-106">Attributes and elements</span></span>

<span data-ttu-id="192aa-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="192aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="192aa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="192aa-108">Attributes</span></span>

<span data-ttu-id="192aa-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="192aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="192aa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="192aa-110">Child elements</span></span>

<span data-ttu-id="192aa-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="192aa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="192aa-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="192aa-112">Parent elements</span></span>

<span data-ttu-id="192aa-113">[SearchMailboxes](searchmailboxes.md)  |  [SetHoldOnMailboxes](setholdonmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="192aa-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="192aa-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="192aa-114">Text value</span></span>

<span data-ttu-id="192aa-115">Une valeur de texte **true** pour l’élément Deduplication indique que les résultats de la recherche peuvent ne pas contenir d’éléments en double.</span><span class="sxs-lookup"><span data-stu-id="192aa-115">A text value of **true** for the Deduplication element indicates that search results may not contain duplicate items.</span></span> <span data-ttu-id="192aa-116">La valeur **false** indique que les résultats de la recherche peuvent contenir des éléments en double.</span><span class="sxs-lookup"><span data-stu-id="192aa-116">A value of **false** indicates that search results may contain duplicate items.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="192aa-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="192aa-117">Remarks</span></span>

<span data-ttu-id="192aa-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="192aa-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="192aa-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="192aa-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="192aa-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="192aa-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="192aa-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="192aa-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="192aa-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="192aa-122">Schema name</span></span>  <br/> |<span data-ttu-id="192aa-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="192aa-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="192aa-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="192aa-124">Validation file</span></span>  <br/> |<span data-ttu-id="192aa-125">types. xsd</span><span class="sxs-lookup"><span data-stu-id="192aa-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="192aa-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="192aa-126">Can be empty</span></span>  <br/> |<span data-ttu-id="192aa-127">false</span><span class="sxs-lookup"><span data-stu-id="192aa-127">false</span></span>  <br/> |
   

