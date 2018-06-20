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
description: L’élément DirectoryPort Spécifie le port utilisé pour se connecter au répertoire lorsque le protocole fournisseur Interface NSPI (Name Service) est utilisé.
ms.openlocfilehash: 1b73b9cd1d21c73f4e897684371993312f741322
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755935"
---
# <a name="directoryport-pox"></a><span data-ttu-id="7da44-103">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="7da44-103">DirectoryPort (POX)</span></span>

<span data-ttu-id="7da44-104">L’élément **DirectoryPort** Spécifie le port utilisé pour se connecter au répertoire lorsque le protocole fournisseur Interface NSPI (Name Service) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="7da44-104">The **DirectoryPort** element specifies the port that is used to connect to the directory when the Name Service Provider Interface (NSPI) protocol is used.</span></span> 
  
- [<span data-ttu-id="7da44-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="7da44-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="7da44-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="7da44-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="7da44-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="7da44-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="7da44-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="7da44-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="7da44-109">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="7da44-109">DirectoryPort (POX)</span></span>](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="7da44-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7da44-110">Attributes and elements</span></span>

<span data-ttu-id="7da44-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7da44-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7da44-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="7da44-112">Attributes</span></span>

<span data-ttu-id="7da44-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7da44-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7da44-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7da44-114">Child elements</span></span>

<span data-ttu-id="7da44-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7da44-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7da44-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7da44-116">Parent elements</span></span>

|<span data-ttu-id="7da44-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7da44-117">**Element**</span></span>|<span data-ttu-id="7da44-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="7da44-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7da44-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="7da44-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="7da44-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="7da44-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7da44-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7da44-121">Text value</span></span>

<span data-ttu-id="7da44-122">La valeur de texte représente le port utilisé pour accéder au serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="7da44-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7da44-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="7da44-123">Remarks</span></span>

<span data-ttu-id="7da44-124">L’élément **DirectoryPort** est uniquement utilisé lorsque l’élément de [Type (POX)](type-pox.md) est égale à EXCH ou EXPR.</span><span class="sxs-lookup"><span data-stu-id="7da44-124">The **DirectoryPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7da44-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7da44-125">See also</span></span>

- [<span data-ttu-id="7da44-126">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7da44-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

