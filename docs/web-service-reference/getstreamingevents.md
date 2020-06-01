---
title: GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: dbe83857-c4f8-4d98-813f-e03c289697a1
description: L’élément GetStreamingEvents représente l’opération utilisée par les clients pour demander des notifications de diffusion en continu à partir du serveur.
ms.openlocfilehash: ec133ecd69c05a2208e95f925133570af0233cf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457318"
---
# <a name="getstreamingevents"></a><span data-ttu-id="a0701-103">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a0701-103">GetStreamingEvents</span></span>

<span data-ttu-id="a0701-104">L’élément **GetStreamingEvents** représente l’opération utilisée par les clients pour demander des notifications de diffusion en continu à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="a0701-104">The **GetStreamingEvents** element represents the operation that is used by clients to request streaming notifications from the server.</span></span> 
  
[<span data-ttu-id="a0701-105">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a0701-105">GetStreamingEvents</span></span>](getstreamingevents.md)
  
```XML
<GetStreamingEvents>
   <SubscriptionId/>
   <ConnectionTimeout/>
</GetStreamingEvents>
```

 <span data-ttu-id="a0701-106">**GetStreamingEventsType**</span><span class="sxs-lookup"><span data-stu-id="a0701-106">**GetStreamingEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0701-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a0701-107">Attributes and elements</span></span>

<span data-ttu-id="a0701-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a0701-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0701-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="a0701-109">Attributes</span></span>

<span data-ttu-id="a0701-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a0701-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0701-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a0701-111">Child elements</span></span>

|<span data-ttu-id="a0701-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a0701-112">**Element**</span></span>|<span data-ttu-id="a0701-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="a0701-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0701-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="a0701-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md) <br/> |<span data-ttu-id="a0701-115">Représente l’identificateur d’un abonnement interrogé pour les événements.</span><span class="sxs-lookup"><span data-stu-id="a0701-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="a0701-116">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="a0701-116">ConnectionTimeout</span></span>](connectiontimeout.md) <br/> |<span data-ttu-id="a0701-117">Représente le nombre de minutes pendant lesquelles une connexion doit rester ouverte.</span><span class="sxs-lookup"><span data-stu-id="a0701-117">Represents the number of minutes to keep a connection open.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a0701-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a0701-118">Parent elements</span></span>

<span data-ttu-id="a0701-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a0701-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a0701-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a0701-120">Text value</span></span>

<span data-ttu-id="a0701-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a0701-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a0701-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="a0701-122">Remarks</span></span>

<span data-ttu-id="a0701-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a0701-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0701-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a0701-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0701-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a0701-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a0701-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a0701-126">Schema name</span></span>  <br/> |<span data-ttu-id="a0701-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a0701-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a0701-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a0701-128">Validation file</span></span>  <br/> |<span data-ttu-id="a0701-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a0701-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a0701-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a0701-130">Can be empty</span></span>  <br/> |<span data-ttu-id="a0701-131">False</span><span class="sxs-lookup"><span data-stu-id="a0701-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0701-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a0701-132">See also</span></span>



[<span data-ttu-id="a0701-133">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="a0701-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="a0701-134">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a0701-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="a0701-135">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="a0701-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="a0701-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a0701-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

