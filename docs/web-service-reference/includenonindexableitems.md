---
title: IncludeNonIndexableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af7f202b-2889-447e-bdeb-aaad18ce6b46
description: L’élément IncludeNonIndexableItems contient une valeur booléenne pour indiquer s’il faut inclure des éléments qui ne peuvent pas être indexés.
ms.openlocfilehash: ae91a3c6db82aea1d45940603d0ff2064d29f43f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827904"
---
# <a name="includenonindexableitems"></a><span data-ttu-id="6a824-103">IncludeNonIndexableItems</span><span class="sxs-lookup"><span data-stu-id="6a824-103">IncludeNonIndexableItems</span></span>

<span data-ttu-id="6a824-104">L’élément **IncludeNonIndexableItems** contient une valeur **booléenne** pour indiquer s’il faut inclure des éléments qui ne peuvent pas être indexés.</span><span class="sxs-lookup"><span data-stu-id="6a824-104">The **IncludeNonIndexableItems** element contains a **Boolean** value to indicate whether to include items that cannot be indexed.</span></span> 
  
```XML
<IncludeNonIndexableItems>true | false</IncludeNonIndexableItems>
```

 <span data-ttu-id="6a824-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6a824-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a824-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6a824-106">Attributes and elements</span></span>

<span data-ttu-id="6a824-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6a824-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a824-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6a824-108">Attributes</span></span>

<span data-ttu-id="6a824-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6a824-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a824-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6a824-110">Child elements</span></span>

<span data-ttu-id="6a824-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6a824-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6a824-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6a824-112">Parent elements</span></span>

[<span data-ttu-id="6a824-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="6a824-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="6a824-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6a824-114">Text value</span></span>

<span data-ttu-id="6a824-115">Une valeur de texte de **la valeur true** pour l’élément **IncludeNonIndexableItems** indique que les éléments qui ne peuvent pas être indexés sont inclus dans la boîte aux lettres suspensions.</span><span class="sxs-lookup"><span data-stu-id="6a824-115">A text value of **true** for the **IncludeNonIndexableItems** element indicates that items that cannot be indexed are included with mailbox holds.</span></span> <span data-ttu-id="6a824-116">La valeur **false** indique que les éléments qui ne peuvent pas être indexés ne figurent pas dans la boîte aux lettres suspensions.</span><span class="sxs-lookup"><span data-stu-id="6a824-116">A value of **false** indicates that the items that cannot be indexed are not included in mailbox holds.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6a824-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="6a824-117">Remarks</span></span>

<span data-ttu-id="6a824-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6a824-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6a824-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6a824-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a824-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6a824-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a824-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6a824-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6a824-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6a824-122">Schema name</span></span>  <br/> |<span data-ttu-id="6a824-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6a824-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6a824-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6a824-124">Validation file</span></span>  <br/> |<span data-ttu-id="6a824-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6a824-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6a824-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6a824-126">Can be empty</span></span>  <br/> |<span data-ttu-id="6a824-127">false</span><span class="sxs-lookup"><span data-stu-id="6a824-127">false</span></span>  <br/> |
   

