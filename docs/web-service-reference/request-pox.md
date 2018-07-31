---
title: Request (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: L’élément de demande contient la demande au service de découverte automatique.
ms.openlocfilehash: 3f5d5258a92840fe79c4936370323b78aa4715b3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354427"
---
# <a name="request-pox"></a><span data-ttu-id="59c6c-103">Request (POX)</span><span class="sxs-lookup"><span data-stu-id="59c6c-103">Request (POX)</span></span>

<span data-ttu-id="59c6c-104">L’élément de **demande** contient la demande au service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="59c6c-104">The **Request** element contains the request to the Autodiscover service.</span></span> 
  
- [<span data-ttu-id="59c6c-105">AutoDiscover (POX)</span><span class="sxs-lookup"><span data-stu-id="59c6c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="59c6c-106">Request (POX)</span><span class="sxs-lookup"><span data-stu-id="59c6c-106">Request (POX)</span></span>](request-pox.md)
  
```xml
<Request>
   <AcceptableResponseSchema/>
   <EMailAddress/>
</Request>
```

```xml
<Request>
   <AcceptableResponseSchema/> 
   <LegacyDN/>
</Request>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="59c6c-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="59c6c-107">Attributes and elements</span></span>

<span data-ttu-id="59c6c-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="59c6c-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59c6c-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="59c6c-109">Attributes</span></span>

<span data-ttu-id="59c6c-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59c6c-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59c6c-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="59c6c-111">Child elements</span></span>

|<span data-ttu-id="59c6c-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59c6c-112">**Element**</span></span>|<span data-ttu-id="59c6c-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="59c6c-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59c6c-114">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="59c6c-114">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md) <br/> |<span data-ttu-id="59c6c-115">Identifie le schéma d’une réponse de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="59c6c-115">Identifies the schema for an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="59c6c-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="59c6c-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="59c6c-117">Identifie l’adresse de messagerie de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59c6c-117">Identifies the user's e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="59c6c-118">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="59c6c-118">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="59c6c-119">Identifie la boîte aux lettres d’un utilisateur par un nom unique hérité.</span><span class="sxs-lookup"><span data-stu-id="59c6c-119">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59c6c-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="59c6c-120">Parent elements</span></span>

|<span data-ttu-id="59c6c-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59c6c-121">**Element**</span></span>|<span data-ttu-id="59c6c-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="59c6c-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59c6c-123">AutoDiscover (POX)</span><span class="sxs-lookup"><span data-stu-id="59c6c-123">AutoDiscover (POX)</span></span>](autodiscover-pox.md) <br/> |<span data-ttu-id="59c6c-124">L’élément racine dans une requête de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="59c6c-124">The root element in an Autodiscover request.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59c6c-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59c6c-125">See also</span></span>

- [<span data-ttu-id="59c6c-126">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="59c6c-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

