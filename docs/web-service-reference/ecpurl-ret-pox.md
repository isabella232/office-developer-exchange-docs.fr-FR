---
title: EcpUrl-ret (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5f090fd2-b0c4-4ca0-a959-1433d73a2069
description: L’élément EcpUrl-ret spécifie une URL partielle peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour accéder aux paramètres de balises de rétention pour un utilisateur à extension messagerie.
ms.openlocfilehash: 366a7a79c0f3c19b2cfef21c01826e62b0e95793
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756075"
---
# <a name="ecpurl-ret-pox"></a><span data-ttu-id="420d8-103">EcpUrl-ret (POX)</span><span class="sxs-lookup"><span data-stu-id="420d8-103">EcpUrl-ret (POX)</span></span>

<span data-ttu-id="420d8-104">L’élément **EcpUrl-ret** spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de balises de rétention pour un utilisateur à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="420d8-104">The **EcpUrl-ret** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="420d8-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="420d8-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="420d8-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="420d8-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="420d8-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="420d8-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="420d8-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="420d8-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="420d8-109">EcpUrl-ret (POX)</span><span class="sxs-lookup"><span data-stu-id="420d8-109">EcpUrl-ret (POX)</span></span>](ecpurl-ret-pox.md)
  
```XML
<EcpUrl-ret/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="420d8-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="420d8-110">Attributes and elements</span></span>

<span data-ttu-id="420d8-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="420d8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="420d8-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="420d8-112">Attributes</span></span>

<span data-ttu-id="420d8-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="420d8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="420d8-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="420d8-114">Child elements</span></span>

<span data-ttu-id="420d8-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="420d8-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="420d8-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="420d8-116">Parent elements</span></span>

|<span data-ttu-id="420d8-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="420d8-117">**Element**</span></span>|<span data-ttu-id="420d8-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="420d8-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="420d8-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="420d8-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="420d8-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="420d8-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="420d8-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="420d8-121">Text value</span></span>

<span data-ttu-id="420d8-122">La valeur de texte représente une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de balises de rétention pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="420d8-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access retention tag settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="420d8-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="420d8-123">Remarks</span></span>

<span data-ttu-id="420d8-124">L’élément **EcpUrl-ret** est un élément enfant facultatif de l’élément de **protocole** .</span><span class="sxs-lookup"><span data-stu-id="420d8-124">The **EcpUrl-ret** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="420d8-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="420d8-125">See also</span></span>



[<span data-ttu-id="420d8-126">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="420d8-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

