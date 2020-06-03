---
title: EcpUrl-TM (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3f35d5ac-55be-4d3a-ad03-7d6e9349d923
description: L’élément EcpUrl-TM spécifie une URL partielle qui peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour accéder à une liste de toutes les boîtes aux lettres de site dont un utilisateur à extension messagerie est actuellement membre.
ms.openlocfilehash: 8d4c787e2eeae5300cd0496f199ea71baace98ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463544"
---
# <a name="ecpurl-tm-pox"></a><span data-ttu-id="8643a-103">EcpUrl-TM (POX)</span><span class="sxs-lookup"><span data-stu-id="8643a-103">EcpUrl-tm (POX)</span></span>

<span data-ttu-id="8643a-104">L’élément **EcpUrl-TM** spécifie une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder à une liste de toutes les boîtes aux lettres de site dont un utilisateur à extension messagerie est actuellement membre.</span><span class="sxs-lookup"><span data-stu-id="8643a-104">The **EcpUrl-tm** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of all site mailboxes of which a mail-enabled user is currently a member.</span></span> 
  
[<span data-ttu-id="8643a-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="8643a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="8643a-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="8643a-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="8643a-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="8643a-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="8643a-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="8643a-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="8643a-109">EcpUrl-TM (POX)</span><span class="sxs-lookup"><span data-stu-id="8643a-109">EcpUrl-tm (POX)</span></span>](ecpurl-tm-pox.md)
  
```XML
<EcpUrl-tm/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8643a-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8643a-110">Attributes and elements</span></span>

<span data-ttu-id="8643a-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8643a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8643a-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="8643a-112">Attributes</span></span>

<span data-ttu-id="8643a-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8643a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8643a-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8643a-114">Child elements</span></span>

<span data-ttu-id="8643a-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8643a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8643a-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8643a-116">Parent elements</span></span>

|<span data-ttu-id="8643a-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8643a-117">**Element**</span></span>|<span data-ttu-id="8643a-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="8643a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8643a-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="8643a-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8643a-120">Contient les spécifications relatives à la connexion d’un client à l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8643a-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8643a-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="8643a-121">Text value</span></span>

<span data-ttu-id="8643a-122">La valeur de texte représente une URL partielle qui peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder à une liste de boîtes aux lettres de site pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="8643a-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of site mailboxes for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8643a-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="8643a-123">Remarks</span></span>

<span data-ttu-id="8643a-124">L’élément **EcpUrl-TM** est un élément enfant facultatif de l’élément **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="8643a-124">The **EcpUrl-tm** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8643a-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8643a-125">See also</span></span>



[<span data-ttu-id="8643a-126">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="8643a-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

