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
description: L’élément UsePOPAuth indique si les informations d’authentification qui sont fournies pour un type de POP3 de compte sont également utilisées pour SMTP Simple Mail Transfer Protocol ().
ms.openlocfilehash: be03568d697b1f5461d49dba388a1d3f1008a67e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838940"
---
# <a name="usepopauth-pox"></a><span data-ttu-id="4694c-103">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="4694c-103">UsePOPAuth (POX)</span></span>

<span data-ttu-id="4694c-104">L’élément **UsePOPAuth** indique si les informations d’authentification qui sont fournies pour un type de POP3 de compte sont également utilisées pour SMTP Simple Mail Transfer Protocol ().</span><span class="sxs-lookup"><span data-stu-id="4694c-104">The **UsePOPAuth** element indicates whether the authentication information that is provided for a POP3 type of account is also used for Simple Mail Transfer Protocol (SMTP).</span></span> 
  
[<span data-ttu-id="4694c-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="4694c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="4694c-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="4694c-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="4694c-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="4694c-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="4694c-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="4694c-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="4694c-109">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="4694c-109">UsePOPAuth (POX)</span></span>](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="4694c-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4694c-110">Attributes and elements</span></span>

<span data-ttu-id="4694c-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4694c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4694c-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="4694c-112">Attributes</span></span>

<span data-ttu-id="4694c-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4694c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4694c-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4694c-114">Child elements</span></span>

<span data-ttu-id="4694c-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4694c-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4694c-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4694c-116">Parent elements</span></span>

|<span data-ttu-id="4694c-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4694c-117">**Element**</span></span>|<span data-ttu-id="4694c-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="4694c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4694c-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="4694c-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="4694c-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="4694c-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4694c-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4694c-121">Text value</span></span>

<span data-ttu-id="4694c-122">La valeur de texte indique si les informations d’authentification qui sont fournies pour un type de POP3 de compte sont également utilisées pour SMTP.</span><span class="sxs-lookup"><span data-stu-id="4694c-122">The text value indicates whether the authentication information that is provided for a POP3 type of account is also used for SMTP.</span></span> <span data-ttu-id="4694c-123">Les valeurs possibles sont **on** et **off**.</span><span class="sxs-lookup"><span data-stu-id="4694c-123">The possible values are **on** and **off**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4694c-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="4694c-124">Remarks</span></span>

<span data-ttu-id="4694c-125">L’élément **UsePOPAuth** est uniquement utilisé lorsque [Type (POX)](type-pox.md) est SMTP.</span><span class="sxs-lookup"><span data-stu-id="4694c-125">The **UsePOPAuth** element is only used when [Type (POX)](type-pox.md) is SMTP.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4694c-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4694c-126">See also</span></span>



[<span data-ttu-id="4694c-127">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="4694c-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

