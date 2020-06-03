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
description: L’élément User fournit des informations spécifiques à l’utilisateur.
ms.openlocfilehash: 8f53319bcf34595305748adafc9aa1e25283611e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530217"
---
# <a name="user-pox"></a><span data-ttu-id="e645f-103">Utilisateur (POX)</span><span class="sxs-lookup"><span data-stu-id="e645f-103">User (POX)</span></span>

<span data-ttu-id="e645f-104">L’élément **User** fournit des informations spécifiques à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e645f-104">The **User** element provides user-specific information.</span></span> 
  
[<span data-ttu-id="e645f-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="e645f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="e645f-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="e645f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="e645f-107">Utilisateur (POX)</span><span class="sxs-lookup"><span data-stu-id="e645f-107">User (POX)</span></span>](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="e645f-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e645f-108">Attributes and elements</span></span>

<span data-ttu-id="e645f-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e645f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e645f-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="e645f-110">Attributes</span></span>

<span data-ttu-id="e645f-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e645f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e645f-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e645f-112">Child elements</span></span>

|<span data-ttu-id="e645f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e645f-113">**Element**</span></span>|<span data-ttu-id="e645f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="e645f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e645f-115">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="e645f-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="e645f-116">Représente le nom d’affichage de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e645f-116">Represents the user's display name.</span></span>  <br/> |
|[<span data-ttu-id="e645f-117">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="e645f-117">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="e645f-118">Identifie la boîte aux lettres d’un utilisateur par le nom unique hérité.</span><span class="sxs-lookup"><span data-stu-id="e645f-118">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="e645f-119">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="e645f-119">DeploymentId (POX)</span></span>](deploymentid-pox.md) <br/> |<span data-ttu-id="e645f-120">Identifie de manière unique la forêt Exchange.</span><span class="sxs-lookup"><span data-stu-id="e645f-120">Uniquely identifies the Exchange forest.</span></span>  <br/> |
|[<span data-ttu-id="e645f-121">AutoDiscoverSMTPAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="e645f-121">AutoDiscoverSMTPAddress (POX)</span></span>](autodiscoversmtpaddress-pox.md) <br/> |<span data-ttu-id="e645f-122">Contient l’adresse SMTP de l’utilisateur qui est utilisée pour le processus de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="e645f-122">Contains the user's SMTP address that is used for the Autodiscover process.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e645f-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e645f-123">Parent elements</span></span>

|<span data-ttu-id="e645f-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e645f-124">**Element**</span></span>|<span data-ttu-id="e645f-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="e645f-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e645f-126">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="e645f-126">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="e645f-127">Contient la réponse du service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="e645f-127">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e645f-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="e645f-128">Remarks</span></span>

<span data-ttu-id="e645f-129">Les demandes et les réponses de découverte automatique doivent être codées au format UTF-8.</span><span class="sxs-lookup"><span data-stu-id="e645f-129">Autodiscover requests and responses must be UTF-8 encoded.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e645f-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e645f-130">See also</span></span>



[<span data-ttu-id="e645f-131">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e645f-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

