---
title: EwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 73cebc8c-770a-4f1b-b93e-51e7e2f3e342
description: L’élément EwsUrl spécifie l’URL de la meilleure instance de point de terminaison pour les services Web Exchange (EWS) pour un utilisateur à extension messagerie.
ms.openlocfilehash: 295e65ddf14524a41c5cb714df78703dbf855a05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454350"
---
# <a name="ewsurl-pox"></a><span data-ttu-id="2dce2-103">EwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="2dce2-103">EwsUrl (POX)</span></span>

<span data-ttu-id="2dce2-104">L’élément **EwsUrl** spécifie l’URL de la meilleure instance de point de terminaison pour les services Web Exchange (EWS) pour un utilisateur à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="2dce2-104">The **EwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="2dce2-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="2dce2-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="2dce2-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="2dce2-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="2dce2-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="2dce2-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="2dce2-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="2dce2-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="2dce2-109">EwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="2dce2-109">EwsUrl (POX)</span></span>](ewsurl-pox.md)
  
```XML
<EwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="2dce2-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2dce2-110">Attributes and elements</span></span>

<span data-ttu-id="2dce2-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2dce2-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2dce2-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="2dce2-112">Attributes</span></span>

<span data-ttu-id="2dce2-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2dce2-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2dce2-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2dce2-114">Child elements</span></span>

<span data-ttu-id="2dce2-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2dce2-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2dce2-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2dce2-116">Parent elements</span></span>

|<span data-ttu-id="2dce2-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2dce2-117">**Element**</span></span>|<span data-ttu-id="2dce2-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="2dce2-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2dce2-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="2dce2-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="2dce2-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2dce2-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2dce2-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="2dce2-121">Text value</span></span>

<span data-ttu-id="2dce2-122">La valeur de texte représente l’URL du point de terminaison EWS de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="2dce2-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2dce2-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="2dce2-123">Remarks</span></span>

<span data-ttu-id="2dce2-124">L’élément **EwsUrl** est un élément enfant facultatif de l’élément **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="2dce2-124">The **EwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2dce2-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2dce2-125">See also</span></span>



[<span data-ttu-id="2dce2-126">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="2dce2-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

