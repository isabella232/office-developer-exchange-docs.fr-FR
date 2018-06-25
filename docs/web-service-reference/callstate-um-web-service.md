---
title: CallState (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallState
api_type:
- schema
ms.assetid: 88670707-12f7-41c5-ac81-dda0c354a2cb
description: L’élément CallState contient une valeur qui indique l’état d’un appel.
ms.openlocfilehash: e751c2e38783c6634a44d8e1b830a9224cdf300a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755489"
---
# <a name="callstate-um-web-service"></a><span data-ttu-id="5027d-103">CallState (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="5027d-103">CallState (UM web service)</span></span>

<span data-ttu-id="5027d-104">L’élément **CallState** contient une valeur qui indique l’état d’un appel.</span><span class="sxs-lookup"><span data-stu-id="5027d-104">The **CallState** element contains a value that indicates the status of a call.</span></span> 
  
[<span data-ttu-id="5027d-105">GetCallInfoResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="5027d-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="5027d-106">CallState (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="5027d-106">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 <span data-ttu-id="5027d-107">**UMCallState**</span><span class="sxs-lookup"><span data-stu-id="5027d-107">**UMCallState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5027d-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5027d-108">Attributes and elements</span></span>

<span data-ttu-id="5027d-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5027d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5027d-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="5027d-110">Attributes</span></span>

<span data-ttu-id="5027d-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5027d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5027d-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5027d-112">Child elements</span></span>

<span data-ttu-id="5027d-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5027d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5027d-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5027d-114">Parent elements</span></span>

|<span data-ttu-id="5027d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5027d-115">**Element**</span></span>|<span data-ttu-id="5027d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="5027d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5027d-117">GetCallInfoResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="5027d-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="5027d-118">Définit une réponse à une [opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="5027d-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5027d-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5027d-119">Text value</span></span>

<span data-ttu-id="5027d-120">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="5027d-120">A text value is required.</span></span> <span data-ttu-id="5027d-121">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="5027d-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="5027d-122">Inactif</span><span class="sxs-lookup"><span data-stu-id="5027d-122">Idle</span></span>
    
- <span data-ttu-id="5027d-123">Connexion</span><span class="sxs-lookup"><span data-stu-id="5027d-123">Connecting</span></span>
    
- <span data-ttu-id="5027d-124">Alerté</span><span class="sxs-lookup"><span data-stu-id="5027d-124">Alerted</span></span>
    
- <span data-ttu-id="5027d-125">Connecté</span><span class="sxs-lookup"><span data-stu-id="5027d-125">Connected</span></span>
    
- <span data-ttu-id="5027d-126">Déconnecté</span><span class="sxs-lookup"><span data-stu-id="5027d-126">Disconnected</span></span>
    
- <span data-ttu-id="5027d-127">Entrant</span><span class="sxs-lookup"><span data-stu-id="5027d-127">Incoming</span></span>
    
- <span data-ttu-id="5027d-128">Transfert</span><span class="sxs-lookup"><span data-stu-id="5027d-128">Transferring</span></span>
    
- <span data-ttu-id="5027d-129">Transfert</span><span class="sxs-lookup"><span data-stu-id="5027d-129">Forwarding</span></span>
    
## <a name="element-information"></a><span data-ttu-id="5027d-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5027d-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5027d-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5027d-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="5027d-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5027d-132">Schema Name</span></span>  <br/> |<span data-ttu-id="5027d-133">Messages</span><span class="sxs-lookup"><span data-stu-id="5027d-133">Messages</span></span>  <br/> |
|<span data-ttu-id="5027d-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5027d-134">Validation File</span></span>  <br/> |<span data-ttu-id="5027d-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5027d-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5027d-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5027d-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="5027d-137">False</span><span class="sxs-lookup"><span data-stu-id="5027d-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5027d-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5027d-138">See also</span></span>



[<span data-ttu-id="5027d-139">Opération GetCallInfo (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="5027d-139">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="5027d-140">GetCallInfoResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="5027d-140">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

