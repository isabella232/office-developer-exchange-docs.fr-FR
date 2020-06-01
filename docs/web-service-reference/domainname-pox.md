---
title: Nom_domaine (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: L’élément DomainName spécifie le domaine de l’utilisateur.
ms.openlocfilehash: ff38d6a876e396317dedece0a81a9f9f0db0f587
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458424"
---
# <a name="domainname-pox"></a><span data-ttu-id="a2b12-103">Nom_domaine (POX)</span><span class="sxs-lookup"><span data-stu-id="a2b12-103">DomainName (POX)</span></span>

<span data-ttu-id="a2b12-104">L’élément **DomainName** spécifie le domaine de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a2b12-104">The **DomainName** element specifies the user's domain.</span></span> 
  
- [<span data-ttu-id="a2b12-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="a2b12-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="a2b12-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="a2b12-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="a2b12-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="a2b12-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="a2b12-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="a2b12-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="a2b12-109">Nom_domaine (POX)</span><span class="sxs-lookup"><span data-stu-id="a2b12-109">DomainName (POX)</span></span>](domainname-pox.md)
  
```xml
<DomainName/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a2b12-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a2b12-110">Attributes and elements</span></span>

<span data-ttu-id="a2b12-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a2b12-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2b12-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="a2b12-112">Attributes</span></span>

<span data-ttu-id="a2b12-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a2b12-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2b12-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a2b12-114">Child elements</span></span>

<span data-ttu-id="a2b12-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a2b12-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a2b12-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a2b12-116">Parent elements</span></span>

|<span data-ttu-id="a2b12-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2b12-117">**Element**</span></span>|<span data-ttu-id="a2b12-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2b12-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2b12-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="a2b12-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a2b12-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a2b12-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a2b12-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a2b12-121">Text value</span></span>

<span data-ttu-id="a2b12-122">La valeur texte spécifie le domaine de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="a2b12-122">The text value specifies the user's domain.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a2b12-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="a2b12-123">Remarks</span></span>

<span data-ttu-id="a2b12-124">Si aucune valeur n’est spécifiée, l’authentification par défaut consiste à utiliser l’adresse de messagerie en tant que format de nom d’utilisateur principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="a2b12-124">If no value is specified, the default authentication is to use the e-mail address as a user principal name (UPN) format.</span></span> <span data-ttu-id="a2b12-125">Par exemple : \<Username\> @ \<Domain\> .</span><span class="sxs-lookup"><span data-stu-id="a2b12-125">For example: \<Username\>@\<Domain\>.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="a2b12-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a2b12-126">See also</span></span>

- [<span data-ttu-id="a2b12-127">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="a2b12-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

