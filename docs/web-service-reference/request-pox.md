---
title: Demande (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: L’élément Request contient la demande au service de découverte automatique.
ms.openlocfilehash: bc215d614441ed8f12c0f1490f4abdbb7b574ad0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459545"
---
# <a name="request-pox"></a><span data-ttu-id="ed87f-103">Demande (POX)</span><span class="sxs-lookup"><span data-stu-id="ed87f-103">Request (POX)</span></span>

<span data-ttu-id="ed87f-104">L’élément **Request** contient la demande au service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="ed87f-104">The **Request** element contains the request to the Autodiscover service.</span></span> 
  
- [<span data-ttu-id="ed87f-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="ed87f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="ed87f-106">Demande (POX)</span><span class="sxs-lookup"><span data-stu-id="ed87f-106">Request (POX)</span></span>](request-pox.md)
  
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

## <a name="attributes-and-elements"></a><span data-ttu-id="ed87f-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ed87f-107">Attributes and elements</span></span>

<span data-ttu-id="ed87f-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ed87f-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed87f-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="ed87f-109">Attributes</span></span>

<span data-ttu-id="ed87f-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ed87f-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed87f-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ed87f-111">Child elements</span></span>

|<span data-ttu-id="ed87f-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ed87f-112">**Element**</span></span>|<span data-ttu-id="ed87f-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="ed87f-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed87f-114">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="ed87f-114">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md) <br/> |<span data-ttu-id="ed87f-115">Identifie le schéma d’une réponse de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="ed87f-115">Identifies the schema for an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="ed87f-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="ed87f-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="ed87f-117">Identifie l’adresse de messagerie de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ed87f-117">Identifies the user's e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="ed87f-118">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="ed87f-118">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="ed87f-119">Identifie la boîte aux lettres d’un utilisateur par le nom unique hérité.</span><span class="sxs-lookup"><span data-stu-id="ed87f-119">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed87f-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ed87f-120">Parent elements</span></span>

|<span data-ttu-id="ed87f-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ed87f-121">**Element**</span></span>|<span data-ttu-id="ed87f-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="ed87f-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed87f-123">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="ed87f-123">AutoDiscover (POX)</span></span>](autodiscover-pox.md) <br/> |<span data-ttu-id="ed87f-124">Élément racine dans une demande de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="ed87f-124">The root element in an Autodiscover request.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed87f-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ed87f-125">See also</span></span>

- [<span data-ttu-id="ed87f-126">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ed87f-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

