---
title: EwsPartnerUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: L’élément EwsPartnerUrl Spécifie l’URL de l’instance de point de terminaison meilleures pour Exchange Web Services (EWS) pour un utilisateur à extension messagerie.
ms.openlocfilehash: 97c33e1fed4adc8a9e8542d85e67c942118f6096
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756240"
---
# <a name="ewspartnerurl-pox"></a><span data-ttu-id="3594f-103">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="3594f-103">EwsPartnerUrl (POX)</span></span>

<span data-ttu-id="3594f-104">L’élément **EwsPartnerUrl** Spécifie l’URL de l’instance de point de terminaison meilleures pour Exchange Web Services (EWS) pour un utilisateur à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="3594f-104">The **EwsPartnerUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="3594f-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="3594f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="3594f-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="3594f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="3594f-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="3594f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="3594f-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="3594f-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="3594f-109">EwsPartnerUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="3594f-109">EwsPartnerUrl (POX)</span></span>](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="3594f-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3594f-110">Attributes and elements</span></span>

<span data-ttu-id="3594f-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3594f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3594f-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="3594f-112">Attributes</span></span>

<span data-ttu-id="3594f-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3594f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3594f-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3594f-114">Child elements</span></span>

<span data-ttu-id="3594f-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3594f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3594f-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3594f-116">Parent elements</span></span>

|<span data-ttu-id="3594f-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3594f-117">**Element**</span></span>|<span data-ttu-id="3594f-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="3594f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3594f-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="3594f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="3594f-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="3594f-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3594f-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3594f-121">Text value</span></span>

<span data-ttu-id="3594f-122">La valeur de text représente l’URL du point de terminaison EWS pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="3594f-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3594f-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="3594f-123">Remarks</span></span>

<span data-ttu-id="3594f-124">L’élément **EwsPartnerUrl** est un élément enfant facultatif de l’élément de **protocole** .</span><span class="sxs-lookup"><span data-stu-id="3594f-124">The **EwsPartnerUrl** element is an optional child element of the **Protocol** element.</span></span> <span data-ttu-id="3594f-125">Elle est équivalente à l’élément [EwsUrl (POX)](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="3594f-125">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="3594f-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3594f-126">See also</span></span>



[<span data-ttu-id="3594f-127">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="3594f-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

