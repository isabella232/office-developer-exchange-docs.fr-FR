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
ms.openlocfilehash: b9af4278a5421dc932573396c3563a64a78de41e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526381"
---
# <a name="legacydn-pox"></a><span data-ttu-id="13611-103">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="13611-103">LegacyDN (POX)</span></span>

<span data-ttu-id="13611-104">L’élément **LegacyDN** identifie la boîte aux lettres d’un utilisateur par un nom unique hérité.</span><span class="sxs-lookup"><span data-stu-id="13611-104">The **LegacyDN** element identifies a user's mailbox by legacy distinguished name.</span></span> 
  
```xml
<LegacyDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="13611-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="13611-105">Attributes and elements</span></span>

<span data-ttu-id="13611-106">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="13611-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13611-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="13611-107">Attributes</span></span>

<span data-ttu-id="13611-108">Aucune.</span><span class="sxs-lookup"><span data-stu-id="13611-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="13611-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="13611-109">Child elements</span></span>

<span data-ttu-id="13611-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="13611-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="13611-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="13611-111">Parent elements</span></span>

|<span data-ttu-id="13611-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="13611-112">**Element**</span></span>|<span data-ttu-id="13611-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="13611-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13611-114">Demande (POX)</span><span class="sxs-lookup"><span data-stu-id="13611-114">Request (POX)</span></span>](request-pox.md) <br/> |<span data-ttu-id="13611-115">Contient la demande au service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="13611-115">Contains the request to the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="13611-116">Utilisateur (POX)</span><span class="sxs-lookup"><span data-stu-id="13611-116">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="13611-117">Fournit des informations spécifiques à l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="13611-117">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="13611-118">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="13611-118">Text value</span></span>

<span data-ttu-id="13611-119">La valeur texte représente l’adresse de messagerie héritée d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="13611-119">The text value represents a user's legacy e-mail address.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="13611-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="13611-120">Remarks</span></span>

<span data-ttu-id="13611-121">L’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est un élément de remplacement pour une demande de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="13611-121">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element is an alternative element for an Autodiscover request.</span></span> <span data-ttu-id="13611-122">Il est utilisé lorsqu’une boîte aux lettres existe sur un ordinateur qui exécute Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="13611-122">It is used when a mailbox exists on a computer that is running Microsoft Exchange Server 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="13611-123">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="13611-123">See also</span></span>

- [<span data-ttu-id="13611-124">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="13611-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

