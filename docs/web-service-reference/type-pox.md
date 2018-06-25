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
description: L’élément Type identifie le type du compte de messagerie configuré.
ms.openlocfilehash: 6e1349769c6a5349304f576419e0c609d3edd9a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838783"
---
# <a name="type-pox"></a><span data-ttu-id="d3d2f-103">Type (POX)</span><span class="sxs-lookup"><span data-stu-id="d3d2f-103">Type (POX)</span></span>

<span data-ttu-id="d3d2f-104">L’élément **Type** identifie le type du compte de messagerie configuré.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-104">The **Type** element identifies the type of the configured mail account.</span></span> 
  
[<span data-ttu-id="d3d2f-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="d3d2f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d3d2f-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="d3d2f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d3d2f-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="d3d2f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d3d2f-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="d3d2f-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="d3d2f-109">Type (POX)</span><span class="sxs-lookup"><span data-stu-id="d3d2f-109">Type (POX)</span></span>](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d3d2f-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d3d2f-110">Attributes and elements</span></span>

<span data-ttu-id="d3d2f-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3d2f-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="d3d2f-112">Attributes</span></span>

<span data-ttu-id="d3d2f-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3d2f-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d3d2f-114">Child elements</span></span>

<span data-ttu-id="d3d2f-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d3d2f-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d3d2f-116">Parent elements</span></span>

|<span data-ttu-id="d3d2f-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3d2f-117">**Element**</span></span>|<span data-ttu-id="d3d2f-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3d2f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3d2f-119">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="d3d2f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="d3d2f-120">Contient les spécifications pour la connexion d’un client sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3d2f-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d3d2f-121">Text value</span></span>

<span data-ttu-id="d3d2f-122">La valeur de texte représente le type de compte de messagerie.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-122">The text value represents the type of mail account.</span></span> <span data-ttu-id="d3d2f-123">Le tableau suivant répertorie les valeurs possibles.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-123">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="d3d2f-124">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="d3d2f-124">**Value**</span></span>|<span data-ttu-id="d3d2f-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3d2f-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d3d2f-126">EXCH</span><span class="sxs-lookup"><span data-stu-id="d3d2f-126">EXCH</span></span>  <br/> |<span data-ttu-id="d3d2f-127">Le protocole utilisé pour se connecter au serveur est RPC Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-127">The protocol that is used to connect to the server is Exchange RPC.</span></span>  <br/> |
|<span data-ttu-id="d3d2f-128">EXHTTP</span><span class="sxs-lookup"><span data-stu-id="d3d2f-128">EXHTTP</span></span>  <br/> |<span data-ttu-id="d3d2f-129">Le protocole utilisé pour se connecter aux connexions RPC/HTTP server.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-129">The protocol that is used to connect to the server RPC/HTTP connections.</span></span>  <br/> |
|<span data-ttu-id="d3d2f-130">EXPR</span><span class="sxs-lookup"><span data-stu-id="d3d2f-130">EXPR</span></span>  <br/> |<span data-ttu-id="d3d2f-131">Le protocole utilisé pour se connecter au serveur est Exchange RPC sur HTTP, à l’aide d’un serveur proxy RPC.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-131">The protocol that is used to connect to the server is Exchange RPC over HTTP, using an RPC proxy server.</span></span>  <br/> <span data-ttu-id="d3d2f-132">Cela s’applique uniquement lorsque l’élément [AccountType (POX)](accounttype-pox.md) est définie pour les courriers électroniques.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-132">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
|<span data-ttu-id="d3d2f-133">WEB</span><span class="sxs-lookup"><span data-stu-id="d3d2f-133">WEB</span></span>  <br/> |<span data-ttu-id="d3d2f-134">Courrier électronique est accessible à partir d’un navigateur Web à l’aide de l’URL qui est spécifié dans l’élément [Serveur (POX)](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="d3d2f-134">E-mail is accessed from a Web browser by using the URL that is specified in the [Server (POX)](server-pox.md) element.</span></span>  <br/> <span data-ttu-id="d3d2f-135">Cela s’applique uniquement lorsque l’élément [AccountType (POX)](accounttype-pox.md) est définie pour les courriers électroniques.</span><span class="sxs-lookup"><span data-stu-id="d3d2f-135">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
   
### <a name="version-differences"></a><span data-ttu-id="d3d2f-136">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="d3d2f-136">Version differences</span></span>

<span data-ttu-id="d3d2f-137">Office 365, Exchange Online et les versions locales d’Exchange commençant par créer 15.00.0995.014 retour une valeur de « EXHTTP » uniquement si le serveur est configuré pour accepter les connexions RPC/HTTP et le client inclut un en-tête [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) qui contient « ExHttpInfo ».</span><span class="sxs-lookup"><span data-stu-id="d3d2f-137">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "EXHTTP" only if the server is configured to accept RPC/HTTP connections and the client includes an [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "ExHttpInfo".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d3d2f-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d3d2f-138">See also</span></span>



[<span data-ttu-id="d3d2f-139">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d3d2f-139">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

