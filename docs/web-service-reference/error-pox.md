---
title: Erreur (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: L’élément error contient une réponse d’erreur de découverte automatique.
ms.openlocfilehash: 1a1a3e83898674e605921cb75371036a8a561a95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530648"
---
# <a name="error-pox"></a><span data-ttu-id="5095b-103">Erreur (POX)</span><span class="sxs-lookup"><span data-stu-id="5095b-103">Error (POX)</span></span>

<span data-ttu-id="5095b-104">L’élément **Error** contient une réponse d’erreur de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="5095b-104">The **Error** element contains an Autodiscover error response.</span></span> 
  
[<span data-ttu-id="5095b-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="5095b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="5095b-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="5095b-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="5095b-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="5095b-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="5095b-108">Erreur (POX)</span><span class="sxs-lookup"><span data-stu-id="5095b-108">Error (POX)</span></span>](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="5095b-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5095b-109">Attributes and elements</span></span>

<span data-ttu-id="5095b-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5095b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5095b-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="5095b-111">Attributes</span></span>

|<span data-ttu-id="5095b-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="5095b-112">**Attribute**</span></span>|<span data-ttu-id="5095b-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="5095b-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5095b-114">Time</span><span class="sxs-lookup"><span data-stu-id="5095b-114">Time</span></span>  <br/> |<span data-ttu-id="5095b-115">Représente l’heure à laquelle la réponse d’erreur a été renvoyée.</span><span class="sxs-lookup"><span data-stu-id="5095b-115">Represents the time when the error response was returned.</span></span>  <br/> |
|<span data-ttu-id="5095b-116">ID</span><span class="sxs-lookup"><span data-stu-id="5095b-116">Id</span></span>  <br/> |<span data-ttu-id="5095b-117">Représente un hachage du nom de l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5095b-117">Represents a hash of the name of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5095b-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5095b-118">Child elements</span></span>

|<span data-ttu-id="5095b-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5095b-119">**Element**</span></span>|<span data-ttu-id="5095b-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="5095b-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5095b-121">ErrorCode (POX)</span><span class="sxs-lookup"><span data-stu-id="5095b-121">ErrorCode (POX)</span></span>](errorcode-pox.md) <br/> |<span data-ttu-id="5095b-122">Contient le code d’erreur d’une réponse de découverte automatique d’erreur.</span><span class="sxs-lookup"><span data-stu-id="5095b-122">Contains the error code for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="5095b-123">Message (POX)</span><span class="sxs-lookup"><span data-stu-id="5095b-123">Message (POX)</span></span>](message-pox.md) <br/> |<span data-ttu-id="5095b-124">Contient le message d’erreur pour une réponse de découverte automatique d’erreur.</span><span class="sxs-lookup"><span data-stu-id="5095b-124">Contains the error message for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="5095b-125">DebugData (POX)</span><span class="sxs-lookup"><span data-stu-id="5095b-125">DebugData (POX)</span></span>](debugdata-pox.md) <br/> |<span data-ttu-id="5095b-126">Contient les données de débogage pour une réponse de découverte automatique d’erreur.</span><span class="sxs-lookup"><span data-stu-id="5095b-126">Contains the debug data for an error Autodiscover response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5095b-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5095b-127">Parent elements</span></span>

|<span data-ttu-id="5095b-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5095b-128">**Element**</span></span>|<span data-ttu-id="5095b-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="5095b-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5095b-130">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="5095b-130">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="5095b-131">Contient une réponse d’erreur de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="5095b-131">Contains an Autodiscover error response.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5095b-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5095b-132">See also</span></span>



[<span data-ttu-id="5095b-133">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="5095b-133">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

