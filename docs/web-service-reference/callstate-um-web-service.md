---
title: CallState (service Web de messagerie unifiée)
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
ms.openlocfilehash: 44614c460286ff49ebc2373263c1827c6be5cc08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454609"
---
# <a name="callstate-um-web-service"></a><span data-ttu-id="6253b-103">CallState (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="6253b-103">CallState (UM web service)</span></span>

<span data-ttu-id="6253b-104">L’élément **CallState** contient une valeur qui indique l’état d’un appel.</span><span class="sxs-lookup"><span data-stu-id="6253b-104">The **CallState** element contains a value that indicates the status of a call.</span></span> 
  
[<span data-ttu-id="6253b-105">GetCallInfoResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="6253b-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="6253b-106">CallState (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="6253b-106">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 <span data-ttu-id="6253b-107">**UMCallState**</span><span class="sxs-lookup"><span data-stu-id="6253b-107">**UMCallState**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6253b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6253b-108">Attributes and elements</span></span>

<span data-ttu-id="6253b-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6253b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6253b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="6253b-110">Attributes</span></span>

<span data-ttu-id="6253b-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6253b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6253b-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6253b-112">Child elements</span></span>

<span data-ttu-id="6253b-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6253b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6253b-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6253b-114">Parent elements</span></span>

|<span data-ttu-id="6253b-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6253b-115">**Element**</span></span>|<span data-ttu-id="6253b-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="6253b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6253b-117">GetCallInfoResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="6253b-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="6253b-118">Définit une réponse à une [opération GetCallInfo (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="6253b-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6253b-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="6253b-119">Text value</span></span>

<span data-ttu-id="6253b-120">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="6253b-120">A text value is required.</span></span> <span data-ttu-id="6253b-121">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="6253b-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="6253b-122">Engrenage</span><span class="sxs-lookup"><span data-stu-id="6253b-122">Idle</span></span>
    
- <span data-ttu-id="6253b-123">Connexion</span><span class="sxs-lookup"><span data-stu-id="6253b-123">Connecting</span></span>
    
- <span data-ttu-id="6253b-124">Averti</span><span class="sxs-lookup"><span data-stu-id="6253b-124">Alerted</span></span>
    
- <span data-ttu-id="6253b-125">Connecté</span><span class="sxs-lookup"><span data-stu-id="6253b-125">Connected</span></span>
    
- <span data-ttu-id="6253b-126">Déconnecté</span><span class="sxs-lookup"><span data-stu-id="6253b-126">Disconnected</span></span>
    
- <span data-ttu-id="6253b-127">Entrant</span><span class="sxs-lookup"><span data-stu-id="6253b-127">Incoming</span></span>
    
- <span data-ttu-id="6253b-128">Transférés</span><span class="sxs-lookup"><span data-stu-id="6253b-128">Transferring</span></span>
    
- <span data-ttu-id="6253b-129">Transfert</span><span class="sxs-lookup"><span data-stu-id="6253b-129">Forwarding</span></span>
    
## <a name="element-information"></a><span data-ttu-id="6253b-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6253b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6253b-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6253b-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="6253b-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6253b-132">Schema Name</span></span>  <br/> |<span data-ttu-id="6253b-133">Messages</span><span class="sxs-lookup"><span data-stu-id="6253b-133">Messages</span></span>  <br/> |
|<span data-ttu-id="6253b-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6253b-134">Validation File</span></span>  <br/> |<span data-ttu-id="6253b-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6253b-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6253b-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6253b-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="6253b-137">False</span><span class="sxs-lookup"><span data-stu-id="6253b-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6253b-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6253b-138">See also</span></span>



[<span data-ttu-id="6253b-139">Opération GetCallInfo (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="6253b-139">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="6253b-140">GetCallInfoResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="6253b-140">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

