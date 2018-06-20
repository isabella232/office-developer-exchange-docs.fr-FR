---
title: Utilisateur (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7c42b516-77f6-4aee-99d8-b866d82d793a
description: L’élément de l’utilisateur fournit des informations spécifiques à l’utilisateur.
ms.openlocfilehash: 3f90ff0cc00170170c7304f2a19fe1d7abd9d1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838944"
---
# <a name="user-pox"></a><span data-ttu-id="a2c84-103">Utilisateur (POX)</span><span class="sxs-lookup"><span data-stu-id="a2c84-103">User (POX)</span></span>

<span data-ttu-id="a2c84-104">L’élément de **l’utilisateur** fournit des informations spécifiques à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a2c84-104">The **User** element provides user-specific information.</span></span> 
  
[<span data-ttu-id="a2c84-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="a2c84-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="a2c84-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="a2c84-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="a2c84-107">Utilisateur (POX)</span><span class="sxs-lookup"><span data-stu-id="a2c84-107">User (POX)</span></span>](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a2c84-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a2c84-108">Attributes and elements</span></span>

<span data-ttu-id="a2c84-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a2c84-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2c84-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="a2c84-110">Attributes</span></span>

<span data-ttu-id="a2c84-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a2c84-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2c84-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a2c84-112">Child elements</span></span>

|<span data-ttu-id="a2c84-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2c84-113">**Element**</span></span>|<span data-ttu-id="a2c84-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2c84-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2c84-115">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="a2c84-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="a2c84-116">Représente le nom complet de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a2c84-116">Represents the user's display name.</span></span>  <br/> |
|[<span data-ttu-id="a2c84-117">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="a2c84-117">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="a2c84-118">Identifie la boîte aux lettres d’un utilisateur par un nom unique hérité.</span><span class="sxs-lookup"><span data-stu-id="a2c84-118">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="a2c84-119">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="a2c84-119">DeploymentId (POX)</span></span>](deploymentid-pox.md) <br/> |<span data-ttu-id="a2c84-120">Identifie de manière unique la forêt Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2c84-120">Uniquely identifies the Exchange forest.</span></span>  <br/> |
|[<span data-ttu-id="a2c84-121">AutoDiscoverSMTPAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="a2c84-121">AutoDiscoverSMTPAddress (POX)</span></span>](autodiscoversmtpaddress-pox.md) <br/> |<span data-ttu-id="a2c84-122">Contient l’adresse SMTP de l’utilisateur qui est utilisé pour le processus de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="a2c84-122">Contains the user's SMTP address that is used for the Autodiscover process.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2c84-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a2c84-123">Parent elements</span></span>

|<span data-ttu-id="a2c84-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2c84-124">**Element**</span></span>|<span data-ttu-id="a2c84-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2c84-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2c84-126">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="a2c84-126">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="a2c84-127">Contient la réponse du service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="a2c84-127">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2c84-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="a2c84-128">Remarks</span></span>

<span data-ttu-id="a2c84-129">Les réponses et les demandes de découverte automatique doivent être au format UTF-8.</span><span class="sxs-lookup"><span data-stu-id="a2c84-129">Autodiscover requests and responses must be UTF-8 encoded.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="a2c84-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a2c84-130">See also</span></span>



[<span data-ttu-id="a2c84-131">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="a2c84-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

