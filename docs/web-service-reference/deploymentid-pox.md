---
title: DeploymentId (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: L’élément DeploymentId identifie de manière unique la forêt Microsoft Exchange Server 2007.
ms.openlocfilehash: 4f2548709753d8407d02218acecd9233f0ba764f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755895"
---
# <a name="deploymentid-pox"></a><span data-ttu-id="7a417-103">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="7a417-103">DeploymentId (POX)</span></span>

<span data-ttu-id="7a417-104">L’élément **DeploymentId** identifie de manière unique la forêt Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="7a417-104">The **DeploymentId** element uniquely identifies the Microsoft Exchange Server 2007 forest.</span></span> 
  
- [<span data-ttu-id="7a417-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="7a417-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="7a417-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="7a417-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="7a417-107">Utilisateur (POX)</span><span class="sxs-lookup"><span data-stu-id="7a417-107">User (POX)</span></span>](user-pox.md)  
- [<span data-ttu-id="7a417-108">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="7a417-108">DeploymentId (POX)</span></span>](deploymentid-pox.md)
  
```xml
<DeploymentId/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="7a417-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7a417-109">Attributes and elements</span></span>

<span data-ttu-id="7a417-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7a417-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a417-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="7a417-111">Attributes</span></span>

<span data-ttu-id="7a417-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7a417-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a417-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7a417-113">Child elements</span></span>

<span data-ttu-id="7a417-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7a417-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7a417-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7a417-115">Parent elements</span></span>

|<span data-ttu-id="7a417-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7a417-116">**Element**</span></span>|<span data-ttu-id="7a417-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7a417-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a417-118">Utilisateur (POX)</span><span class="sxs-lookup"><span data-stu-id="7a417-118">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="7a417-119">Fournit des informations spécifiques à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7a417-119">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7a417-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7a417-120">Text value</span></span>

<span data-ttu-id="7a417-121">La valeur de texte identifie de manière unique la forêt Exchange 2007 au format GUID.</span><span class="sxs-lookup"><span data-stu-id="7a417-121">The text value uniquely identifies the Exchange 2007 forest in GUID format.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7a417-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="7a417-122">Remarks</span></span>

<span data-ttu-id="7a417-123">Si vous désinstallez et réinstallez Exchange 2007 et que vous utilisez le même nom de serveur, la valeur de **DeploymentId** est modifiée.</span><span class="sxs-lookup"><span data-stu-id="7a417-123">If you uninstall and then reinstall Exchange 2007 and you use the same server name, the **DeploymentId** value changes.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7a417-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7a417-124">See also</span></span>

- [<span data-ttu-id="7a417-125">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7a417-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

