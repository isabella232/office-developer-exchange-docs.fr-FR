---
title: DomainName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: L’élément DomainName Spécifie le domaine de l’utilisateur.
ms.openlocfilehash: c38d2e470bd174ab6dd7e5e1dd3eee23daea5e69
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756034"
---
# <a name="domainname-pox"></a><span data-ttu-id="aab1b-103">DomainName (POX)</span><span class="sxs-lookup"><span data-stu-id="aab1b-103">DomainName (POX)</span></span>

<span data-ttu-id="aab1b-104">L’élément **DomainName** Spécifie le domaine de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="aab1b-104">The **DomainName** element specifies the user's domain.</span></span> 
  
- [<span data-ttu-id="aab1b-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="aab1b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="aab1b-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="aab1b-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="aab1b-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="aab1b-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="aab1b-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="aab1b-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="aab1b-109">DomainName (POX)</span><span class="sxs-lookup"><span data-stu-id="aab1b-109">DomainName (POX)</span></span>](domainname-pox.md)
  
```xml
<DomainName/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="aab1b-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="aab1b-110">Attributes and elements</span></span>

<span data-ttu-id="aab1b-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="aab1b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aab1b-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="aab1b-112">Attributes</span></span>

<span data-ttu-id="aab1b-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aab1b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aab1b-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="aab1b-114">Child elements</span></span>

<span data-ttu-id="aab1b-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="aab1b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aab1b-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="aab1b-116">Parent elements</span></span>

|<span data-ttu-id="aab1b-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="aab1b-117">**Element**</span></span>|<span data-ttu-id="aab1b-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="aab1b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aab1b-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="aab1b-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="aab1b-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="aab1b-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aab1b-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="aab1b-121">Text value</span></span>

<span data-ttu-id="aab1b-122">La valeur texte spécifie le domaine de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="aab1b-122">The text value specifies the user's domain.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aab1b-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="aab1b-123">Remarks</span></span>

<span data-ttu-id="aab1b-124">Si aucune valeur n’est pas spécifié, l’authentification par défaut consiste à utiliser l’adresse de messagerie comme un format nom utilisateur principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="aab1b-124">If no value is specified, the default authentication is to use the e-mail address as a user principal name (UPN) format.</span></span> <span data-ttu-id="aab1b-125">Par exemple : \<nom d’utilisateur\>@\<domaine\>.</span><span class="sxs-lookup"><span data-stu-id="aab1b-125">For example: \<Username\>@\<Domain\>.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="aab1b-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="aab1b-126">See also</span></span>

- [<span data-ttu-id="aab1b-127">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="aab1b-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

