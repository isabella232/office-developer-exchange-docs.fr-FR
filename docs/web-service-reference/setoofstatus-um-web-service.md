---
title: SetOofStatus (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 9fc0ea9c-7a98-4fd7-a90c-cf5639c63a3a
description: L’élément SetOofStatus définit une demande pour définir l’état Unified Messaging d’absence du bureau Office (OOF) de l’utilisateur qui effectue la demande.
ms.openlocfilehash: df28c98013e1d5c00ea120ce1aa342e9fc2c6f31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829447"
---
# <a name="setoofstatus-um-web-service"></a><span data-ttu-id="812f9-103">SetOofStatus (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="812f9-103">SetOofStatus (UM web service)</span></span>

<span data-ttu-id="812f9-104">L’élément **SetOofStatus** définit une demande pour définir l’état Unified Messaging d’absence du bureau Office (OOF) de l’utilisateur qui effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="812f9-104">The **SetOofStatus** element defines a request to set the Unified Messaging Out of Office (OOF) status for the user who makes the request.</span></span> 
  
[<span data-ttu-id="812f9-105">SetOofStatus (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="812f9-105">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 <span data-ttu-id="812f9-106">**Type**</span><span class="sxs-lookup"><span data-stu-id="812f9-106">**Type**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="812f9-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="812f9-107">Attributes and elements</span></span>

<span data-ttu-id="812f9-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="812f9-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="812f9-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="812f9-109">Attributes</span></span>

<span data-ttu-id="812f9-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="812f9-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="812f9-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="812f9-111">Child elements</span></span>

|<span data-ttu-id="812f9-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="812f9-112">**Element**</span></span>|<span data-ttu-id="812f9-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="812f9-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="812f9-114">État (service web de messagerie unifiée - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="812f9-114">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md) <br/> |<span data-ttu-id="812f9-115">Définit une valeur à utiliser dans une requête [d’opération SetOofStatus (service web de messagerie unifiée)](setoofstatus-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="812f9-115">Defines a value to use in a [SetOofStatus operation (UM web service)](setoofstatus-operation-um-web-service.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="812f9-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="812f9-116">Parent elements</span></span>

<span data-ttu-id="812f9-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="812f9-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="812f9-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="812f9-118">Text value</span></span>

<span data-ttu-id="812f9-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="812f9-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="812f9-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="812f9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="812f9-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="812f9-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="812f9-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="812f9-122">Schema Name</span></span>  <br/> |<span data-ttu-id="812f9-123">Messages</span><span class="sxs-lookup"><span data-stu-id="812f9-123">Messages</span></span>  <br/> |
|<span data-ttu-id="812f9-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="812f9-124">Validation File</span></span>  <br/> |<span data-ttu-id="812f9-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="812f9-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="812f9-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="812f9-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="812f9-127">False</span><span class="sxs-lookup"><span data-stu-id="812f9-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="812f9-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="812f9-128">See also</span></span>



[<span data-ttu-id="812f9-129">Opération SetOofStatus (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="812f9-129">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)
  
[<span data-ttu-id="812f9-130">État (service web de messagerie unifiée - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="812f9-130">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)

