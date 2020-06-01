---
title: UsePOPAuth (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 28f552d8-6bb8-49b4-a45c-b2053670f1cc
description: L’élément UsePOPAuth indique si les informations d’authentification fournies pour un type de compte POP3 sont également utilisées pour le protocole SMTP (Simple Mail Transfer Protocol).
ms.openlocfilehash: 8d5bfffaab31c382ad43915e18b8a7a2b2737c21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466506"
---
# <a name="usepopauth-pox"></a><span data-ttu-id="ca3cf-103">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="ca3cf-103">UsePOPAuth (POX)</span></span>

<span data-ttu-id="ca3cf-104">L’élément **UsePOPAuth** indique si les informations d’authentification fournies pour un type de compte POP3 sont également utilisées pour le protocole SMTP (Simple Mail Transfer Protocol).</span><span class="sxs-lookup"><span data-stu-id="ca3cf-104">The **UsePOPAuth** element indicates whether the authentication information that is provided for a POP3 type of account is also used for Simple Mail Transfer Protocol (SMTP).</span></span> 
  
[<span data-ttu-id="ca3cf-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="ca3cf-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="ca3cf-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="ca3cf-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="ca3cf-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="ca3cf-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="ca3cf-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="ca3cf-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="ca3cf-109">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="ca3cf-109">UsePOPAuth (POX)</span></span>](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="ca3cf-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ca3cf-110">Attributes and elements</span></span>

<span data-ttu-id="ca3cf-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ca3cf-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca3cf-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="ca3cf-112">Attributes</span></span>

<span data-ttu-id="ca3cf-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ca3cf-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca3cf-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ca3cf-114">Child elements</span></span>

<span data-ttu-id="ca3cf-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ca3cf-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ca3cf-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ca3cf-116">Parent elements</span></span>

|<span data-ttu-id="ca3cf-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ca3cf-117">**Element**</span></span>|<span data-ttu-id="ca3cf-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="ca3cf-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca3cf-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="ca3cf-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="ca3cf-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ca3cf-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ca3cf-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ca3cf-121">Text value</span></span>

<span data-ttu-id="ca3cf-122">La valeur Text indique si les informations d’authentification fournies pour un type de compte POP3 sont également utilisées pour SMTP.</span><span class="sxs-lookup"><span data-stu-id="ca3cf-122">The text value indicates whether the authentication information that is provided for a POP3 type of account is also used for SMTP.</span></span> <span data-ttu-id="ca3cf-123">Les valeurs possibles sont **on** et **off**.</span><span class="sxs-lookup"><span data-stu-id="ca3cf-123">The possible values are **on** and **off**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ca3cf-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="ca3cf-124">Remarks</span></span>

<span data-ttu-id="ca3cf-125">L’élément **UsePOPAuth** est utilisé uniquement lorsque [type (POX)](type-pox.md) est SMTP.</span><span class="sxs-lookup"><span data-stu-id="ca3cf-125">The **UsePOPAuth** element is only used when [Type (POX)](type-pox.md) is SMTP.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ca3cf-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ca3cf-126">See also</span></span>



[<span data-ttu-id="ca3cf-127">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ca3cf-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

