---
title: TTL (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 178eefa1-995c-4bea-930b-e51293961191
description: L’élément TTL spécifie la durée de vie, en heures, pendant laquelle les paramètres restent valides.
ms.openlocfilehash: 9a17cbe4e669d1afe9f3ef4a24f2a9a2889a7d52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467381"
---
# <a name="ttl-pox"></a><span data-ttu-id="84f15-103">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="84f15-103">TTL (POX)</span></span>

<span data-ttu-id="84f15-104">L’élément **TTL** spécifie la durée de vie, en heures, pendant laquelle les paramètres restent valides.</span><span class="sxs-lookup"><span data-stu-id="84f15-104">The **TTL** element specifies the Time to Live, in hours, during which the settings remain valid.</span></span> 
  
[<span data-ttu-id="84f15-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="84f15-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="84f15-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="84f15-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="84f15-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="84f15-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="84f15-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="84f15-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="84f15-109">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="84f15-109">TTL (POX)</span></span>](ttl-pox.md)
  
```xml
<TTL/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="84f15-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="84f15-110">Attributes and elements</span></span>

<span data-ttu-id="84f15-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="84f15-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84f15-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="84f15-112">Attributes</span></span>

<span data-ttu-id="84f15-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="84f15-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84f15-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="84f15-114">Child elements</span></span>

<span data-ttu-id="84f15-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="84f15-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="84f15-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="84f15-116">Parent elements</span></span>

|<span data-ttu-id="84f15-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="84f15-117">**Element**</span></span>|<span data-ttu-id="84f15-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="84f15-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84f15-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="84f15-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="84f15-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="84f15-120">Contains the specifications for connecting a client to the Exchange Server 2007 computer on which the Client Access server role is installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="84f15-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="84f15-121">Text value</span></span>

<span data-ttu-id="84f15-122">La valeur de texte représente la durée de vie, en heures, pendant laquelle les paramètres restent valides.</span><span class="sxs-lookup"><span data-stu-id="84f15-122">The text value represents the Time to Live, in hours, during which the settings remain valid.</span></span> <span data-ttu-id="84f15-123">La valeur zéro indique que la redécouverte n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="84f15-123">A value of zero indicates that rediscovery is not required.</span></span> <span data-ttu-id="84f15-124">Si aucune valeur n’est spécifiée, la valeur par défaut de cet élément est 1 heure.</span><span class="sxs-lookup"><span data-stu-id="84f15-124">If no value is specified, the default value for this element is 1 hour.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="84f15-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="84f15-125">Remarks</span></span>

<span data-ttu-id="84f15-126">Une fois que le temps représenté par l’élément **TTL** s’est écoulé, les paramètres doivent être redécouverts à l’aide d’une demande de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="84f15-126">After the time that is represented by the **TTL** element has elapsed, the settings should be rediscovered by using an Autodiscover request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="84f15-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="84f15-127">See also</span></span>



[<span data-ttu-id="84f15-128">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="84f15-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

