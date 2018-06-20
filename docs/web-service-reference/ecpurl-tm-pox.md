---
title: EcpUrl-tm (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3f35d5ac-55be-4d3a-ad03-7d6e9349d923
description: L’élément EcpUrl-tm spécifie une URL partielle peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut servir à accéder à une liste de toutes les boîtes aux lettres de site dont un utilisateur à extension messagerie est un membre.
ms.openlocfilehash: 786459cab98f8c169f768b6ef850792e8111761a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756071"
---
# <a name="ecpurl-tm-pox"></a><span data-ttu-id="1c172-103">EcpUrl-tm (POX)</span><span class="sxs-lookup"><span data-stu-id="1c172-103">EcpUrl-tm (POX)</span></span>

<span data-ttu-id="1c172-104">L’élément **EcpUrl-tm** spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut servir à accéder à une liste de toutes les boîtes aux lettres de site dont un utilisateur à extension messagerie est un membre.</span><span class="sxs-lookup"><span data-stu-id="1c172-104">The **EcpUrl-tm** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of all site mailboxes of which a mail-enabled user is currently a member.</span></span> 
  
[<span data-ttu-id="1c172-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="1c172-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="1c172-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="1c172-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="1c172-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="1c172-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="1c172-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="1c172-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="1c172-109">EcpUrl-tm (POX)</span><span class="sxs-lookup"><span data-stu-id="1c172-109">EcpUrl-tm (POX)</span></span>](ecpurl-tm-pox.md)
  
```XML
<EcpUrl-tm/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="1c172-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1c172-110">Attributes and elements</span></span>

<span data-ttu-id="1c172-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1c172-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c172-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="1c172-112">Attributes</span></span>

<span data-ttu-id="1c172-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1c172-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c172-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1c172-114">Child elements</span></span>

<span data-ttu-id="1c172-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1c172-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1c172-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1c172-116">Parent elements</span></span>

|<span data-ttu-id="1c172-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1c172-117">**Element**</span></span>|<span data-ttu-id="1c172-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="1c172-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c172-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="1c172-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="1c172-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="1c172-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1c172-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1c172-121">Text value</span></span>

<span data-ttu-id="1c172-122">La valeur de texte représente une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder à une liste de boîtes aux lettres de site pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1c172-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access a list of site mailboxes for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1c172-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="1c172-123">Remarks</span></span>

<span data-ttu-id="1c172-124">L’élément **EcpUrl-tm** est un élément enfant facultatif de l’élément de **protocole** .</span><span class="sxs-lookup"><span data-stu-id="1c172-124">The **EcpUrl-tm** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1c172-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1c172-125">See also</span></span>



[<span data-ttu-id="1c172-126">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="1c172-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

