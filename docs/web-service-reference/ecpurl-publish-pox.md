---
title: Publication EcpUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a51189db-f6e5-428d-833d-65a209204a5b
description: L’élément de publication EcpUrl spécifie une URL partielle peut être combinée avec la valeur de l’élément EcpUrl (POX) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’un utilisateur à extension messagerie de publication de calendrier.
ms.openlocfilehash: 82f55be3ce529f6e57db5ffe18bbdea609b13595
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756069"
---
# <a name="ecpurl-publish-pox"></a><span data-ttu-id="ea449-103">Publication EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="ea449-103">EcpUrl-publish (POX)</span></span>

<span data-ttu-id="ea449-104">L’élément **de publication EcpUrl** spécifie une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres d’un utilisateur à extension messagerie de publication de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ea449-104">The **EcpUrl-publish** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access calendar publishing settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="ea449-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="ea449-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="ea449-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="ea449-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="ea449-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="ea449-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="ea449-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="ea449-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="ea449-109">Publication EcpUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="ea449-109">EcpUrl-publish (POX)</span></span>](ecpurl-publish-pox.md)
  
```XML
<EcpUrl-publish/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="ea449-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ea449-110">Attributes and elements</span></span>

<span data-ttu-id="ea449-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ea449-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea449-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="ea449-112">Attributes</span></span>

<span data-ttu-id="ea449-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ea449-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea449-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ea449-114">Child elements</span></span>

<span data-ttu-id="ea449-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ea449-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ea449-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ea449-116">Parent elements</span></span>

|<span data-ttu-id="ea449-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ea449-117">**Element**</span></span>|<span data-ttu-id="ea449-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="ea449-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea449-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="ea449-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="ea449-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="ea449-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ea449-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ea449-121">Text value</span></span>

<span data-ttu-id="ea449-122">La valeur de texte représente une URL partielle peut être combinée avec la valeur de l’élément [EcpUrl (POX)](ecpurl-pox.md) pour générer une URL qui peut être utilisée pour accéder aux paramètres de publication de calendrier pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ea449-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access calendar publishing settings for the user.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ea449-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="ea449-123">Remarks</span></span>

<span data-ttu-id="ea449-124">L’élément **de publication EcpUrl** est un élément enfant facultatif de l’élément de **protocole** .</span><span class="sxs-lookup"><span data-stu-id="ea449-124">The **EcpUrl-publish** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ea449-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ea449-125">See also</span></span>



[<span data-ttu-id="ea449-126">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ea449-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

