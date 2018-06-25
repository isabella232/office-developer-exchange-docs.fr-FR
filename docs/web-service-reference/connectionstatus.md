---
title: ConnectionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionStatus
api_type:
- schema
ms.assetid: 4300f9d6-8bf9-48c2-9f07-d80197864e17
description: L’élément ConnectionStatus fournit une description textuelle de l’état d’un abonnement de diffusion en continu.
ms.openlocfilehash: 567308d79eaccba24230deddf5d78a724b8746af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755544"
---
# <a name="connectionstatus"></a><span data-ttu-id="490aa-103">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="490aa-103">ConnectionStatus</span></span>

<span data-ttu-id="490aa-104">L’élément **ConnectionStatus** fournit une description textuelle de l’état d’un abonnement de diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="490aa-104">The **ConnectionStatus** element provides a text description of the status of a streaming subscription.</span></span> 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 <span data-ttu-id="490aa-105">**ConnectionStatusType**</span><span class="sxs-lookup"><span data-stu-id="490aa-105">**ConnectionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="490aa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="490aa-106">Attributes and elements</span></span>

<span data-ttu-id="490aa-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="490aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="490aa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="490aa-108">Attributes</span></span>

<span data-ttu-id="490aa-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="490aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="490aa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="490aa-110">Child elements</span></span>

<span data-ttu-id="490aa-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="490aa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="490aa-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="490aa-112">Parent elements</span></span>

|<span data-ttu-id="490aa-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="490aa-113">**Element**</span></span>|<span data-ttu-id="490aa-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="490aa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="490aa-115">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="490aa-115">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="490aa-116">Contient l’état et les résultats d’une seule demande [d’opération GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="490aa-116">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="490aa-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="490aa-117">Text value</span></span>

<span data-ttu-id="490aa-118">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="490aa-118">A text value is required.</span></span> <span data-ttu-id="490aa-119">Les valeurs de texte possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="490aa-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="490aa-120">OK</span><span class="sxs-lookup"><span data-stu-id="490aa-120">OK</span></span>
    
- <span data-ttu-id="490aa-121">Closed</span><span class="sxs-lookup"><span data-stu-id="490aa-121">Closed</span></span>
    
## <a name="remarks"></a><span data-ttu-id="490aa-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="490aa-122">Remarks</span></span>

<span data-ttu-id="490aa-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="490aa-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="490aa-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="490aa-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="490aa-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="490aa-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="490aa-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="490aa-126">Schema Name</span></span>  <br/> |<span data-ttu-id="490aa-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="490aa-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="490aa-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="490aa-128">Validation File</span></span>  <br/> |<span data-ttu-id="490aa-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="490aa-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="490aa-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="490aa-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="490aa-131">False</span><span class="sxs-lookup"><span data-stu-id="490aa-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="490aa-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="490aa-132">See also</span></span>



[<span data-ttu-id="490aa-133">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="490aa-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="490aa-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="490aa-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

