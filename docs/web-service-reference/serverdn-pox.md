---
title: ServerDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2ef73d13-e8bb-43f6-96c7-3ee157fed739
description: L’élément ServerDN Spécifie le nom unique de l’ordinateur qui exécute Microsoft Exchange Server 2007.
ms.openlocfilehash: d2b9ce663d8245a78acd088b0622406c0dfcb4da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829374"
---
# <a name="serverdn-pox"></a><span data-ttu-id="d5565-103">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="d5565-103">ServerDN (POX)</span></span>

<span data-ttu-id="d5565-104">L’élément **ServerDN** Spécifie le nom unique de l’ordinateur qui exécute Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="d5565-104">The **ServerDN** element specifies the distinguished name of the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="d5565-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="d5565-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d5565-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="d5565-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d5565-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="d5565-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d5565-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="d5565-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="d5565-109">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="d5565-109">ServerDN (POX)</span></span>](serverdn-pox.md)
  
```xml
<ServerDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d5565-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d5565-110">Attributes and elements</span></span>

<span data-ttu-id="d5565-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d5565-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5565-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="d5565-112">Attributes</span></span>

<span data-ttu-id="d5565-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d5565-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5565-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d5565-114">Child elements</span></span>

<span data-ttu-id="d5565-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d5565-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d5565-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d5565-116">Parent elements</span></span>

|<span data-ttu-id="d5565-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d5565-117">**Element**</span></span>|<span data-ttu-id="d5565-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="d5565-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5565-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="d5565-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="d5565-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="d5565-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d5565-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d5565-121">Text value</span></span>

<span data-ttu-id="d5565-122">La valeur de texte représente le nom unique du serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5565-122">The text value represents the distinguished name of the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d5565-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="d5565-123">Remarks</span></span>

<span data-ttu-id="d5565-124">La valeur **ServerDN** est uniquement utilisée lorsque [Type (POX)](type-pox.md) est égal à change</span><span class="sxs-lookup"><span data-stu-id="d5565-124">The **ServerDN** value is only used when [Type (POX)](type-pox.md) is equal to EXCH.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d5565-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d5565-125">See also</span></span>



[<span data-ttu-id="d5565-126">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d5565-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

