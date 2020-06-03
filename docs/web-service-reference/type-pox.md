---
title: Type (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: L’élément type identifie le type du compte de messagerie configuré.
ms.openlocfilehash: ad3570094ebe28498dfdc375cf7fc255434ba20d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465099"
---
# <a name="type-pox"></a><span data-ttu-id="4bca1-103">Type (POX)</span><span class="sxs-lookup"><span data-stu-id="4bca1-103">Type (POX)</span></span>

<span data-ttu-id="4bca1-104">L’élément **type** identifie le type du compte de messagerie configuré.</span><span class="sxs-lookup"><span data-stu-id="4bca1-104">The **Type** element identifies the type of the configured mail account.</span></span> 
  
[<span data-ttu-id="4bca1-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="4bca1-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="4bca1-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="4bca1-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="4bca1-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="4bca1-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="4bca1-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="4bca1-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="4bca1-109">Type (POX)</span><span class="sxs-lookup"><span data-stu-id="4bca1-109">Type (POX)</span></span>](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="4bca1-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4bca1-110">Attributes and elements</span></span>

<span data-ttu-id="4bca1-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4bca1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4bca1-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="4bca1-112">Attributes</span></span>

<span data-ttu-id="4bca1-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4bca1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4bca1-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4bca1-114">Child elements</span></span>

<span data-ttu-id="4bca1-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4bca1-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4bca1-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4bca1-116">Parent elements</span></span>

|<span data-ttu-id="4bca1-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4bca1-117">**Element**</span></span>|<span data-ttu-id="4bca1-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="4bca1-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bca1-119">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="4bca1-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="4bca1-120">Contient les spécifications relatives à la connexion d’un client au serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="4bca1-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4bca1-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4bca1-121">Text value</span></span>

<span data-ttu-id="4bca1-122">La valeur de texte représente le type de compte de messagerie.</span><span class="sxs-lookup"><span data-stu-id="4bca1-122">The text value represents the type of mail account.</span></span> <span data-ttu-id="4bca1-123">Le tableau suivant répertorie les valeurs possibles.</span><span class="sxs-lookup"><span data-stu-id="4bca1-123">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="4bca1-124">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4bca1-124">**Value**</span></span>|<span data-ttu-id="4bca1-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="4bca1-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4bca1-126">EXCH</span><span class="sxs-lookup"><span data-stu-id="4bca1-126">EXCH</span></span>  <br/> |<span data-ttu-id="4bca1-127">Le protocole utilisé pour se connecter au serveur est Exchange RPC.</span><span class="sxs-lookup"><span data-stu-id="4bca1-127">The protocol that is used to connect to the server is Exchange RPC.</span></span>  <br/> |
|<span data-ttu-id="4bca1-128">HTTP</span><span class="sxs-lookup"><span data-stu-id="4bca1-128">EXHTTP</span></span>  <br/> |<span data-ttu-id="4bca1-129">Protocole utilisé pour se connecter aux connexions RPC/HTTP du serveur.</span><span class="sxs-lookup"><span data-stu-id="4bca1-129">The protocol that is used to connect to the server RPC/HTTP connections.</span></span>  <br/> |
|<span data-ttu-id="4bca1-130">ARGUMENT</span><span class="sxs-lookup"><span data-stu-id="4bca1-130">EXPR</span></span>  <br/> |<span data-ttu-id="4bca1-131">Le protocole utilisé pour se connecter au serveur est Exchange RPC sur HTTP à l’aide d’un serveur proxy RPC.</span><span class="sxs-lookup"><span data-stu-id="4bca1-131">The protocol that is used to connect to the server is Exchange RPC over HTTP, using an RPC proxy server.</span></span>  <br/> <span data-ttu-id="4bca1-132">Ceci s’applique uniquement lorsque l’élément [AccountType (POX)](accounttype-pox.md) est défini sur courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="4bca1-132">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
|<span data-ttu-id="4bca1-133">WEB</span><span class="sxs-lookup"><span data-stu-id="4bca1-133">WEB</span></span>  <br/> |<span data-ttu-id="4bca1-134">Le courrier électronique est accessible à partir d’un navigateur Web à l’aide de l’URL spécifiée dans l’élément [serveur (POX)](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="4bca1-134">E-mail is accessed from a Web browser by using the URL that is specified in the [Server (POX)](server-pox.md) element.</span></span>  <br/> <span data-ttu-id="4bca1-135">Ceci s’applique uniquement lorsque l’élément [AccountType (POX)](accounttype-pox.md) est défini sur courrier électronique.</span><span class="sxs-lookup"><span data-stu-id="4bca1-135">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
   
### <a name="version-differences"></a><span data-ttu-id="4bca1-136">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="4bca1-136">Version differences</span></span>

<span data-ttu-id="4bca1-137">Office 365, Exchange Online et les versions locales d’Exchange commençant par Build 15.00.0995.014 renvoient la valeur « exhttp » uniquement si le serveur est configuré pour accepter les connexions RPC/HTTP et si le client inclut un en-tête [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) contenant « ExHttpInfo ».</span><span class="sxs-lookup"><span data-stu-id="4bca1-137">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "EXHTTP" only if the server is configured to accept RPC/HTTP connections and the client includes an [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "ExHttpInfo".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4bca1-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4bca1-138">See also</span></span>



[<span data-ttu-id="4bca1-139">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="4bca1-139">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

