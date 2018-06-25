---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: L’élément NetworkRequirements contient les critères utilisés pour déterminer si l’ordinateur client est sur un réseau qui répond aux exigences du fournisseur de services Internet (fournisseur de services Internet) pour se connecter au serveur.
ms.openlocfilehash: f3abcff04cd4121b8dcc7ceff7658ad389e6d0b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828529"
---
# <a name="networkrequirements-pox"></a><span data-ttu-id="709d9-103">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="709d9-103">NetworkRequirements (POX)</span></span>

<span data-ttu-id="709d9-104">L’élément **NetworkRequirements** contient les critères utilisés pour déterminer si l’ordinateur client est sur un réseau qui répond aux exigences du fournisseur de services Internet (fournisseur de services Internet) pour se connecter au serveur.</span><span class="sxs-lookup"><span data-stu-id="709d9-104">The **NetworkRequirements** element contains the criteria that are used to determine whether the client computer is on a network that meets the requirements of the Internet service provider (ISP) to connect to the server.</span></span> 
  
[<span data-ttu-id="709d9-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="709d9-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="709d9-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="709d9-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="709d9-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="709d9-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="709d9-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="709d9-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="709d9-109">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="709d9-109">NetworkRequirements (POX)</span></span>](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="709d9-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="709d9-110">Attributes and elements</span></span>

<span data-ttu-id="709d9-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="709d9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="709d9-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="709d9-112">Attributes</span></span>

<span data-ttu-id="709d9-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="709d9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="709d9-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="709d9-114">Child elements</span></span>

|<span data-ttu-id="709d9-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="709d9-115">**Element**</span></span>|<span data-ttu-id="709d9-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="709d9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="709d9-117">IPv4Start (POX)</span><span class="sxs-lookup"><span data-stu-id="709d9-117">IPv4Start (POX)</span></span>](ipv4start-pox.md) <br/> |<span data-ttu-id="709d9-118">Identifie le début d’une version de IP 4 (IPv4) adresses qui sont utilisés pour identifier un ordinateur sur un réseau.</span><span class="sxs-lookup"><span data-stu-id="709d9-118">Identifies the start of a range of IP version 4 (IPv4) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="709d9-119">IPv4End (POX)</span><span class="sxs-lookup"><span data-stu-id="709d9-119">IPv4End (POX)</span></span>](ipv4end-pox.md) <br/> |<span data-ttu-id="709d9-120">Identifie la fin d’une version de IP 4 (IPv4) adresses qui sont utilisés pour identifier un ordinateur sur le réseau.</span><span class="sxs-lookup"><span data-stu-id="709d9-120">Identifies the end of a range of IP version 4 (IPv4) addresses that are used to identify a computer on the network.</span></span>  <br/> |
|[<span data-ttu-id="709d9-121">IPv6Start (POX)</span><span class="sxs-lookup"><span data-stu-id="709d9-121">IPv6Start (POX)</span></span>](ipv6start-pox.md) <br/> |<span data-ttu-id="709d9-122">Identifie le début d’une version 6 (IPv6) de la plage IP adresses qui sont utilisés pour identifier un ordinateur sur un réseau.</span><span class="sxs-lookup"><span data-stu-id="709d9-122">Identifies the start of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="709d9-123">IPv6End (POX)</span><span class="sxs-lookup"><span data-stu-id="709d9-123">IPv6End (POX)</span></span>](ipv6end-pox.md) <br/> |<span data-ttu-id="709d9-124">Identifie la fin d’une version 6 (IPv6) de la plage IP adresses qui sont utilisés pour identifier un ordinateur sur un réseau.</span><span class="sxs-lookup"><span data-stu-id="709d9-124">Identifies the end of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="709d9-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="709d9-125">Parent elements</span></span>

|<span data-ttu-id="709d9-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="709d9-126">**Element**</span></span>|<span data-ttu-id="709d9-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="709d9-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="709d9-128">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="709d9-128">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="709d9-129">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="709d9-129">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="709d9-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="709d9-130">Remarks</span></span>

<span data-ttu-id="709d9-131">Si le client de messagerie ne correspond pas à la configuration réseau requise, il doit essayer d’autres types de protocoles.</span><span class="sxs-lookup"><span data-stu-id="709d9-131">If the e-mail client does not match the network requirements, it should try other protocol types.</span></span> <span data-ttu-id="709d9-132">Fournisseurs de services Internet peuvent fournir un ensemble de serveurs avec des balises de [Protocole (POX)](protocol-pox.md) qui ne nécessitent pas d’authentification, mais sont nécessaires sur le réseau du fournisseur de services Internet.</span><span class="sxs-lookup"><span data-stu-id="709d9-132">ISPs may provide one set of servers with [Protocol (POX)](protocol-pox.md) tags that do not require authentication but are required to be on the ISP network.</span></span> <span data-ttu-id="709d9-133">Fournisseurs de services Internet peuvent indiquer un autre ensemble de serveurs qui nécessitent une authentification, mais ne doivent pas se trouver sur un réseau spécifique.</span><span class="sxs-lookup"><span data-stu-id="709d9-133">ISPs may list another set of servers that require authentication but are not required to be on a specific network.</span></span> 
  
<span data-ttu-id="709d9-134">L’élément **NetworkRequirements** est facultative.</span><span class="sxs-lookup"><span data-stu-id="709d9-134">The **NetworkRequirements** element is optional.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="709d9-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="709d9-135">See also</span></span>



[<span data-ttu-id="709d9-136">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="709d9-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

