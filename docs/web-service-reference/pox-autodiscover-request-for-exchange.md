---
title: Demande de découverte automatique variole pour Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: La demande de découverte automatique contient une requête pour la configuration de l’accès client d’un utilisateur.
ms.openlocfilehash: 48d6c30946e75936ed93a6f4507d8a8d3ae47d40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828865"
---
# <a name="pox-autodiscover-request-for-exchange"></a><span data-ttu-id="d924c-103">Demande de découverte automatique variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d924c-103">POX Autodiscover request for Exchange</span></span>

<span data-ttu-id="d924c-104">La demande de découverte automatique contient une requête pour la configuration de l’accès client d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d924c-104">The Autodiscover request contains a query for a user's client access configuration.</span></span>
  
## <a name="autodiscover-request-example"></a><span data-ttu-id="d924c-105">Exemple de requête de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="d924c-105">Autodiscover request example</span></span>

### <a name="description"></a><span data-ttu-id="d924c-106">Description</span><span class="sxs-lookup"><span data-stu-id="d924c-106">Description</span></span>

<span data-ttu-id="d924c-107">L’exemple XML suivant montre un corps de demande de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="d924c-107">The following XML example shows an Autodiscover request body.</span></span>
  
### <a name="code"></a><span data-ttu-id="d924c-108">Code</span><span class="sxs-lookup"><span data-stu-id="d924c-108">Code</span></span>

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a><span data-ttu-id="d924c-109">En-têtes de demande</span><span class="sxs-lookup"><span data-stu-id="d924c-109">Request Headers</span></span>

<span data-ttu-id="d924c-110">Les en-têtes HTTP suivants sont facultatifs lors de l’envoi de demandes de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="d924c-110">The following HTTP headers are optional when sending Autodiscover requests.</span></span>
  
<span data-ttu-id="d924c-111">**Le tableau 1. En-têtes de demande HTTP**</span><span class="sxs-lookup"><span data-stu-id="d924c-111">**Table 1. HTTP request headers**</span></span>

|<span data-ttu-id="d924c-112">**Header**</span><span class="sxs-lookup"><span data-stu-id="d924c-112">**Header**</span></span>|<span data-ttu-id="d924c-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="d924c-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d924c-114">X-MapiHttpCapability</span><span class="sxs-lookup"><span data-stu-id="d924c-114">X-MapiHttpCapability</span></span>  <br/> |<span data-ttu-id="d924c-115">Si présente et définie sur « 1 », indique que le client demande des informations qui peuvent être utilisées pour se connecter au serveur à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="d924c-115">If present and set to "1", indicates that the client is requesting information that can be used to connect to the server by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="d924c-116">Cet en-tête est applicable aux clients qui implémentent le protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="d924c-116">This header is applicable to clients that implement the MAPI/HTTP protocol.</span></span>  <br/> |
|<span data-ttu-id="d924c-117">X-ClientCanHandle</span><span class="sxs-lookup"><span data-stu-id="d924c-117">X-ClientCanHandle</span></span>  <br/> |<span data-ttu-id="d924c-118">Cet en-tête contient une liste délimitée par des fonctions prises en charge par le client.</span><span class="sxs-lookup"><span data-stu-id="d924c-118">This header contains a comma-delimited list of capabilities that the client supports.</span></span> <span data-ttu-id="d924c-119">Les valeurs possibles sont spécifiés dans le tableau 2.</span><span class="sxs-lookup"><span data-stu-id="d924c-119">The possible values are specified in Table 2.</span></span>  <br/> |
   
<span data-ttu-id="d924c-120">**Le tableau 2. Valeurs d’en-tête X-ClientCanHandle**</span><span class="sxs-lookup"><span data-stu-id="d924c-120">**Table 2. X-ClientCanHandle header values**</span></span>

|<span data-ttu-id="d924c-121">**Valeur X-ClientCanHandle (pas la casse)**</span><span class="sxs-lookup"><span data-stu-id="d924c-121">**X-ClientCanHandle value (case-insensitive)**</span></span>|<span data-ttu-id="d924c-122">**Version minimale du serveur**</span><span class="sxs-lookup"><span data-stu-id="d924c-122">**Minimum server version**</span></span>|<span data-ttu-id="d924c-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="d924c-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d924c-124">Négocier</span><span class="sxs-lookup"><span data-stu-id="d924c-124">Negotiate</span></span>  <br/> |<span data-ttu-id="d924c-125">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="d924c-125">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="d924c-126">Si cette valeur est présente, le serveur renvoie une valeur « Negotiate » dans l’élément [AuthPackage (POX)](authpackage-pox.md) si le serveur est configuré pour accepter l’authentification par négociation.</span><span class="sxs-lookup"><span data-stu-id="d924c-126">If this value is present, the server will return a value of "Negotiate" in the [AuthPackage (POX)](authpackage-pox.md) element if the server is configured to accept Negotiate authentication.</span></span> <span data-ttu-id="d924c-127">Si cette valeur n’est pas présente, le serveur ne sera pas renvoie une valeur de « Négocier » dans l’élément **AuthPackage** .</span><span class="sxs-lookup"><span data-stu-id="d924c-127">If this value is not present, the server will not return a value of "Negotiate" in the **AuthPackage** element.</span></span>  <br/> |
|<span data-ttu-id="d924c-128">ExHttpInfo</span><span class="sxs-lookup"><span data-stu-id="d924c-128">ExHttpInfo</span></span>  <br/> |<span data-ttu-id="d924c-129">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="d924c-129">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="d924c-130">Si cette valeur est présente, le serveur renvoie un élément de [Protocole (POX)](protocol-pox.md) avec un élément de [Type (POX)](type-pox.md) la valeur « EXHTTP » si le serveur est configuré pour accepter les connexions RPC/HTTP.</span><span class="sxs-lookup"><span data-stu-id="d924c-130">If this value is present, the server will return a [Protocol (POX)](protocol-pox.md) element with a [Type (POX)](type-pox.md) element set to "EXHTTP" if the server is configured to accept RPC/HTTP connections.</span></span> <span data-ttu-id="d924c-131">Si cette valeur n’est pas présente, le serveur renvoie pas un élément de **protocole** avec un élément de **Type** défini sur « EXHTTP ».</span><span class="sxs-lookup"><span data-stu-id="d924c-131">If this value is not present, the server will not return a **Protocol** element with a **Type** element set to "EXHTTP".</span></span>  <br/> |
   
### <a name="request-elements"></a><span data-ttu-id="d924c-132">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="d924c-132">Request elements</span></span>

<span data-ttu-id="d924c-133">Les éléments suivants sont utilisés dans le corps de la demande :</span><span class="sxs-lookup"><span data-stu-id="d924c-133">The following elements are used in the request body:</span></span>
  
- [<span data-ttu-id="d924c-134">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="d924c-134">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="d924c-135">Demande (POX)</span><span class="sxs-lookup"><span data-stu-id="d924c-135">Request (POX)</span></span>](request-pox.md)
    
- [<span data-ttu-id="d924c-136">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="d924c-136">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md)
    
- [<span data-ttu-id="d924c-137">EMailAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="d924c-137">EMailAddress (POX)</span></span>](emailaddress-pox.md)
    
> [!NOTE]
> <span data-ttu-id="d924c-138">L’élément [LegacyDN (POX)](legacydn-pox.md) peut être utilisé à la place de l’élément [EMailAddress (POX)](emailaddress-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="d924c-138">The [LegacyDN (POX)](legacydn-pox.md) element can be used in place of the [EMailAddress (POX)](emailaddress-pox.md) element.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="d924c-139">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="d924c-139">Version differences</span></span>

<span data-ttu-id="d924c-140">L’en-tête X-MapiHttpCapability est disponible dans Office 365, Exchange Online et créer des versions d’Exchange commençant par 15.00.0847.032 (Exchange Server 2013 SP1) sur site.</span><span class="sxs-lookup"><span data-stu-id="d924c-140">The X-MapiHttpCapability header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>
  
<span data-ttu-id="d924c-141">L’en-tête X-ClientCanHandle est disponible dans Office 365, Exchange Online et créer des versions d’Exchange commençant par 15.00.0995.014 local.</span><span class="sxs-lookup"><span data-stu-id="d924c-141">The X-ClientCanHandle header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d924c-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d924c-142">See also</span></span>



[<span data-ttu-id="d924c-143">Réponse de découverte automatique variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d924c-143">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)


[<span data-ttu-id="d924c-144">Référence de service web variole découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d924c-144">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="d924c-145">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d924c-145">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

