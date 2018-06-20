---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: L’élément EmwsUrl Spécifie l’URL de l’instance de point de terminaison meilleures pour Exchange Web Services (EWS) pour un utilisateur à extension messagerie.
ms.openlocfilehash: d8905d098c9978c3413f67e9a1b2443a52fb0d1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756154"
---
# <a name="emwsurl-pox"></a><span data-ttu-id="59e9d-103">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="59e9d-103">EmwsUrl (POX)</span></span>

<span data-ttu-id="59e9d-104">L’élément **EmwsUrl** Spécifie l’URL de l’instance de point de terminaison meilleures pour Exchange Web Services (EWS) pour un utilisateur à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="59e9d-104">The **EmwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
- [<span data-ttu-id="59e9d-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="59e9d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="59e9d-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="59e9d-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="59e9d-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="59e9d-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="59e9d-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="59e9d-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="59e9d-109">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="59e9d-109">EmwsUrl (POX)</span></span>](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="59e9d-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="59e9d-110">Attributes and elements</span></span>

<span data-ttu-id="59e9d-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="59e9d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59e9d-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="59e9d-112">Attributes</span></span>

<span data-ttu-id="59e9d-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59e9d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59e9d-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="59e9d-114">Child elements</span></span>

<span data-ttu-id="59e9d-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59e9d-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="59e9d-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="59e9d-116">Parent elements</span></span>

|<span data-ttu-id="59e9d-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59e9d-117">**Element**</span></span>|<span data-ttu-id="59e9d-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="59e9d-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59e9d-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="59e9d-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="59e9d-120">Contient les spécifications pour connecter un client à l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="59e9d-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="59e9d-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="59e9d-121">Text value</span></span>

<span data-ttu-id="59e9d-122">La valeur de text représente l’URL du point de terminaison EWS pour l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59e9d-122">The text value represents the URL of the EWS endpoint for the user.</span></span> <span data-ttu-id="59e9d-123">Elle est équivalente à l’élément [EwsUrl (POX)](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="59e9d-123">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="59e9d-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="59e9d-124">Remarks</span></span>

<span data-ttu-id="59e9d-125">L’élément **EmwsUrl** est un élément enfant facultatif de l’élément de **protocole** .</span><span class="sxs-lookup"><span data-stu-id="59e9d-125">The **EmwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="59e9d-126">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59e9d-126">See also</span></span>

- [<span data-ttu-id="59e9d-127">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="59e9d-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
