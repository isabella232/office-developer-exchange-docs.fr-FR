---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: L’élément TokenIssuer Spécifie l’Uri (SOAP) et le point de terminaison (SOAP) pour le service d’émission de jeton de sécurité.
ms.openlocfilehash: 1c267fc6cbfdadd471c568473cc9aeeafb43ae2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838732"
---
# <a name="tokenissuer-soap"></a><span data-ttu-id="22530-103">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22530-103">TokenIssuer (SOAP)</span></span>

<span data-ttu-id="22530-104">L’élément **TokenIssuer** Spécifie [l’Uri (SOAP)](uri-soap.md) et le [Point de terminaison (SOAP)](endpoint-soap.md) pour le service d’émission de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="22530-104">The **TokenIssuer** element specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span> 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 <span data-ttu-id="22530-105">**TokenIssuer**</span><span class="sxs-lookup"><span data-stu-id="22530-105">**TokenIssuer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22530-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="22530-106">Attributes and elements</span></span>

<span data-ttu-id="22530-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="22530-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22530-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="22530-108">Attributes</span></span>

<span data-ttu-id="22530-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="22530-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22530-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="22530-110">Child elements</span></span>

|<span data-ttu-id="22530-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22530-111">**Element**</span></span>|<span data-ttu-id="22530-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="22530-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22530-113">URI (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22530-113">Uri (SOAP)</span></span>](uri-soap.md) <br/> |<span data-ttu-id="22530-114">URI du service de jeton de sécurité qui a émis le jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="22530-114">The URI of the security token service that issued the security token.</span></span>  <br/> |
|[<span data-ttu-id="22530-115">Point de terminaison (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22530-115">Endpoint (SOAP)</span></span>](endpoint-soap.md) <br/> |<span data-ttu-id="22530-116">L’URI du point de terminaison du service web.</span><span class="sxs-lookup"><span data-stu-id="22530-116">The web service Endpoint URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22530-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="22530-117">Parent elements</span></span>

|<span data-ttu-id="22530-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22530-118">**Element**</span></span>|<span data-ttu-id="22530-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="22530-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22530-120">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22530-120">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="22530-121">Représente une collection de service d’émission de jeton de sécurité [Uri (SOAP)](uri-soap.md) et le [Point de terminaison (SOAP)](endpoint-soap.md).</span><span class="sxs-lookup"><span data-stu-id="22530-121">Represents a collection of security token service [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="22530-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="22530-122">Remarks</span></span>

<span data-ttu-id="22530-123">Utilisez l’élément **TokenIssuer** pour spécifier le service d’émission de jeton de sécurité lors de l’utilisation de jetons de sécurité.</span><span class="sxs-lookup"><span data-stu-id="22530-123">Use the **TokenIssuer** element to specify the security token service when using security tokens.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="22530-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="22530-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22530-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="22530-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="22530-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="22530-126">Schema Name</span></span>  <br/> |<span data-ttu-id="22530-127">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="22530-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="22530-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="22530-128">Validation File</span></span>  <br/> |<span data-ttu-id="22530-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="22530-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="22530-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="22530-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="22530-131">True</span><span class="sxs-lookup"><span data-stu-id="22530-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22530-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="22530-132">See also</span></span>



[<span data-ttu-id="22530-133">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="22530-133">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="22530-134">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="22530-134">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

