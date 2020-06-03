---
title: EcpUrl-RET (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5f090fd2-b0c4-4ca0-a959-1433d73a2069
description: L’élément EcpUrl-RET spécifie une URL partielle pouvant être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour accéder aux paramètres de balise de rétention pour un utilisateur à extension messagerie.
ms.openlocfilehash: 1f6878dc58bb01fca6a56fdd645efd3363a3d442
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458690"
---
# <a name="ecpurl-ret-pox"></a><span data-ttu-id="0352e-103">EcpUrl-RET (POX)</span><span class="sxs-lookup"><span data-stu-id="0352e-103">EcpUrl-ret (POX)</span></span>

<span data-ttu-id="0352e-104">L’élément **EcpUrl-RET** spécifie une URL partielle pouvant être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de balise de rétention pour un utilisateur à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="0352e-104">The **EcpUrl-ret** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="0352e-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="0352e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="0352e-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="0352e-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="0352e-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="0352e-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="0352e-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="0352e-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="0352e-109">EcpUrl-RET (POX)</span><span class="sxs-lookup"><span data-stu-id="0352e-109">EcpUrl-ret (POX)</span></span>](ecpurl-ret-pox.md)
  
```XML
<EcpUrl-ret/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0352e-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0352e-110">Attributes and elements</span></span>

<span data-ttu-id="0352e-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0352e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0352e-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="0352e-112">Attributes</span></span>

<span data-ttu-id="0352e-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0352e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0352e-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0352e-114">Child elements</span></span>

<span data-ttu-id="0352e-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0352e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0352e-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0352e-116">Parent elements</span></span>

|<span data-ttu-id="0352e-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0352e-117">**Element**</span></span>|<span data-ttu-id="0352e-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="0352e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0352e-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="0352e-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="0352e-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0352e-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0352e-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0352e-121">Text value</span></span>

<span data-ttu-id="0352e-122">La valeur de texte représente une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de balise de rétention de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="0352e-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0352e-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="0352e-123">Remarks</span></span>

<span data-ttu-id="0352e-124">L’élément **EcpUrl-RET** est un élément enfant facultatif de l’élément **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="0352e-124">The **EcpUrl-ret** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0352e-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0352e-125">See also</span></span>



[<span data-ttu-id="0352e-126">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0352e-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

