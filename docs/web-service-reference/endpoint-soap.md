---
title: Point de terminaison (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 630cdbb5-d1c7-422c-924a-abf5738e9e5e
description: L’élément Endpoint spécifie le point de terminaison du service d’émission de jeton de sécurité.
ms.openlocfilehash: 93659bbefa4a95063304cf3abad81cb61767070a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458396"
---
# <a name="endpoint-soap"></a><span data-ttu-id="fdb1a-103">Point de terminaison (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fdb1a-103">Endpoint (SOAP)</span></span>

<span data-ttu-id="fdb1a-104">L’élément **Endpoint** spécifie le point de terminaison du service d’émission de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="fdb1a-104">The **Endpoint** element specifies the security token service endpoint.</span></span> 
  
```XML
<Endpoint/>
```

 <span data-ttu-id="fdb1a-105">**XS : anyURI**</span><span class="sxs-lookup"><span data-stu-id="fdb1a-105">**xs:anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fdb1a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fdb1a-106">Attributes and elements</span></span>

<span data-ttu-id="fdb1a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fdb1a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fdb1a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fdb1a-108">Attributes</span></span>

<span data-ttu-id="fdb1a-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="fdb1a-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fdb1a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fdb1a-110">Child elements</span></span>

<span data-ttu-id="fdb1a-111">Aucun</span><span class="sxs-lookup"><span data-stu-id="fdb1a-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fdb1a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fdb1a-112">Parent elements</span></span>

|<span data-ttu-id="fdb1a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fdb1a-113">**Element**</span></span>|<span data-ttu-id="fdb1a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="fdb1a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fdb1a-115">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fdb1a-115">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="fdb1a-116">Spécifie l’URI et le point de terminaison pour le service d’émission de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="fdb1a-116">Specifies the URI and Endpoint for the security token service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fdb1a-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="fdb1a-117">Text value</span></span>

<span data-ttu-id="fdb1a-118">La valeur de texte représente le point de terminaison pour le service Web de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="fdb1a-118">The text value represents the endpoint for the security token web service.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fdb1a-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="fdb1a-119">Remarks</span></span>

<span data-ttu-id="fdb1a-120">Le point de terminaison est utilisé pour communiquer avec le service Web de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="fdb1a-120">The endpoint is used for communicating with the security token web service.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fdb1a-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fdb1a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fdb1a-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fdb1a-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="fdb1a-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fdb1a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="fdb1a-124">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="fdb1a-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="fdb1a-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fdb1a-125">Validation File</span></span>  <br/> |<span data-ttu-id="fdb1a-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fdb1a-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fdb1a-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fdb1a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="fdb1a-128">True</span><span class="sxs-lookup"><span data-stu-id="fdb1a-128">True</span></span>  <br/> |
   

