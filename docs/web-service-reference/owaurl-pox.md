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
description: L’élément OWAUrl décrit l’URL et le schéma d’authentification qui est utilisé pour accéder à un ordinateur qui exécute Microsoft Exchange Server 2007 qui a le rôle de serveur Client Access installé qui héberge Outlook Web Access.
ms.openlocfilehash: 93d03506e2a74aa1b4ef6d2a49ccbda01cfc1f9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828673"
---
# <a name="owaurl-pox"></a><span data-ttu-id="1a1c7-103">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1a1c7-103">OWAUrl (POX)</span></span>

<span data-ttu-id="1a1c7-104">L’élément **OWAUrl** décrit l’URL et le schéma d’authentification qui est utilisé pour accéder à un ordinateur qui exécute Microsoft Exchange Server 2007 qui a le rôle de serveur Client Access installé qui héberge Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="1a1c7-104">The **OWAUrl** element describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that hosts Outlook Web Access.</span></span> 
  
[<span data-ttu-id="1a1c7-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="1a1c7-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="1a1c7-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="1a1c7-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="1a1c7-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="1a1c7-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="1a1c7-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="1a1c7-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="1a1c7-109">Interne (POX)</span><span class="sxs-lookup"><span data-stu-id="1a1c7-109">Internal (POX)</span></span>](internal-pox.md)
  
[<span data-ttu-id="1a1c7-110">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1a1c7-110">OWAUrl (POX)</span></span>](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="1a1c7-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1a1c7-111">Attributes and elements</span></span>

<span data-ttu-id="1a1c7-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1a1c7-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a1c7-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="1a1c7-113">Attributes</span></span>

|<span data-ttu-id="1a1c7-114">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="1a1c7-114">**Attribute**</span></span>|<span data-ttu-id="1a1c7-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a1c7-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a1c7-116">**AuthenticationMethod**</span><span class="sxs-lookup"><span data-stu-id="1a1c7-116">**AuthenticationMethod**</span></span> <br/> |<span data-ttu-id="1a1c7-117">Décrit les méthodes d’authentification pour accéder à Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="1a1c7-117">Describes the authentication methods for accessing Outlook Web Access.</span></span>  <br/> |
   
#### <a name="authenticationmethod-attribute"></a><span data-ttu-id="1a1c7-118">Attribut AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="1a1c7-118">AuthenticationMethod Attribute</span></span>

|<span data-ttu-id="1a1c7-119">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="1a1c7-119">**Value**</span></span>|<span data-ttu-id="1a1c7-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a1c7-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a1c7-121">WindowsIntegrated</span><span class="sxs-lookup"><span data-stu-id="1a1c7-121">WindowsIntegrated</span></span>  <br/> |<span data-ttu-id="1a1c7-122">Authentification Windows intégrée.</span><span class="sxs-lookup"><span data-stu-id="1a1c7-122">Integrated Windows authentication.</span></span>  <br/> |
|<span data-ttu-id="1a1c7-123">AVEC AUTHENTIFICATION PAR FORMULAIRE</span><span class="sxs-lookup"><span data-stu-id="1a1c7-123">FBA</span></span>  <br/> |<span data-ttu-id="1a1c7-124">Authentification basée sur les formulaires.</span><span class="sxs-lookup"><span data-stu-id="1a1c7-124">Forms-based authentication.</span></span>  <br/> |
|<span data-ttu-id="1a1c7-125">NTLM</span><span class="sxs-lookup"><span data-stu-id="1a1c7-125">NTLM</span></span>  <br/> |<span data-ttu-id="1a1c7-126">Authentification NTLM.</span><span class="sxs-lookup"><span data-stu-id="1a1c7-126">NTLM authentication.</span></span>  <br/> |
|<span data-ttu-id="1a1c7-127">Digest</span><span class="sxs-lookup"><span data-stu-id="1a1c7-127">Digest</span></span>  <br/> |<span data-ttu-id="1a1c7-128">Authentification Digest.</span><span class="sxs-lookup"><span data-stu-id="1a1c7-128">Digest authentication.</span></span>  <br/> |
|<span data-ttu-id="1a1c7-129">Basic</span><span class="sxs-lookup"><span data-stu-id="1a1c7-129">Basic</span></span>  <br/> |<span data-ttu-id="1a1c7-130">Authentification de base.</span><span class="sxs-lookup"><span data-stu-id="1a1c7-130">Basic authentication.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1a1c7-131">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1a1c7-131">Child elements</span></span>

<span data-ttu-id="1a1c7-132">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1a1c7-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1a1c7-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1a1c7-133">Parent elements</span></span>

|<span data-ttu-id="1a1c7-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1a1c7-134">**Element**</span></span>|<span data-ttu-id="1a1c7-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="1a1c7-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a1c7-136">Interne (POX)</span><span class="sxs-lookup"><span data-stu-id="1a1c7-136">Internal (POX)</span></span>](internal-pox.md) <br/> |<span data-ttu-id="1a1c7-137">Contient la collection d’URL Outlook Web Access un client peut se connecter à lorsqu’il est à l’intérieur du pare-feu.</span><span class="sxs-lookup"><span data-stu-id="1a1c7-137">Contains the collection of Outlook Web Access URLs that a client can connect to when it is inside the firewall.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a1c7-138">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1a1c7-138">Text value</span></span>

<span data-ttu-id="1a1c7-139">La valeur de text représente l’URL pour le service d’Outlook Web Access sur un serveur d’accès au Client.</span><span class="sxs-lookup"><span data-stu-id="1a1c7-139">The text value represents the URL for the Outlook Web Access service on a Client Access server.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="1a1c7-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1a1c7-140">See also</span></span>



[<span data-ttu-id="1a1c7-141">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="1a1c7-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

