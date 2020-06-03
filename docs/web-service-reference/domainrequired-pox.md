---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: L’élément DomainRequired indique si le domaine est requis pour l’authentification.
ms.openlocfilehash: 97d602c40b247f9a6650cc4440b53bf23c18482e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461323"
---
# <a name="domainrequired-pox"></a><span data-ttu-id="79e10-103">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="79e10-103">DomainRequired (POX)</span></span>

<span data-ttu-id="79e10-104">L’élément **DomainRequired** indique si le domaine est requis pour l’authentification.</span><span class="sxs-lookup"><span data-stu-id="79e10-104">The **DomainRequired** element indicates whether the domain is required for authentication.</span></span> 
  
- [<span data-ttu-id="79e10-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="79e10-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="79e10-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="79e10-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="79e10-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="79e10-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="79e10-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="79e10-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="79e10-109">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="79e10-109">DomainRequired (POX)</span></span>](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="79e10-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="79e10-110">Attributes and elements</span></span>

<span data-ttu-id="79e10-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="79e10-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79e10-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="79e10-112">Attributes</span></span>

<span data-ttu-id="79e10-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="79e10-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79e10-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="79e10-114">Child elements</span></span>

<span data-ttu-id="79e10-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79e10-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79e10-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="79e10-116">Parent elements</span></span>

|<span data-ttu-id="79e10-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="79e10-117">**Element**</span></span>|<span data-ttu-id="79e10-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="79e10-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79e10-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="79e10-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="79e10-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="79e10-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79e10-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="79e10-121">Text value</span></span>

<span data-ttu-id="79e10-122">La valeur Text indique si le domaine est requis pour l’authentification.</span><span class="sxs-lookup"><span data-stu-id="79e10-122">The text value indicates whether the domain is required for authentication.</span></span> <span data-ttu-id="79e10-123">Les valeurs possibles sont **on** et **off**.</span><span class="sxs-lookup"><span data-stu-id="79e10-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="79e10-124">Si la valeur est **activée**, la demande suivante doit contenir le domaine du compte de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="79e10-124">If the value is **on**, the subsequent request must contain the domain of the user's account.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="79e10-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="79e10-125">Remarks</span></span>

<span data-ttu-id="79e10-126">Si le domaine n’est pas spécifié dans l’élément [LoginName (POX)](loginname-pox.md) ou si l’élément **LoginName** n’a pas été spécifié, l’utilisateur doit entrer le domaine pour que l’authentification réussisse.</span><span class="sxs-lookup"><span data-stu-id="79e10-126">If the domain is not specified in the [LoginName (POX)](loginname-pox.md) element, or the **LoginName** element was not specified, the user must enter the domain before authentication will succeed.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="79e10-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79e10-127">See also</span></span>

- [<span data-ttu-id="79e10-128">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="79e10-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

