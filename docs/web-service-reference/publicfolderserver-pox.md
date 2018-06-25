---
title: PublicFolderServer (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 37ad46ab-7817-4fdd-ad2d-26cb525cd96b
description: L’élément PublicFolderServer contient le nom de domaine complet (FQDN) du serveur de dossiers publics de l’utilisateur.
ms.openlocfilehash: 6fb2f1a97279ee7f2e94c008474ddfed088faea1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828928"
---
# <a name="publicfolderserver-pox"></a><span data-ttu-id="ec76b-103">PublicFolderServer (POX)</span><span class="sxs-lookup"><span data-stu-id="ec76b-103">PublicFolderServer (POX)</span></span>

<span data-ttu-id="ec76b-104">L’élément **PublicFolderServer** contient le nom de domaine complet (FQDN) du serveur de dossiers publics de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ec76b-104">The **PublicFolderServer** element contains the fully-qualified domain name (FQDN) of the public folder server for the user.</span></span> 
  
[<span data-ttu-id="ec76b-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="ec76b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="ec76b-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="ec76b-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="ec76b-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="ec76b-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="ec76b-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="ec76b-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="ec76b-109">PublicFolderServer (POX)</span><span class="sxs-lookup"><span data-stu-id="ec76b-109">PublicFolderServer (POX)</span></span>](publicfolderserver-pox.md)
  
```XML
<PublicFolderServer/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="ec76b-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ec76b-110">Attributes and elements</span></span>

<span data-ttu-id="ec76b-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ec76b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec76b-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="ec76b-112">Attributes</span></span>

<span data-ttu-id="ec76b-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ec76b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec76b-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ec76b-114">Child elements</span></span>

<span data-ttu-id="ec76b-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ec76b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ec76b-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ec76b-116">Parent elements</span></span>

|<span data-ttu-id="ec76b-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ec76b-117">**Element**</span></span>|<span data-ttu-id="ec76b-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec76b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec76b-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="ec76b-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="ec76b-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="ec76b-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ec76b-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ec76b-121">Text value</span></span>

<span data-ttu-id="ec76b-122">La valeur de texte représente le nom de domaine complet du serveur de dossiers publics de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ec76b-122">The text value represents the FQDN of the public folder server for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ec76b-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="ec76b-123">Remarks</span></span>

<span data-ttu-id="ec76b-124">L’élément **PublicFolderServer** est un élément enfant facultatif de l’élément de **protocole** .</span><span class="sxs-lookup"><span data-stu-id="ec76b-124">The **PublicFolderServer** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ec76b-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ec76b-125">See also</span></span>



[<span data-ttu-id="ec76b-126">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ec76b-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

