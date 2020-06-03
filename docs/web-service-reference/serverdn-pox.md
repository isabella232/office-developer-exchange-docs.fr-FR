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
description: L’élément ServerDN spécifie le nom unique de l’ordinateur qui exécute Microsoft Exchange Server 2007.
ms.openlocfilehash: 16c6e7368e221b7e54c8d7d63532bb29464a7e54
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461995"
---
# <a name="serverdn-pox"></a><span data-ttu-id="0bf8e-103">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="0bf8e-103">ServerDN (POX)</span></span>

<span data-ttu-id="0bf8e-104">L’élément **ServerDN** spécifie le nom unique de l’ordinateur qui exécute Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="0bf8e-104">The **ServerDN** element specifies the distinguished name of the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="0bf8e-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="0bf8e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="0bf8e-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="0bf8e-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="0bf8e-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="0bf8e-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="0bf8e-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="0bf8e-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="0bf8e-109">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="0bf8e-109">ServerDN (POX)</span></span>](serverdn-pox.md)
  
```xml
<ServerDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0bf8e-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0bf8e-110">Attributes and elements</span></span>

<span data-ttu-id="0bf8e-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0bf8e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bf8e-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="0bf8e-112">Attributes</span></span>

<span data-ttu-id="0bf8e-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0bf8e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bf8e-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0bf8e-114">Child elements</span></span>

<span data-ttu-id="0bf8e-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0bf8e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0bf8e-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0bf8e-116">Parent elements</span></span>

|<span data-ttu-id="0bf8e-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0bf8e-117">**Element**</span></span>|<span data-ttu-id="0bf8e-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="0bf8e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bf8e-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="0bf8e-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="0bf8e-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0bf8e-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0bf8e-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0bf8e-121">Text value</span></span>

<span data-ttu-id="0bf8e-122">La valeur de texte représente le nom unique du serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bf8e-122">The text value represents the distinguished name of the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0bf8e-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="0bf8e-123">Remarks</span></span>

<span data-ttu-id="0bf8e-124">La valeur **ServerDN** est utilisée uniquement lorsque [type (POX)](type-pox.md) est égal à Exch.</span><span class="sxs-lookup"><span data-stu-id="0bf8e-124">The **ServerDN** value is only used when [Type (POX)](type-pox.md) is equal to EXCH.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0bf8e-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0bf8e-125">See also</span></span>



[<span data-ttu-id="0bf8e-126">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0bf8e-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

