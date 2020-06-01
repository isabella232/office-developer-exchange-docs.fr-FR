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
ms.openlocfilehash: 4986a3404763e88fb3e84d52a5d30d54c810f93a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467920"
---
# <a name="deploymentid-pox"></a><span data-ttu-id="c94ac-103">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="c94ac-103">DeploymentId (POX)</span></span>

<span data-ttu-id="c94ac-104">L’élément **deploymentId** identifie de manière unique la forêt Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="c94ac-104">The **DeploymentId** element uniquely identifies the Microsoft Exchange Server 2007 forest.</span></span> 
  
- [<span data-ttu-id="c94ac-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="c94ac-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="c94ac-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="c94ac-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="c94ac-107">Utilisateur (POX)</span><span class="sxs-lookup"><span data-stu-id="c94ac-107">User (POX)</span></span>](user-pox.md)  
- [<span data-ttu-id="c94ac-108">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="c94ac-108">DeploymentId (POX)</span></span>](deploymentid-pox.md)
  
```xml
<DeploymentId/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="c94ac-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c94ac-109">Attributes and elements</span></span>

<span data-ttu-id="c94ac-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c94ac-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c94ac-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="c94ac-111">Attributes</span></span>

<span data-ttu-id="c94ac-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c94ac-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c94ac-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c94ac-113">Child elements</span></span>

<span data-ttu-id="c94ac-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c94ac-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c94ac-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c94ac-115">Parent elements</span></span>

|<span data-ttu-id="c94ac-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c94ac-116">**Element**</span></span>|<span data-ttu-id="c94ac-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c94ac-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c94ac-118">Utilisateur (POX)</span><span class="sxs-lookup"><span data-stu-id="c94ac-118">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="c94ac-119">Fournit des informations spécifiques à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c94ac-119">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c94ac-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="c94ac-120">Text value</span></span>

<span data-ttu-id="c94ac-121">La valeur Text identifie de manière unique la forêt Exchange 2007 au format GUID.</span><span class="sxs-lookup"><span data-stu-id="c94ac-121">The text value uniquely identifies the Exchange 2007 forest in GUID format.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c94ac-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="c94ac-122">Remarks</span></span>

<span data-ttu-id="c94ac-123">Si vous désinstallez, puis réinstallez Exchange 2007 et que vous utilisez le même nom de serveur, la valeur **deploymentId** change.</span><span class="sxs-lookup"><span data-stu-id="c94ac-123">If you uninstall and then reinstall Exchange 2007 and you use the same server name, the **DeploymentId** value changes.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c94ac-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c94ac-124">See also</span></span>

- [<span data-ttu-id="c94ac-125">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="c94ac-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

