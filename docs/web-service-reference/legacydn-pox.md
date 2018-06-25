---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: L’élément LegacyDN identifie la boîte aux lettres d’un utilisateur par un nom unique hérité.
ms.openlocfilehash: f7ec1dea29a7d3ad6d470ef7812390d179fe1d2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828243"
---
# <a name="legacydn-pox"></a><span data-ttu-id="74fc1-103">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="74fc1-103">LegacyDN (POX)</span></span>

<span data-ttu-id="74fc1-104">L’élément **LegacyDN** identifie la boîte aux lettres d’un utilisateur par un nom unique hérité.</span><span class="sxs-lookup"><span data-stu-id="74fc1-104">The **LegacyDN** element identifies a user's mailbox by legacy distinguished name.</span></span> 
  
```xml
<LegacyDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="74fc1-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="74fc1-105">Attributes and elements</span></span>

<span data-ttu-id="74fc1-106">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="74fc1-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74fc1-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="74fc1-107">Attributes</span></span>

<span data-ttu-id="74fc1-108">Aucun.</span><span class="sxs-lookup"><span data-stu-id="74fc1-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74fc1-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="74fc1-109">Child elements</span></span>

<span data-ttu-id="74fc1-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="74fc1-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="74fc1-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="74fc1-111">Parent elements</span></span>

|<span data-ttu-id="74fc1-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="74fc1-112">**Element**</span></span>|<span data-ttu-id="74fc1-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="74fc1-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74fc1-114">Demande (POX)</span><span class="sxs-lookup"><span data-stu-id="74fc1-114">Request (POX)</span></span>](request-pox.md) <br/> |<span data-ttu-id="74fc1-115">Contient la demande au service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="74fc1-115">Contains the request to the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="74fc1-116">Utilisateur (POX)</span><span class="sxs-lookup"><span data-stu-id="74fc1-116">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="74fc1-117">Fournit des informations spécifiques à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="74fc1-117">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="74fc1-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="74fc1-118">Text value</span></span>

<span data-ttu-id="74fc1-119">La valeur de texte représente l’adresse de messagerie hérités d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="74fc1-119">The text value represents a user's legacy e-mail address.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74fc1-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="74fc1-120">Remarks</span></span>

<span data-ttu-id="74fc1-121">L’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est un autre élément pour une demande de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="74fc1-121">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element is an alternative element for an Autodiscover request.</span></span> <span data-ttu-id="74fc1-122">Il est utilisé lorsqu’une boîte aux lettres existe sur un ordinateur qui exécute Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="74fc1-122">It is used when a mailbox exists on a computer that is running Microsoft Exchange Server 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="74fc1-123">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="74fc1-123">See also</span></span>

- [<span data-ttu-id="74fc1-124">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="74fc1-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

