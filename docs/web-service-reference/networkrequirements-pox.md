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
description: L’élément NetworkRequirements contient les critères utilisés pour déterminer si l’ordinateur client est sur un réseau qui répond aux exigences du fournisseur de services Internet pour se connecter au serveur.
ms.openlocfilehash: d588f7eb12a445fba9c997c4b9db0a6842105b4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462723"
---
# <a name="networkrequirements-pox"></a><span data-ttu-id="d022d-103">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="d022d-103">NetworkRequirements (POX)</span></span>

<span data-ttu-id="d022d-104">L’élément **NetworkRequirements** contient les critères utilisés pour déterminer si l’ordinateur client est sur un réseau qui répond aux exigences du fournisseur de services Internet pour se connecter au serveur.</span><span class="sxs-lookup"><span data-stu-id="d022d-104">The **NetworkRequirements** element contains the criteria that are used to determine whether the client computer is on a network that meets the requirements of the Internet service provider (ISP) to connect to the server.</span></span> 
  
[<span data-ttu-id="d022d-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="d022d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d022d-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="d022d-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d022d-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="d022d-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d022d-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="d022d-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="d022d-109">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="d022d-109">NetworkRequirements (POX)</span></span>](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d022d-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d022d-110">Attributes and elements</span></span>

<span data-ttu-id="d022d-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d022d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d022d-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="d022d-112">Attributes</span></span>

<span data-ttu-id="d022d-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d022d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d022d-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d022d-114">Child elements</span></span>

|<span data-ttu-id="d022d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d022d-115">**Element**</span></span>|<span data-ttu-id="d022d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="d022d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d022d-117">IPv4Start (POX)</span><span class="sxs-lookup"><span data-stu-id="d022d-117">IPv4Start (POX)</span></span>](ipv4start-pox.md) <br/> |<span data-ttu-id="d022d-118">Identifie le début d’une plage d’adresses IP version 4 (IPv4) utilisées pour identifier un ordinateur sur un réseau.</span><span class="sxs-lookup"><span data-stu-id="d022d-118">Identifies the start of a range of IP version 4 (IPv4) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="d022d-119">IPv4End (POX)</span><span class="sxs-lookup"><span data-stu-id="d022d-119">IPv4End (POX)</span></span>](ipv4end-pox.md) <br/> |<span data-ttu-id="d022d-120">Identifie la fin d’une plage d’adresses IP version 4 (IPv4) utilisées pour identifier un ordinateur sur le réseau.</span><span class="sxs-lookup"><span data-stu-id="d022d-120">Identifies the end of a range of IP version 4 (IPv4) addresses that are used to identify a computer on the network.</span></span>  <br/> |
|[<span data-ttu-id="d022d-121">IPv6Start (POX)</span><span class="sxs-lookup"><span data-stu-id="d022d-121">IPv6Start (POX)</span></span>](ipv6start-pox.md) <br/> |<span data-ttu-id="d022d-122">Identifie le début d’une plage d’adresses IP version 6 (IPv6) utilisées pour identifier un ordinateur sur un réseau.</span><span class="sxs-lookup"><span data-stu-id="d022d-122">Identifies the start of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="d022d-123">IPv6End (POX)</span><span class="sxs-lookup"><span data-stu-id="d022d-123">IPv6End (POX)</span></span>](ipv6end-pox.md) <br/> |<span data-ttu-id="d022d-124">Identifie la fin d’une plage d’adresses IP version 6 (IPv6) utilisées pour identifier un ordinateur sur un réseau.</span><span class="sxs-lookup"><span data-stu-id="d022d-124">Identifies the end of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d022d-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d022d-125">Parent elements</span></span>

|<span data-ttu-id="d022d-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d022d-126">**Element**</span></span>|<span data-ttu-id="d022d-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="d022d-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d022d-128">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="d022d-128">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="d022d-129">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d022d-129">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d022d-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="d022d-130">Remarks</span></span>

<span data-ttu-id="d022d-131">Si le client de messagerie ne correspond pas à la configuration réseau requise, il doit essayer d’autres types de protocole.</span><span class="sxs-lookup"><span data-stu-id="d022d-131">If the e-mail client does not match the network requirements, it should try other protocol types.</span></span> <span data-ttu-id="d022d-132">Les fournisseurs de services Internet peuvent fournir un ensemble de serveurs avec des balises de [protocole](protocol-pox.md) qui ne nécessitent pas d’authentification, mais qui doivent être sur le réseau du fournisseur de services Internet.</span><span class="sxs-lookup"><span data-stu-id="d022d-132">ISPs may provide one set of servers with [Protocol (POX)](protocol-pox.md) tags that do not require authentication but are required to be on the ISP network.</span></span> <span data-ttu-id="d022d-133">Ils peuvent répertorier un autre ensemble de serveurs qui nécessitent une authentification, mais ils ne doivent pas nécessairement se trouver sur un réseau spécifique.</span><span class="sxs-lookup"><span data-stu-id="d022d-133">ISPs may list another set of servers that require authentication but are not required to be on a specific network.</span></span> 
  
<span data-ttu-id="d022d-134">L’élément **NetworkRequirements** est facultatif.</span><span class="sxs-lookup"><span data-stu-id="d022d-134">The **NetworkRequirements** element is optional.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d022d-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d022d-135">See also</span></span>



[<span data-ttu-id="d022d-136">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d022d-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

