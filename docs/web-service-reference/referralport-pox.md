---
title: ReferralPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cd693f1e-fed4-4eb9-8297-178906f47050
description: L’élément ReferralPort spécifie le port utilisé pour obtenir une référence à un annuaire.
ms.openlocfilehash: 6b3968d7b2f252439d2dfbc647bd8337668cf818
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456793"
---
# <a name="referralport-pox"></a><span data-ttu-id="c8e3c-103">ReferralPort (POX)</span><span class="sxs-lookup"><span data-stu-id="c8e3c-103">ReferralPort (POX)</span></span>

<span data-ttu-id="c8e3c-104">L’élément **ReferralPort** spécifie le port utilisé pour obtenir une référence à un annuaire.</span><span class="sxs-lookup"><span data-stu-id="c8e3c-104">The **ReferralPort** element specifies the port that is used to get a referral to a directory.</span></span> 
  
[<span data-ttu-id="c8e3c-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="c8e3c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="c8e3c-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="c8e3c-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="c8e3c-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="c8e3c-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="c8e3c-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="c8e3c-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="c8e3c-109">ReferralPort (POX)</span><span class="sxs-lookup"><span data-stu-id="c8e3c-109">ReferralPort (POX)</span></span>](referralport-pox.md)
  
```xml
<ReferralPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="c8e3c-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c8e3c-110">Attributes and elements</span></span>

<span data-ttu-id="c8e3c-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c8e3c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8e3c-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="c8e3c-112">Attributes</span></span>

<span data-ttu-id="c8e3c-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c8e3c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8e3c-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c8e3c-114">Child elements</span></span>

<span data-ttu-id="c8e3c-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c8e3c-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8e3c-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c8e3c-116">Parent elements</span></span>

|<span data-ttu-id="c8e3c-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c8e3c-117">**Element**</span></span>|<span data-ttu-id="c8e3c-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="c8e3c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8e3c-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="c8e3c-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="c8e3c-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c8e3c-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c8e3c-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="c8e3c-121">Text value</span></span>

<span data-ttu-id="c8e3c-122">La valeur de texte représente le port utilisé pour accéder au serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c8e3c-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c8e3c-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="c8e3c-123">Remarks</span></span>

<span data-ttu-id="c8e3c-124">L’élément **ReferralPort** est utilisé uniquement lorsque l’élément [type (POX)](type-pox.md) est égal à Exch ou Expr.</span><span class="sxs-lookup"><span data-stu-id="c8e3c-124">The **ReferralPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c8e3c-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c8e3c-125">See also</span></span>



[<span data-ttu-id="c8e3c-126">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="c8e3c-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

