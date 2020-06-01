---
title: Délai d’expiration (durée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: L’élément Timeout spécifie la durée avant l’expiration d’un abonnement extrait par le serveur.
ms.openlocfilehash: b5b0e77d794080cd8e0da1e14acf4cb059b80b08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460280"
---
# <a name="timeout-duration"></a><span data-ttu-id="2d4b3-103">Délai d’expiration (durée)</span><span class="sxs-lookup"><span data-stu-id="2d4b3-103">Timeout (duration)</span></span>

<span data-ttu-id="2d4b3-104">L’élément **timeout** spécifie la durée avant l’expiration d’un abonnement extrait par le serveur.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-104">The **Timeout** element specifies the length of time before a pull subscription is timed out by the server.</span></span> 
  
```XML
<Timeout></Timeout>
```

 <span data-ttu-id="2d4b3-105">**SubscriptionTimeoutType**</span><span class="sxs-lookup"><span data-stu-id="2d4b3-105">**SubscriptionTimeoutType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d4b3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2d4b3-106">Attributes and elements</span></span>

<span data-ttu-id="2d4b3-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d4b3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2d4b3-108">Attributes</span></span>

<span data-ttu-id="2d4b3-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d4b3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2d4b3-110">Child elements</span></span>

<span data-ttu-id="2d4b3-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2d4b3-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2d4b3-112">Parent elements</span></span>

[<span data-ttu-id="2d4b3-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="2d4b3-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
## <a name="text-value"></a><span data-ttu-id="2d4b3-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="2d4b3-114">Text value</span></span>

<span data-ttu-id="2d4b3-115">La valeur de texte de l’élément **timeout** est la durée, en minutes, avant qu’un abonnement extrait ne soit expiré par le serveur.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-115">The text value of the **Timeout** element is the length of time, in minutes, before a pull subscription is timed out by the server.</span></span> <span data-ttu-id="2d4b3-116">La valeur minimale est 1 ; la valeur maximale est 1440.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-116">The minimum value is 1; the maximum value is 1440.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2d4b3-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="2d4b3-117">Remarks</span></span>

<span data-ttu-id="2d4b3-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2d4b3-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d4b3-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d4b3-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2d4b3-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d4b3-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2d4b3-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d4b3-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2d4b3-122">Schema name</span></span>  <br/> |<span data-ttu-id="2d4b3-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2d4b3-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="2d4b3-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2d4b3-124">Validation file</span></span>  <br/> |<span data-ttu-id="2d4b3-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2d4b3-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d4b3-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2d4b3-126">Can be empty</span></span>  <br/> ||
   

