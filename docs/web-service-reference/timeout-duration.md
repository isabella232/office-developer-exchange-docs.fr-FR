---
title: Délai d’expiration (durée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: L’élément Timeout spécifie l’intervalle de temps avant un abonnement est dépassé par le serveur.
ms.openlocfilehash: 23b210dcdd87f2388aecec246068f12ec6c69a78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838698"
---
# <a name="timeout-duration"></a><span data-ttu-id="31c4b-103">Délai d’expiration (durée)</span><span class="sxs-lookup"><span data-stu-id="31c4b-103">Timeout (duration)</span></span>

<span data-ttu-id="31c4b-104">L’élément **Timeout** Spécifie l’intervalle de temps avant un abonnement est dépassé par le serveur.</span><span class="sxs-lookup"><span data-stu-id="31c4b-104">The **Timeout** element specifies the length of time before a pull subscription is timed out by the server.</span></span> 
  
```XML
<Timeout></Timeout>
```

 <span data-ttu-id="31c4b-105">**SubscriptionTimeoutType**</span><span class="sxs-lookup"><span data-stu-id="31c4b-105">**SubscriptionTimeoutType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31c4b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="31c4b-106">Attributes and elements</span></span>

<span data-ttu-id="31c4b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="31c4b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31c4b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="31c4b-108">Attributes</span></span>

<span data-ttu-id="31c4b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="31c4b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31c4b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="31c4b-110">Child elements</span></span>

<span data-ttu-id="31c4b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="31c4b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="31c4b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="31c4b-112">Parent elements</span></span>

[<span data-ttu-id="31c4b-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="31c4b-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
## <a name="text-value"></a><span data-ttu-id="31c4b-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="31c4b-114">Text value</span></span>

<span data-ttu-id="31c4b-115">La valeur de texte de l’élément de **délai d’attente** est la durée, en minutes, avant qu’un abonnement est dépassé par le serveur.</span><span class="sxs-lookup"><span data-stu-id="31c4b-115">The text value of the **Timeout** element is the length of time, in minutes, before a pull subscription is timed out by the server.</span></span> <span data-ttu-id="31c4b-116">La valeur minimale est 1 ; la valeur maximale est de 1440.</span><span class="sxs-lookup"><span data-stu-id="31c4b-116">The minimum value is 1; the maximum value is 1440.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="31c4b-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="31c4b-117">Remarks</span></span>

<span data-ttu-id="31c4b-118">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="31c4b-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="31c4b-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="31c4b-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31c4b-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="31c4b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31c4b-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="31c4b-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31c4b-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="31c4b-122">Schema name</span></span>  <br/> |<span data-ttu-id="31c4b-123">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="31c4b-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="31c4b-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="31c4b-124">Validation file</span></span>  <br/> |<span data-ttu-id="31c4b-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="31c4b-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="31c4b-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="31c4b-126">Can be empty</span></span>  <br/> ||
   

