---
title: GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: 22d4da6b-d8a8-484f-82c4-3e4b8f5431cd
description: L’élément GetEvents représente l’opération utilisée par les clients de type pull pour demander des notifications à partir du serveur.
ms.openlocfilehash: 004f782ccd32b3c5e501080bfc59419a6e7d9ce4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462499"
---
# <a name="getevents"></a><span data-ttu-id="5daca-103">GetEvents</span><span class="sxs-lookup"><span data-stu-id="5daca-103">GetEvents</span></span>

<span data-ttu-id="5daca-104">L’élément **GetEvents** représente l’opération utilisée par les clients de type pull pour demander des notifications à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="5daca-104">The **GetEvents** element represents the operation used by pull clients to request notifications from the server.</span></span> 
  
[<span data-ttu-id="5daca-105">GetEvents</span><span class="sxs-lookup"><span data-stu-id="5daca-105">GetEvents</span></span>](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 <span data-ttu-id="5daca-106">**GetEventsType**</span><span class="sxs-lookup"><span data-stu-id="5daca-106">**GetEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5daca-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5daca-107">Attributes and elements</span></span>

<span data-ttu-id="5daca-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5daca-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5daca-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="5daca-109">Attributes</span></span>

<span data-ttu-id="5daca-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5daca-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5daca-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5daca-111">Child elements</span></span>

|<span data-ttu-id="5daca-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5daca-112">**Element**</span></span>|<span data-ttu-id="5daca-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="5daca-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5daca-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="5daca-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="5daca-115">Représente l’identificateur d’un abonnement interrogé pour les événements.</span><span class="sxs-lookup"><span data-stu-id="5daca-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="5daca-116">Watermark</span><span class="sxs-lookup"><span data-stu-id="5daca-116">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="5daca-117">Représente le dernier filigrane renvoyé au client.</span><span class="sxs-lookup"><span data-stu-id="5daca-117">Represents the last watermark returned to the client.</span></span> <span data-ttu-id="5daca-118">Si GetEvents n’a pas été appelé pour cet abonnement, le client utilise le filigrane renvoyé à partir de la demande subscribe.</span><span class="sxs-lookup"><span data-stu-id="5daca-118">If GetEvents has not been called for this subscription, the client uses the watermark returned from the Subscribe request.</span></span> <span data-ttu-id="5daca-119">Dans le cas contraire, le filigrane du dernier événement de la dernière réponse GetEvents est utilisé.</span><span class="sxs-lookup"><span data-stu-id="5daca-119">Otherwise, the watermark from the last event in the last GetEvents response is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5daca-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5daca-120">Parent elements</span></span>

<span data-ttu-id="5daca-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5daca-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5daca-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="5daca-122">Remarks</span></span>

<span data-ttu-id="5daca-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5daca-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5daca-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5daca-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5daca-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5daca-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5daca-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5daca-126">Schema name</span></span>  <br/> |<span data-ttu-id="5daca-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="5daca-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5daca-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5daca-128">Validation file</span></span>  <br/> |<span data-ttu-id="5daca-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5daca-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5daca-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5daca-130">Can be empty</span></span>  <br/> |<span data-ttu-id="5daca-131">false</span><span class="sxs-lookup"><span data-stu-id="5daca-131">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5daca-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5daca-132">See also</span></span>



[<span data-ttu-id="5daca-133">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="5daca-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="5daca-134">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="5daca-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="5daca-135">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="5daca-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

