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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462716"
---
# <a name="connectionstatus"></a><span data-ttu-id="8da77-103">ConnectionStatus Closed</span><span class="sxs-lookup"><span data-stu-id="8da77-103">ConnectionStatus</span></span>

<span data-ttu-id="8da77-104">L’élément **ConnectionStatus Closed** fournit une description textuelle de l’état d’un abonnement de diffusion en continu.</span><span class="sxs-lookup"><span data-stu-id="8da77-104">The **ConnectionStatus** element provides a text description of the status of a streaming subscription.</span></span> 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 <span data-ttu-id="8da77-105">**ConnectionStatusType**</span><span class="sxs-lookup"><span data-stu-id="8da77-105">**ConnectionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8da77-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8da77-106">Attributes and elements</span></span>

<span data-ttu-id="8da77-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8da77-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8da77-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8da77-108">Attributes</span></span>

<span data-ttu-id="8da77-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8da77-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8da77-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8da77-110">Child elements</span></span>

<span data-ttu-id="8da77-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8da77-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8da77-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8da77-112">Parent elements</span></span>

|<span data-ttu-id="8da77-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8da77-113">**Element**</span></span>|<span data-ttu-id="8da77-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="8da77-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8da77-115">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8da77-115">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="8da77-116">Contient l’État et le résultat d’une seule demande d' [opération GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="8da77-116">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8da77-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="8da77-117">Text value</span></span>

<span data-ttu-id="8da77-118">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="8da77-118">A text value is required.</span></span> <span data-ttu-id="8da77-119">Voici les valeurs de texte possibles pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="8da77-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="8da77-120">OK</span><span class="sxs-lookup"><span data-stu-id="8da77-120">OK</span></span>
    
- <span data-ttu-id="8da77-121">Fermé</span><span class="sxs-lookup"><span data-stu-id="8da77-121">Closed</span></span>
    
## <a name="remarks"></a><span data-ttu-id="8da77-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="8da77-122">Remarks</span></span>

<span data-ttu-id="8da77-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8da77-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8da77-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8da77-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8da77-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8da77-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8da77-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8da77-126">Schema Name</span></span>  <br/> |<span data-ttu-id="8da77-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="8da77-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8da77-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8da77-128">Validation File</span></span>  <br/> |<span data-ttu-id="8da77-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8da77-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8da77-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8da77-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="8da77-131">False</span><span class="sxs-lookup"><span data-stu-id="8da77-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8da77-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8da77-132">See also</span></span>



[<span data-ttu-id="8da77-133">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="8da77-133">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)


- [<span data-ttu-id="8da77-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8da77-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

