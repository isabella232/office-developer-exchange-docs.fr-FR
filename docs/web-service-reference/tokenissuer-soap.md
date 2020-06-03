---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: L’élément TokenIssuer spécifie l’URI (SOAP) et le point de terminaison (SOAP) pour le service d’émission de jeton de sécurité.
ms.openlocfilehash: e9c0b4140de26c7ff05daf4e863b3e8a17fedc62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526325"
---
# <a name="tokenissuer-soap"></a><span data-ttu-id="d010a-103">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d010a-103">TokenIssuer (SOAP)</span></span>

<span data-ttu-id="d010a-104">L’élément **TokenIssuer** spécifie l' [URI (SOAP)](uri-soap.md) et le [point de terminaison (SOAP)](endpoint-soap.md) pour le service d’émission de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="d010a-104">The **TokenIssuer** element specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span> 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 <span data-ttu-id="d010a-105">**TokenIssuer**</span><span class="sxs-lookup"><span data-stu-id="d010a-105">**TokenIssuer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d010a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d010a-106">Attributes and elements</span></span>

<span data-ttu-id="d010a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d010a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d010a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d010a-108">Attributes</span></span>

<span data-ttu-id="d010a-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="d010a-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d010a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d010a-110">Child elements</span></span>

|<span data-ttu-id="d010a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d010a-111">**Element**</span></span>|<span data-ttu-id="d010a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d010a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d010a-113">URI (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d010a-113">Uri (SOAP)</span></span>](uri-soap.md) <br/> |<span data-ttu-id="d010a-114">URI du service d’émission de jeton de sécurité qui a émis le jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="d010a-114">The URI of the security token service that issued the security token.</span></span>  <br/> |
|[<span data-ttu-id="d010a-115">Point de terminaison (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d010a-115">Endpoint (SOAP)</span></span>](endpoint-soap.md) <br/> |<span data-ttu-id="d010a-116">URI du point de terminaison du service Web.</span><span class="sxs-lookup"><span data-stu-id="d010a-116">The web service Endpoint URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d010a-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d010a-117">Parent elements</span></span>

|<span data-ttu-id="d010a-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d010a-118">**Element**</span></span>|<span data-ttu-id="d010a-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="d010a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d010a-120">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d010a-120">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="d010a-121">Représente une collection de [protocole SOAP (](uri-soap.md) Security Token Service URI) et de [point de terminaison (SOAP)](endpoint-soap.md).</span><span class="sxs-lookup"><span data-stu-id="d010a-121">Represents a collection of security token service [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d010a-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="d010a-122">Remarks</span></span>

<span data-ttu-id="d010a-123">Utilisez l’élément **TokenIssuer** pour spécifier le service d’émission de jeton de sécurité lors de l’utilisation de jetons de sécurité.</span><span class="sxs-lookup"><span data-stu-id="d010a-123">Use the **TokenIssuer** element to specify the security token service when using security tokens.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d010a-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d010a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d010a-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d010a-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d010a-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d010a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d010a-127">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="d010a-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d010a-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d010a-128">Validation File</span></span>  <br/> |<span data-ttu-id="d010a-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d010a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d010a-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d010a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d010a-131">True</span><span class="sxs-lookup"><span data-stu-id="d010a-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d010a-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d010a-132">See also</span></span>



[<span data-ttu-id="d010a-133">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="d010a-133">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="d010a-134">Éléments XML de découverte automatique SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="d010a-134">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

