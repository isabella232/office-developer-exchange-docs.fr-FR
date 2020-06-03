---
title: DirectoryPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: L’élément DirectoryPort spécifie le port utilisé pour se connecter à l’annuaire lorsque le protocole NSPI (Name Service Provider Interface) est utilisé.
ms.openlocfilehash: 2ba0a15cea0b4eb9b6069fab384edb3d9747a360
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462086"
---
# <a name="directoryport-pox"></a><span data-ttu-id="d485d-103">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="d485d-103">DirectoryPort (POX)</span></span>

<span data-ttu-id="d485d-104">L’élément **DirectoryPort** spécifie le port utilisé pour se connecter à l’annuaire lorsque le protocole NSPI (Name Service Provider Interface) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="d485d-104">The **DirectoryPort** element specifies the port that is used to connect to the directory when the Name Service Provider Interface (NSPI) protocol is used.</span></span> 
  
- [<span data-ttu-id="d485d-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="d485d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="d485d-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="d485d-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="d485d-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="d485d-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="d485d-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="d485d-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="d485d-109">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="d485d-109">DirectoryPort (POX)</span></span>](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d485d-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d485d-110">Attributes and elements</span></span>

<span data-ttu-id="d485d-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d485d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d485d-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="d485d-112">Attributes</span></span>

<span data-ttu-id="d485d-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d485d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d485d-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d485d-114">Child elements</span></span>

<span data-ttu-id="d485d-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d485d-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d485d-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d485d-116">Parent elements</span></span>

|<span data-ttu-id="d485d-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d485d-117">**Element**</span></span>|<span data-ttu-id="d485d-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="d485d-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d485d-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="d485d-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="d485d-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d485d-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d485d-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="d485d-121">Text value</span></span>

<span data-ttu-id="d485d-122">La valeur de texte représente le port utilisé pour accéder au serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="d485d-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d485d-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="d485d-123">Remarks</span></span>

<span data-ttu-id="d485d-124">L’élément **DirectoryPort** est utilisé uniquement lorsque l’élément [type (POX)](type-pox.md) est égal à Exch ou Expr.</span><span class="sxs-lookup"><span data-stu-id="d485d-124">The **DirectoryPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d485d-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d485d-125">See also</span></span>

- [<span data-ttu-id="d485d-126">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d485d-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

