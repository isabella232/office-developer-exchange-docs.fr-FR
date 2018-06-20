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
description: L’élément Error contient une réponse d’erreur de découverte automatique.
ms.openlocfilehash: 3135a352365fe3000ce2d202ad78452d5c8ccc7f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756202"
---
# <a name="error-pox"></a><span data-ttu-id="304f9-103">Erreur (POX)</span><span class="sxs-lookup"><span data-stu-id="304f9-103">Error (POX)</span></span>

<span data-ttu-id="304f9-104">L’élément **Error** contient une réponse d’erreur de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="304f9-104">The **Error** element contains an Autodiscover error response.</span></span> 
  
[<span data-ttu-id="304f9-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="304f9-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="304f9-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="304f9-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="304f9-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="304f9-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="304f9-108">Erreur (POX)</span><span class="sxs-lookup"><span data-stu-id="304f9-108">Error (POX)</span></span>](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="304f9-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="304f9-109">Attributes and elements</span></span>

<span data-ttu-id="304f9-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="304f9-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="304f9-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="304f9-111">Attributes</span></span>

|<span data-ttu-id="304f9-112">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="304f9-112">**Attribute**</span></span>|<span data-ttu-id="304f9-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="304f9-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="304f9-114">Heure</span><span class="sxs-lookup"><span data-stu-id="304f9-114">Time</span></span>  <br/> |<span data-ttu-id="304f9-115">Représente le temps lorsque la réponse d’erreur a été renvoyée.</span><span class="sxs-lookup"><span data-stu-id="304f9-115">Represents the time when the error response was returned.</span></span>  <br/> |
|<span data-ttu-id="304f9-116">ID</span><span class="sxs-lookup"><span data-stu-id="304f9-116">Id</span></span>  <br/> |<span data-ttu-id="304f9-117">Représente un hachage du nom de l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="304f9-117">Represents a hash of the name of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="304f9-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="304f9-118">Child elements</span></span>

|<span data-ttu-id="304f9-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="304f9-119">**Element**</span></span>|<span data-ttu-id="304f9-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="304f9-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="304f9-121">ErrorCode (POX)</span><span class="sxs-lookup"><span data-stu-id="304f9-121">ErrorCode (POX)</span></span>](errorcode-pox.md) <br/> |<span data-ttu-id="304f9-122">Contient le code d’erreur pour une erreur de réponse de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="304f9-122">Contains the error code for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="304f9-123">Message (POX)</span><span class="sxs-lookup"><span data-stu-id="304f9-123">Message (POX)</span></span>](message-pox.md) <br/> |<span data-ttu-id="304f9-124">Contient le message d’erreur pour une erreur de réponse de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="304f9-124">Contains the error message for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="304f9-125">DebugData (POX)</span><span class="sxs-lookup"><span data-stu-id="304f9-125">DebugData (POX)</span></span>](debugdata-pox.md) <br/> |<span data-ttu-id="304f9-126">Contient les données de débogage pour une erreur de réponse de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="304f9-126">Contains the debug data for an error Autodiscover response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="304f9-127">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="304f9-127">Parent elements</span></span>

|<span data-ttu-id="304f9-128">**Élément**</span><span class="sxs-lookup"><span data-stu-id="304f9-128">**Element**</span></span>|<span data-ttu-id="304f9-129">**Description**</span><span class="sxs-lookup"><span data-stu-id="304f9-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="304f9-130">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="304f9-130">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="304f9-131">Contient une réponse d’erreur de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="304f9-131">Contains an Autodiscover error response.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="304f9-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="304f9-132">See also</span></span>



[<span data-ttu-id="304f9-133">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="304f9-133">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

