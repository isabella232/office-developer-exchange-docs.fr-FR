---
title: Point de terminaison (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 630cdbb5-d1c7-422c-924a-abf5738e9e5e
description: L’élément de point de terminaison Spécifie le point de terminaison de service d’émission de jeton de sécurité.
ms.openlocfilehash: 85e1ad785b35649238ac3944f51472addf617c20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756179"
---
# <a name="endpoint-soap"></a><span data-ttu-id="93ff5-103">Point de terminaison (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93ff5-103">Endpoint (SOAP)</span></span>

<span data-ttu-id="93ff5-104">L’élément de **point de terminaison** Spécifie le point de terminaison de service d’émission de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="93ff5-104">The **Endpoint** element specifies the security token service endpoint.</span></span> 
  
```XML
<Endpoint/>
```

 <span data-ttu-id="93ff5-105">**xs : anyURI**</span><span class="sxs-lookup"><span data-stu-id="93ff5-105">**xs:anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93ff5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="93ff5-106">Attributes and elements</span></span>

<span data-ttu-id="93ff5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="93ff5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93ff5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="93ff5-108">Attributes</span></span>

<span data-ttu-id="93ff5-109">Aucun</span><span class="sxs-lookup"><span data-stu-id="93ff5-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93ff5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="93ff5-110">Child elements</span></span>

<span data-ttu-id="93ff5-111">Aucun</span><span class="sxs-lookup"><span data-stu-id="93ff5-111">None</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93ff5-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="93ff5-112">Parent elements</span></span>

|<span data-ttu-id="93ff5-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="93ff5-113">**Element**</span></span>|<span data-ttu-id="93ff5-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="93ff5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93ff5-115">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="93ff5-115">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="93ff5-116">Spécifie l’URI et le point de terminaison pour le service d’émission de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="93ff5-116">Specifies the URI and Endpoint for the security token service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93ff5-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="93ff5-117">Text value</span></span>

<span data-ttu-id="93ff5-118">La valeur de texte représente le point de terminaison pour le service web d’émission de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="93ff5-118">The text value represents the endpoint for the security token web service.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93ff5-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="93ff5-119">Remarks</span></span>

<span data-ttu-id="93ff5-120">Le point de terminaison est utilisé pour communiquer avec le service web d’émission de jeton de sécurité.</span><span class="sxs-lookup"><span data-stu-id="93ff5-120">The endpoint is used for communicating with the security token web service.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93ff5-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="93ff5-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93ff5-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="93ff5-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="93ff5-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="93ff5-123">Schema Name</span></span>  <br/> |<span data-ttu-id="93ff5-124">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="93ff5-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="93ff5-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="93ff5-125">Validation File</span></span>  <br/> |<span data-ttu-id="93ff5-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="93ff5-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93ff5-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="93ff5-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="93ff5-128">True</span><span class="sxs-lookup"><span data-stu-id="93ff5-128">True</span></span>  <br/> |
   

