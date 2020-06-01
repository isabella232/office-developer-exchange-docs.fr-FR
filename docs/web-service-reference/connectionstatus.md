---
title: ConnectionStatus Closed
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
description: L’élément ConnectionStatus Closed fournit une description textuelle de l’état d’un abonnement de diffusion en continu.
ms.openlocfilehash: 928537201041950011ae06444e3c412228d252ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462716"
---
# <a name="connectionstatus"></a><span data-ttu-id="c044e-103">ConnectionStatus Closed</span><span class="sxs-lookup"><span data-stu-id="c044e-103">ConnectionStatus</span></span>

<span data-ttu-id="c044e-104">L’élément **ConnectionStatus Closed** fournit une description textuelle de l’état d’un abonnement de diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="c044e-104">The **ConnectionStatus** element provides a text description of the status of a streaming subscription.</span></span> 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 <span data-ttu-id="c044e-105">**ConnectionStatusType**</span><span class="sxs-lookup"><span data-stu-id="c044e-105">**ConnectionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c044e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c044e-106">Attributes and elements</span></span>

<span data-ttu-id="c044e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c044e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c044e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c044e-108">Attributes</span></span>

<span data-ttu-id="c044e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c044e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c044e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c044e-110">Child elements</span></span>

<span data-ttu-id="c044e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c044e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c044e-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c044e-112">Parent elements</span></span>

|<span data-ttu-id="c044e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c044e-113">**Element**</span></span>|<span data-ttu-id="c044e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="c044e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c044e-115">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c044e-115">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="c044e-116">Contient l’État et le résultat d’une seule demande d' [opération GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c044e-116">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c044e-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="c044e-117">Text value</span></span>

<span data-ttu-id="c044e-118">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="c044e-118">A text value is required.</span></span> <span data-ttu-id="c044e-119">Voici les valeurs de texte possibles pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="c044e-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="c044e-120">OK</span><span class="sxs-lookup"><span data-stu-id="c044e-120">OK</span></span>
    
- <span data-ttu-id="c044e-121">Fermé</span><span class="sxs-lookup"><span data-stu-id="c044e-121">Closed</span></span>
    
## <a name="remarks"></a><span data-ttu-id="c044e-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="c044e-122">Remarks</span></span>

<span data-ttu-id="c044e-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c044e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c044e-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c044e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c044e-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c044e-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c044e-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c044e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c044e-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="c044e-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c044e-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c044e-128">Validation File</span></span>  <br/> |<span data-ttu-id="c044e-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c044e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c044e-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c044e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c044e-131">False</span><span class="sxs-lookup"><span data-stu-id="c044e-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c044e-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c044e-132">See also</span></span>



[<span data-ttu-id="c044e-133">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="c044e-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="c044e-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c044e-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

