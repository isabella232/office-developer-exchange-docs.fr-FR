---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Les éléments TokenIssuers représente la collection TokenIssuer (SOAP).
ms.openlocfilehash: b070d85b32d5bce8461ac4e930329f237885bad7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838744"
---
# <a name="tokenissuers-soap"></a><span data-ttu-id="9c9cc-103">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9c9cc-103">TokenIssuers (SOAP)</span></span>

<span data-ttu-id="9c9cc-104">Les éléments **TokenIssuers** représente la collection [TokenIssuer (SOAP)](tokenissuer-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="9c9cc-104">The **TokenIssuers** elements represents the [TokenIssuer (SOAP)](tokenissuer-soap.md) collection.</span></span> 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 <span data-ttu-id="9c9cc-105">**TokenIssuers**</span><span class="sxs-lookup"><span data-stu-id="9c9cc-105">**TokenIssuers**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c9cc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9c9cc-106">Attributes and elements</span></span>

<span data-ttu-id="9c9cc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9c9cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c9cc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9c9cc-108">Attributes</span></span>

<span data-ttu-id="9c9cc-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="9c9cc-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c9cc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9c9cc-110">Child elements</span></span>

|<span data-ttu-id="9c9cc-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9c9cc-111">**Element**</span></span>|<span data-ttu-id="9c9cc-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="9c9cc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c9cc-113">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9c9cc-113">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="9c9cc-114">Spécifie [l’Uri (SOAP)](uri-soap.md) et le [Point de terminaison (SOAP)](endpoint-soap.md) pour le service d’émission de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="9c9cc-114">Specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9c9cc-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9c9cc-115">Parent elements</span></span>

|<span data-ttu-id="9c9cc-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9c9cc-116">**Element**</span></span>|<span data-ttu-id="9c9cc-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="9c9cc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c9cc-118">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9c9cc-118">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="9c9cc-119">Contient la réponse de [l’opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="9c9cc-119">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9c9cc-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="9c9cc-120">Remarks</span></span>

<span data-ttu-id="9c9cc-121">La **TokenIssuers** représente une collection d’éléments [TokenIssuer (SOAP)](tokenissuer-soap.md) à utiliser dans la découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="9c9cc-121">The **TokenIssuers** represents a collection of [TokenIssuer (SOAP)](tokenissuer-soap.md) elements to be used in the Autodiscovery.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9c9cc-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9c9cc-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c9cc-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9c9cc-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9c9cc-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9c9cc-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9c9cc-125">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="9c9cc-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9c9cc-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9c9cc-126">Validation File</span></span>  <br/> |<span data-ttu-id="9c9cc-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9c9cc-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9c9cc-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9c9cc-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="9c9cc-129">True</span><span class="sxs-lookup"><span data-stu-id="9c9cc-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9c9cc-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9c9cc-130">See also</span></span>



[<span data-ttu-id="9c9cc-131">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="9c9cc-131">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="9c9cc-132">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9c9cc-132">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

