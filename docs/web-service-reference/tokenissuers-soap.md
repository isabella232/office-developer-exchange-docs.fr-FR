---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Les éléments TokenIssuers représentent la collection de TokenIssuer (SOAP).
ms.openlocfilehash: 352487ad3fd9c1ee7de756a109fb98a49d0cdcd7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457073"
---
# <a name="tokenissuers-soap"></a><span data-ttu-id="ad9c0-103">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad9c0-103">TokenIssuers (SOAP)</span></span>

<span data-ttu-id="ad9c0-104">Les éléments **TokenIssuers** représentent la collection de [TokenIssuer (SOAP)](tokenissuer-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="ad9c0-104">The **TokenIssuers** elements represents the [TokenIssuer (SOAP)](tokenissuer-soap.md) collection.</span></span> 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 <span data-ttu-id="ad9c0-105">**TokenIssuers**</span><span class="sxs-lookup"><span data-stu-id="ad9c0-105">**TokenIssuers**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad9c0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ad9c0-106">Attributes and elements</span></span>

<span data-ttu-id="ad9c0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ad9c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad9c0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ad9c0-108">Attributes</span></span>

<span data-ttu-id="ad9c0-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="ad9c0-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad9c0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ad9c0-110">Child elements</span></span>

|<span data-ttu-id="ad9c0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad9c0-111">**Element**</span></span>|<span data-ttu-id="ad9c0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad9c0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad9c0-113">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad9c0-113">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="ad9c0-114">Spécifie l' [URI (SOAP)](uri-soap.md) et le [point de terminaison (SOAP)](endpoint-soap.md) pour le service d’émission de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="ad9c0-114">Specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ad9c0-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ad9c0-115">Parent elements</span></span>

|<span data-ttu-id="ad9c0-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ad9c0-116">**Element**</span></span>|<span data-ttu-id="ad9c0-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ad9c0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad9c0-118">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ad9c0-118">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="ad9c0-119">Contient la réponse [SOAP (GetFederationInformation Operation)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="ad9c0-119">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ad9c0-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="ad9c0-120">Remarks</span></span>

<span data-ttu-id="ad9c0-121">Le **TokenIssuers** représente une collection d’éléments [TokenIssuer (SOAP)](tokenissuer-soap.md) à utiliser dans le service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="ad9c0-121">The **TokenIssuers** represents a collection of [TokenIssuer (SOAP)](tokenissuer-soap.md) elements to be used in the Autodiscovery.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ad9c0-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ad9c0-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad9c0-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ad9c0-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ad9c0-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ad9c0-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ad9c0-125">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ad9c0-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ad9c0-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ad9c0-126">Validation File</span></span>  <br/> |<span data-ttu-id="ad9c0-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ad9c0-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ad9c0-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ad9c0-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad9c0-129">True</span><span class="sxs-lookup"><span data-stu-id="ad9c0-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad9c0-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ad9c0-130">See also</span></span>



[<span data-ttu-id="ad9c0-131">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ad9c0-131">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="ad9c0-132">Éléments XML de découverte automatique SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="ad9c0-132">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

