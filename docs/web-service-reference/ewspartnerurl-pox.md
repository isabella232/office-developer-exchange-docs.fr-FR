---
title: EwsPartnerUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: L’élément EwsPartnerUrl spécifie l’URL de la meilleure instance de point de terminaison pour les services Web Exchange (EWS) pour un utilisateur à extension messagerie.
ms.openlocfilehash: a67eb17bb3db67a922c53ba5e37900ee0a9b956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526108"
---
# <a name="ewspartnerurl-pox"></a><span data-ttu-id="9a4c4-103">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="9a4c4-103">EwsPartnerUrl (POX)</span></span>

<span data-ttu-id="9a4c4-104">L’élément **EwsPartnerUrl** spécifie l’URL de la meilleure instance de point de terminaison pour les services Web Exchange (EWS) pour un utilisateur à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="9a4c4-104">The **EwsPartnerUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="9a4c4-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="9a4c4-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="9a4c4-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="9a4c4-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="9a4c4-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="9a4c4-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="9a4c4-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="9a4c4-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="9a4c4-109">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="9a4c4-109">EwsPartnerUrl (POX)</span></span>](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9a4c4-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9a4c4-110">Attributes and elements</span></span>

<span data-ttu-id="9a4c4-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9a4c4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a4c4-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="9a4c4-112">Attributes</span></span>

<span data-ttu-id="9a4c4-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9a4c4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a4c4-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9a4c4-114">Child elements</span></span>

<span data-ttu-id="9a4c4-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9a4c4-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9a4c4-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9a4c4-116">Parent elements</span></span>

|<span data-ttu-id="9a4c4-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9a4c4-117">**Element**</span></span>|<span data-ttu-id="9a4c4-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="9a4c4-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a4c4-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="9a4c4-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="9a4c4-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9a4c4-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a4c4-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="9a4c4-121">Text value</span></span>

<span data-ttu-id="9a4c4-122">La valeur de texte représente l’URL du point de terminaison EWS de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="9a4c4-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a4c4-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="9a4c4-123">Remarks</span></span>

<span data-ttu-id="9a4c4-124">L’élément **EwsPartnerUrl** est un élément enfant facultatif de l’élément **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="9a4c4-124">The **EwsPartnerUrl** element is an optional child element of the **Protocol** element.</span></span> <span data-ttu-id="9a4c4-125">Elle est équivalente à l’élément [EwsUrl (POX)](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="9a4c4-125">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="9a4c4-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9a4c4-126">See also</span></span>



[<span data-ttu-id="9a4c4-127">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="9a4c4-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

