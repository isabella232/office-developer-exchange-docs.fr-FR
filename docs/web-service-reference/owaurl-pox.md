---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: L’élément OWAUrl décrit l’URL et le schéma d’authentification utilisés pour accéder à un ordinateur spécifique exécutant Microsoft Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé et qui héberge Outlook Web Access.
ms.openlocfilehash: c0728af063cfbf1353eb7d3b81f5fcfe8b398f7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457262"
---
# <a name="owaurl-pox"></a><span data-ttu-id="7d54d-103">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="7d54d-103">OWAUrl (POX)</span></span>

<span data-ttu-id="7d54d-104">L’élément **OWAUrl** décrit l’URL et le schéma d’authentification utilisés pour accéder à un ordinateur spécifique exécutant Microsoft Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé et qui héberge Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="7d54d-104">The **OWAUrl** element describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that hosts Outlook Web Access.</span></span> 
  
[<span data-ttu-id="7d54d-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="7d54d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="7d54d-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="7d54d-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="7d54d-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="7d54d-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="7d54d-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="7d54d-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="7d54d-109">Interne (POX)</span><span class="sxs-lookup"><span data-stu-id="7d54d-109">Internal (POX)</span></span>](internal-pox.md)
  
[<span data-ttu-id="7d54d-110">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="7d54d-110">OWAUrl (POX)</span></span>](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="7d54d-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7d54d-111">Attributes and elements</span></span>

<span data-ttu-id="7d54d-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7d54d-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d54d-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="7d54d-113">Attributes</span></span>

|<span data-ttu-id="7d54d-114">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7d54d-114">**Attribute**</span></span>|<span data-ttu-id="7d54d-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="7d54d-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7d54d-116">**AuthenticationMethod**</span><span class="sxs-lookup"><span data-stu-id="7d54d-116">**AuthenticationMethod**</span></span> <br/> |<span data-ttu-id="7d54d-117">Décrit les méthodes d’authentification permettant d’accéder à Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="7d54d-117">Describes the authentication methods for accessing Outlook Web Access.</span></span>  <br/> |
   
#### <a name="authenticationmethod-attribute"></a><span data-ttu-id="7d54d-118">Attribut AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="7d54d-118">AuthenticationMethod Attribute</span></span>

|<span data-ttu-id="7d54d-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="7d54d-119">**Value**</span></span>|<span data-ttu-id="7d54d-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="7d54d-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7d54d-121">WindowsIntegrated</span><span class="sxs-lookup"><span data-stu-id="7d54d-121">WindowsIntegrated</span></span>  <br/> |<span data-ttu-id="7d54d-122">Authentification Windows intégrée.</span><span class="sxs-lookup"><span data-stu-id="7d54d-122">Integrated Windows authentication.</span></span>  <br/> |
|<span data-ttu-id="7d54d-123">FBA</span><span class="sxs-lookup"><span data-stu-id="7d54d-123">FBA</span></span>  <br/> |<span data-ttu-id="7d54d-124">Authentification basée sur les formulaires.</span><span class="sxs-lookup"><span data-stu-id="7d54d-124">Forms-based authentication.</span></span>  <br/> |
|<span data-ttu-id="7d54d-125">NTLM</span><span class="sxs-lookup"><span data-stu-id="7d54d-125">NTLM</span></span>  <br/> |<span data-ttu-id="7d54d-126">Authentification NTLM.</span><span class="sxs-lookup"><span data-stu-id="7d54d-126">NTLM authentication.</span></span>  <br/> |
|<span data-ttu-id="7d54d-127">Digest</span><span class="sxs-lookup"><span data-stu-id="7d54d-127">Digest</span></span>  <br/> |<span data-ttu-id="7d54d-128">Authentification Digest.</span><span class="sxs-lookup"><span data-stu-id="7d54d-128">Digest authentication.</span></span>  <br/> |
|<span data-ttu-id="7d54d-129">De base</span><span class="sxs-lookup"><span data-stu-id="7d54d-129">Basic</span></span>  <br/> |<span data-ttu-id="7d54d-130">Authentification de base.</span><span class="sxs-lookup"><span data-stu-id="7d54d-130">Basic authentication.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7d54d-131">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7d54d-131">Child elements</span></span>

<span data-ttu-id="7d54d-132">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7d54d-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7d54d-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7d54d-133">Parent elements</span></span>

|<span data-ttu-id="7d54d-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7d54d-134">**Element**</span></span>|<span data-ttu-id="7d54d-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="7d54d-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d54d-136">Interne (POX)</span><span class="sxs-lookup"><span data-stu-id="7d54d-136">Internal (POX)</span></span>](internal-pox.md) <br/> |<span data-ttu-id="7d54d-137">Contient la collection d’URL Outlook Web Access à laquelle un client peut se connecter lorsqu’il se trouve à l’intérieur du pare-feu.</span><span class="sxs-lookup"><span data-stu-id="7d54d-137">Contains the collection of Outlook Web Access URLs that a client can connect to when it is inside the firewall.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d54d-138">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="7d54d-138">Text value</span></span>

<span data-ttu-id="7d54d-139">La valeur texte représente l’URL du service Outlook Web Access sur un serveur d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="7d54d-139">The text value represents the URL for the Outlook Web Access service on a Client Access server.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="7d54d-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7d54d-140">See also</span></span>



[<span data-ttu-id="7d54d-141">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7d54d-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

