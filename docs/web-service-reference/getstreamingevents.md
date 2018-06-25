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
description: L’élément GetStreamingEvents représente l’opération qui est utilisée par les clients pour demander des notifications de diffusion en continu à partir du serveur.
ms.openlocfilehash: b07015541cf9c2fbbbc11ebc9f10421bdb9ee84f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827679"
---
# <a name="getstreamingevents"></a><span data-ttu-id="794f0-103">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="794f0-103">GetStreamingEvents</span></span>

<span data-ttu-id="794f0-104">L’élément **GetStreamingEvents** représente l’opération qui est utilisée par les clients pour demander des notifications de diffusion en continu à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="794f0-104">The **GetStreamingEvents** element represents the operation that is used by clients to request streaming notifications from the server.</span></span> 
  
[<span data-ttu-id="794f0-105">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="794f0-105">GetStreamingEvents</span></span>](getstreamingevents.md)
  
```XML
<GetStreamingEvents>
   <SubscriptionId/>
   <ConnectionTimeout/>
</GetStreamingEvents>
```

 <span data-ttu-id="794f0-106">**GetStreamingEventsType**</span><span class="sxs-lookup"><span data-stu-id="794f0-106">**GetStreamingEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="794f0-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="794f0-107">Attributes and elements</span></span>

<span data-ttu-id="794f0-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="794f0-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="794f0-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="794f0-109">Attributes</span></span>

<span data-ttu-id="794f0-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="794f0-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="794f0-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="794f0-111">Child elements</span></span>

|<span data-ttu-id="794f0-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="794f0-112">**Element**</span></span>|<span data-ttu-id="794f0-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="794f0-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="794f0-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="794f0-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md) <br/> |<span data-ttu-id="794f0-115">Représente l’identificateur d’un abonnement est interrogé pour les événements.</span><span class="sxs-lookup"><span data-stu-id="794f0-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="794f0-116">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="794f0-116">ConnectionTimeout</span></span>](connectiontimeout.md) <br/> |<span data-ttu-id="794f0-117">Représente le nombre de minutes à conserver une connexion ouverte.</span><span class="sxs-lookup"><span data-stu-id="794f0-117">Represents the number of minutes to keep a connection open.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="794f0-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="794f0-118">Parent elements</span></span>

<span data-ttu-id="794f0-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="794f0-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="794f0-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="794f0-120">Text value</span></span>

<span data-ttu-id="794f0-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="794f0-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="794f0-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="794f0-122">Remarks</span></span>

<span data-ttu-id="794f0-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="794f0-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="794f0-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="794f0-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="794f0-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="794f0-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="794f0-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="794f0-126">Schema name</span></span>  <br/> |<span data-ttu-id="794f0-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="794f0-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="794f0-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="794f0-128">Validation file</span></span>  <br/> |<span data-ttu-id="794f0-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="794f0-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="794f0-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="794f0-130">Can be empty</span></span>  <br/> |<span data-ttu-id="794f0-131">False</span><span class="sxs-lookup"><span data-stu-id="794f0-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="794f0-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="794f0-132">See also</span></span>



[<span data-ttu-id="794f0-133">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="794f0-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="794f0-134">Opération de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="794f0-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="794f0-135">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="794f0-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="794f0-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="794f0-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

