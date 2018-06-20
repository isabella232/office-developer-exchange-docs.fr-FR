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
description: L’élément de durée de vie spécifie la durée de vie, en heures, pendant laquelle les paramètres restent valides.
ms.openlocfilehash: 5fecf3103553a82ed2aeeecfc1e4e1b9fe38583c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838781"
---
# <a name="ttl-pox"></a><span data-ttu-id="db3a5-103">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="db3a5-103">TTL (POX)</span></span>

<span data-ttu-id="db3a5-104">L’élément de **durée de vie** spécifie la durée de vie, en heures, pendant laquelle les paramètres restent valides.</span><span class="sxs-lookup"><span data-stu-id="db3a5-104">The **TTL** element specifies the Time to Live, in hours, during which the settings remain valid.</span></span> 
  
[<span data-ttu-id="db3a5-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="db3a5-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="db3a5-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="db3a5-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="db3a5-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="db3a5-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="db3a5-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="db3a5-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="db3a5-109">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="db3a5-109">TTL (POX)</span></span>](ttl-pox.md)
  
```xml
<TTL/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="db3a5-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="db3a5-110">Attributes and elements</span></span>

<span data-ttu-id="db3a5-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="db3a5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db3a5-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="db3a5-112">Attributes</span></span>

<span data-ttu-id="db3a5-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="db3a5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db3a5-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="db3a5-114">Child elements</span></span>

<span data-ttu-id="db3a5-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="db3a5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="db3a5-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="db3a5-116">Parent elements</span></span>

|<span data-ttu-id="db3a5-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="db3a5-117">**Element**</span></span>|<span data-ttu-id="db3a5-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="db3a5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db3a5-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="db3a5-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="db3a5-120">Contient les spécifications pour connecter un client à l’ordinateur Exchange Server 2007 sur lequel est installé le rôle de serveur d’accès au Client.</span><span class="sxs-lookup"><span data-stu-id="db3a5-120">Contains the specifications for connecting a client to the Exchange Server 2007 computer on which the Client Access server role is installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="db3a5-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="db3a5-121">Text value</span></span>

<span data-ttu-id="db3a5-122">La valeur de texte représente la durée de vie, en heures, pendant laquelle les paramètres restent valides.</span><span class="sxs-lookup"><span data-stu-id="db3a5-122">The text value represents the Time to Live, in hours, during which the settings remain valid.</span></span> <span data-ttu-id="db3a5-123">La valeur zéro indique que redécouverte n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="db3a5-123">A value of zero indicates that rediscovery is not required.</span></span> <span data-ttu-id="db3a5-124">Si aucune valeur n’est pas spécifié, la valeur par défaut de cet élément est 1 heure.</span><span class="sxs-lookup"><span data-stu-id="db3a5-124">If no value is specified, the default value for this element is 1 hour.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="db3a5-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="db3a5-125">Remarks</span></span>

<span data-ttu-id="db3a5-126">Une fois le temps qui est représenté par l’élément de **durée de vie** écoulée, doivent identifier les paramètres à l’aide d’une requête de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="db3a5-126">After the time that is represented by the **TTL** element has elapsed, the settings should be rediscovered by using an Autodiscover request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="db3a5-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="db3a5-127">See also</span></span>



[<span data-ttu-id="db3a5-128">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="db3a5-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

