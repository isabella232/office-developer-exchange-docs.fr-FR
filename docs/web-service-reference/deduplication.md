---
title: Déduplication
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a38acc3d-29a8-4466-81a4-73cb30fe5e80
description: L’élément déduplication indique si le résultat de recherche doit supprimer les doublons.
ms.openlocfilehash: 3f06bb1dccd0677b7fd43c4ad82eda54a0c3f812
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755833"
---
# <a name="deduplication"></a><span data-ttu-id="4c31b-103">Déduplication</span><span class="sxs-lookup"><span data-stu-id="4c31b-103">Deduplication</span></span>

<span data-ttu-id="4c31b-104">L’élément **déduplication** indique si le résultat de recherche doit supprimer les doublons.</span><span class="sxs-lookup"><span data-stu-id="4c31b-104">The **Deduplication** element indicates whether the search result should remove duplicate items.</span></span> 
  
```XML
<Deduplication> true | false </Deduplication>
```

<span data-ttu-id="4c31b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4c31b-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4c31b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4c31b-106">Attributes and elements</span></span>

<span data-ttu-id="4c31b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4c31b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c31b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4c31b-108">Attributes</span></span>

<span data-ttu-id="4c31b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4c31b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c31b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4c31b-110">Child elements</span></span>

<span data-ttu-id="4c31b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4c31b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4c31b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4c31b-112">Parent elements</span></span>

<span data-ttu-id="4c31b-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="4c31b-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="4c31b-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4c31b-114">Text value</span></span>

<span data-ttu-id="4c31b-115">Une valeur de texte de **la valeur true** pour l’élément déduplication indique que les résultats de recherche peuvent contenir pas de doublons.</span><span class="sxs-lookup"><span data-stu-id="4c31b-115">A text value of **true** for the Deduplication element indicates that search results may not contain duplicate items.</span></span> <span data-ttu-id="4c31b-116">La valeur **false** indique que les résultats de recherche peuvent contenir des éléments en double.</span><span class="sxs-lookup"><span data-stu-id="4c31b-116">A value of **false** indicates that search results may contain duplicate items.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4c31b-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="4c31b-117">Remarks</span></span>

<span data-ttu-id="4c31b-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4c31b-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4c31b-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4c31b-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c31b-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4c31b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c31b-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4c31b-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4c31b-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4c31b-122">Schema name</span></span>  <br/> |<span data-ttu-id="4c31b-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4c31b-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="4c31b-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4c31b-124">Validation file</span></span>  <br/> |<span data-ttu-id="4c31b-125">types.xsd</span><span class="sxs-lookup"><span data-stu-id="4c31b-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4c31b-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4c31b-126">Can be empty</span></span>  <br/> |<span data-ttu-id="4c31b-127">false</span><span class="sxs-lookup"><span data-stu-id="4c31b-127">false</span></span>  <br/> |
   

