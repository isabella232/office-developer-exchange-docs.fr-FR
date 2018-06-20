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
ms.openlocfilehash: f314b9d27d1b4ee472d249ec49af1a785ff9ac25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756030"
---
# <a name="domainrequired-pox"></a><span data-ttu-id="c2756-103">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="c2756-103">DomainRequired (POX)</span></span>

<span data-ttu-id="c2756-104">L’élément **DomainRequired** indique si le domaine est requis pour l’authentification.</span><span class="sxs-lookup"><span data-stu-id="c2756-104">The **DomainRequired** element indicates whether the domain is required for authentication.</span></span> 
  
- [<span data-ttu-id="c2756-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="c2756-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="c2756-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="c2756-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="c2756-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="c2756-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="c2756-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="c2756-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="c2756-109">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="c2756-109">DomainRequired (POX)</span></span>](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="c2756-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c2756-110">Attributes and elements</span></span>

<span data-ttu-id="c2756-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c2756-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2756-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="c2756-112">Attributes</span></span>

<span data-ttu-id="c2756-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c2756-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2756-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c2756-114">Child elements</span></span>

<span data-ttu-id="c2756-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c2756-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c2756-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c2756-116">Parent elements</span></span>

|<span data-ttu-id="c2756-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c2756-117">**Element**</span></span>|<span data-ttu-id="c2756-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="c2756-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2756-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="c2756-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="c2756-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="c2756-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2756-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c2756-121">Text value</span></span>

<span data-ttu-id="c2756-122">La valeur de texte indique si le domaine est requis pour l’authentification.</span><span class="sxs-lookup"><span data-stu-id="c2756-122">The text value indicates whether the domain is required for authentication.</span></span> <span data-ttu-id="c2756-123">Les valeurs possibles sont **on** et **off**.</span><span class="sxs-lookup"><span data-stu-id="c2756-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="c2756-124">Si la valeur est **activée**, la requête suivante doit contenir le domaine du compte de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c2756-124">If the value is **on**, the subsequent request must contain the domain of the user's account.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c2756-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="c2756-125">Remarks</span></span>

<span data-ttu-id="c2756-126">Si le domaine n’est pas spécifié dans l’élément [LoginName (POX)](loginname-pox.md) ou l’élément **LoginName** n’a pas été spécifié, l’utilisateur doit entrer le domaine avant l’authentification réussit.</span><span class="sxs-lookup"><span data-stu-id="c2756-126">If the domain is not specified in the [LoginName (POX)](loginname-pox.md) element, or the **LoginName** element was not specified, the user must enter the domain before authentication will succeed.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c2756-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c2756-127">See also</span></span>

- [<span data-ttu-id="c2756-128">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="c2756-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

