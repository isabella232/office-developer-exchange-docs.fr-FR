---
title: Demande de découverte automatique POX pour Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: La demande de découverte automatique contient une requête pour la configuration d’accès client d’un utilisateur.
ms.openlocfilehash: b2138f9813c7b75aef9afb90089b9b874aac7532
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461666"
---
# <a name="pox-autodiscover-request-for-exchange"></a><span data-ttu-id="decb3-103">Demande de découverte automatique POX pour Exchange</span><span class="sxs-lookup"><span data-stu-id="decb3-103">POX Autodiscover request for Exchange</span></span>

<span data-ttu-id="decb3-104">La demande de découverte automatique contient une requête pour la configuration d’accès client d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="decb3-104">The Autodiscover request contains a query for a user's client access configuration.</span></span>
  
## <a name="autodiscover-request-example"></a><span data-ttu-id="decb3-105">Exemple de requête de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="decb3-105">Autodiscover request example</span></span>

### <a name="description"></a><span data-ttu-id="decb3-106">Description</span><span class="sxs-lookup"><span data-stu-id="decb3-106">Description</span></span>

<span data-ttu-id="decb3-107">L’exemple de code XML suivant montre un corps de demande de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="decb3-107">The following XML example shows an Autodiscover request body.</span></span>
  
### <a name="code"></a><span data-ttu-id="decb3-108">Code</span><span class="sxs-lookup"><span data-stu-id="decb3-108">Code</span></span>

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a><span data-ttu-id="decb3-109">En-têtes de demande</span><span class="sxs-lookup"><span data-stu-id="decb3-109">Request Headers</span></span>

<span data-ttu-id="decb3-110">Les en-têtes HTTP suivants sont facultatifs lors de l’envoi de demandes de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="decb3-110">The following HTTP headers are optional when sending Autodiscover requests.</span></span>
  
<span data-ttu-id="decb3-111">**Tableau 1. En-têtes de requête HTTP**</span><span class="sxs-lookup"><span data-stu-id="decb3-111">**Table 1. HTTP request headers**</span></span>

|<span data-ttu-id="decb3-112">**Header**</span><span class="sxs-lookup"><span data-stu-id="decb3-112">**Header**</span></span>|<span data-ttu-id="decb3-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="decb3-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="decb3-114">X-MapiHttpCapability</span><span class="sxs-lookup"><span data-stu-id="decb3-114">X-MapiHttpCapability</span></span>  <br/> |<span data-ttu-id="decb3-115">Si présent et défini sur « 1 », indique que le client demande des informations qui peuvent être utilisées pour se connecter au serveur à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="decb3-115">If present and set to "1", indicates that the client is requesting information that can be used to connect to the server by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="decb3-116">Cet en-tête s’applique aux clients qui implémentent le protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="decb3-116">This header is applicable to clients that implement the MAPI/HTTP protocol.</span></span>  <br/> |
|<span data-ttu-id="decb3-117">X-ClientCanHandle</span><span class="sxs-lookup"><span data-stu-id="decb3-117">X-ClientCanHandle</span></span>  <br/> |<span data-ttu-id="decb3-118">Cet en-tête contient une liste délimitée par des virgules des fonctionnalités prises en charge par le client.</span><span class="sxs-lookup"><span data-stu-id="decb3-118">This header contains a comma-delimited list of capabilities that the client supports.</span></span> <span data-ttu-id="decb3-119">Les valeurs possibles sont spécifiées dans le tableau 2.</span><span class="sxs-lookup"><span data-stu-id="decb3-119">The possible values are specified in Table 2.</span></span>  <br/> |
   
<span data-ttu-id="decb3-120">**Tableau 2. Valeurs d’en-tête X-ClientCanHandle**</span><span class="sxs-lookup"><span data-stu-id="decb3-120">**Table 2. X-ClientCanHandle header values**</span></span>

|<span data-ttu-id="decb3-121">**Valeur X-ClientCanHandle (ne respectant pas la casse)**</span><span class="sxs-lookup"><span data-stu-id="decb3-121">**X-ClientCanHandle value (case-insensitive)**</span></span>|<span data-ttu-id="decb3-122">**Version de serveur minimale**</span><span class="sxs-lookup"><span data-stu-id="decb3-122">**Minimum server version**</span></span>|<span data-ttu-id="decb3-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="decb3-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="decb3-124">Poursuivre</span><span class="sxs-lookup"><span data-stu-id="decb3-124">Negotiate</span></span>  <br/> |<span data-ttu-id="decb3-125">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="decb3-125">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="decb3-126">Si cette valeur est présente, le serveur renvoie la valeur « Negotiate » dans l’élément [package (POX)](authpackage-pox.md) si le serveur est configuré pour accepter l’authentification par négociation.</span><span class="sxs-lookup"><span data-stu-id="decb3-126">If this value is present, the server will return a value of "Negotiate" in the [AuthPackage (POX)](authpackage-pox.md) element if the server is configured to accept Negotiate authentication.</span></span> <span data-ttu-id="decb3-127">Si cette valeur n’est pas présente, le serveur ne renvoie pas la valeur « Negotiate » dans l’élément **package** .</span><span class="sxs-lookup"><span data-stu-id="decb3-127">If this value is not present, the server will not return a value of "Negotiate" in the **AuthPackage** element.</span></span>  <br/> |
|<span data-ttu-id="decb3-128">ExHttpInfo</span><span class="sxs-lookup"><span data-stu-id="decb3-128">ExHttpInfo</span></span>  <br/> |<span data-ttu-id="decb3-129">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="decb3-129">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="decb3-130">Si cette valeur est présente, le serveur renvoie un élément [Protocol (POX)](protocol-pox.md) avec un élément [type (POX)](type-pox.md) défini sur « exhttp » si le serveur est configuré pour accepter les connexions RPC/HTTP.</span><span class="sxs-lookup"><span data-stu-id="decb3-130">If this value is present, the server will return a [Protocol (POX)](protocol-pox.md) element with a [Type (POX)](type-pox.md) element set to "EXHTTP" if the server is configured to accept RPC/HTTP connections.</span></span> <span data-ttu-id="decb3-131">Si cette valeur n’est pas présente, le serveur ne renvoie pas un élément de **protocole** dont l’élément **type** est défini sur « exhttp ».</span><span class="sxs-lookup"><span data-stu-id="decb3-131">If this value is not present, the server will not return a **Protocol** element with a **Type** element set to "EXHTTP".</span></span>  <br/> |
   
### <a name="request-elements"></a><span data-ttu-id="decb3-132">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="decb3-132">Request elements</span></span>

<span data-ttu-id="decb3-133">Les éléments suivants sont utilisés dans le corps de la demande :</span><span class="sxs-lookup"><span data-stu-id="decb3-133">The following elements are used in the request body:</span></span>
  
- [<span data-ttu-id="decb3-134">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="decb3-134">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="decb3-135">Demande (POX)</span><span class="sxs-lookup"><span data-stu-id="decb3-135">Request (POX)</span></span>](request-pox.md)
    
- [<span data-ttu-id="decb3-136">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="decb3-136">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md)
    
- [<span data-ttu-id="decb3-137">EMailAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="decb3-137">EMailAddress (POX)</span></span>](emailaddress-pox.md)
    
> [!NOTE]
> <span data-ttu-id="decb3-138">L’élément [LegacyDN (POX)](legacydn-pox.md) peut être utilisé à la place de l’élément [EMailAddress (POX)](emailaddress-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="decb3-138">The [LegacyDN (POX)](legacydn-pox.md) element can be used in place of the [EMailAddress (POX)](emailaddress-pox.md) element.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="decb3-139">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="decb3-139">Version differences</span></span>

<span data-ttu-id="decb3-140">L’en-tête X-MapiHttpCapability est disponible dans Office 365, Exchange Online et les versions locales d’Exchange à partir de la version 15.00.0847.032 (Exchange Server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="decb3-140">The X-MapiHttpCapability header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>
  
<span data-ttu-id="decb3-141">L’en-tête X-ClientCanHandle est disponible dans Office 365, Exchange Online et les versions locales d’Exchange à partir de la version 15.00.0995.014.</span><span class="sxs-lookup"><span data-stu-id="decb3-141">The X-ClientCanHandle header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="decb3-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="decb3-142">See also</span></span>



[<span data-ttu-id="decb3-143">Réponse de découverte automatique POX pour Exchange</span><span class="sxs-lookup"><span data-stu-id="decb3-143">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)


[<span data-ttu-id="decb3-144">Référence du service Web de découverte automatique POX pour Exchange</span><span class="sxs-lookup"><span data-stu-id="decb3-144">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="decb3-145">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="decb3-145">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

