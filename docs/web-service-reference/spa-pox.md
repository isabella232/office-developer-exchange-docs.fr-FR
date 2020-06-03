---
title: SPA (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: fba018d5-0c65-4e1b-9767-d1ce8b356278
description: L’élément SPA indique si l’authentification par mot de passe sécurisé (SPA) est requise.
ms.openlocfilehash: cf57b3a6046b1b9b030b7cae81381189eee92c1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467640"
---
# <a name="spa-pox"></a><span data-ttu-id="13e89-103">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="13e89-103">SPA (POX)</span></span>

<span data-ttu-id="13e89-104">L’élément **Spa** indique si l’authentification par mot de passe sécurisé (Spa) est requise.</span><span class="sxs-lookup"><span data-stu-id="13e89-104">The **SPA** element indicates whether Secure Password Authentication (SPA) is required.</span></span> 
  
[<span data-ttu-id="13e89-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="13e89-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="13e89-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="13e89-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="13e89-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="13e89-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="13e89-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="13e89-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="13e89-109">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="13e89-109">SPA (POX)</span></span>](spa-pox.md)
  
```xml
<SPA/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="13e89-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="13e89-110">Attributes and elements</span></span>

<span data-ttu-id="13e89-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="13e89-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13e89-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="13e89-112">Attributes</span></span>

<span data-ttu-id="13e89-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="13e89-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="13e89-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="13e89-114">Child elements</span></span>

<span data-ttu-id="13e89-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="13e89-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="13e89-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="13e89-116">Parent elements</span></span>

|<span data-ttu-id="13e89-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="13e89-117">**Element**</span></span>|<span data-ttu-id="13e89-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="13e89-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13e89-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="13e89-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="13e89-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="13e89-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="13e89-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="13e89-121">Text value</span></span>

<span data-ttu-id="13e89-122">La valeur texte indique si SPA est requis.</span><span class="sxs-lookup"><span data-stu-id="13e89-122">The text value indicates whether SPA is required.</span></span> <span data-ttu-id="13e89-123">Si la valeur du texte est **activée**, Spa est requis.</span><span class="sxs-lookup"><span data-stu-id="13e89-123">If the text value is **on**, SPA is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="13e89-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="13e89-124">Remarks</span></span>

<span data-ttu-id="13e89-125">Si cet élément n’est pas présent, la valeur par défaut est définie **sur on**.</span><span class="sxs-lookup"><span data-stu-id="13e89-125">If this element is not present, the default value is set to **on**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="13e89-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="13e89-126">See also</span></span>



[<span data-ttu-id="13e89-127">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="13e89-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

