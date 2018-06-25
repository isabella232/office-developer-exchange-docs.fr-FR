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
description: L’élément GetEvents représente l’opération utilisée par les clients de l’extraction pour demander des notifications à partir du serveur.
ms.openlocfilehash: e7b24207bff579a2f5230676d6520452f96fe0ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756588"
---
# <a name="getevents"></a><span data-ttu-id="d4c83-103">GetEvents</span><span class="sxs-lookup"><span data-stu-id="d4c83-103">GetEvents</span></span>

<span data-ttu-id="d4c83-104">L’élément **GetEvents** représente l’opération utilisée par les clients de l’extraction pour demander des notifications à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="d4c83-104">The **GetEvents** element represents the operation used by pull clients to request notifications from the server.</span></span> 
  
[<span data-ttu-id="d4c83-105">GetEvents</span><span class="sxs-lookup"><span data-stu-id="d4c83-105">GetEvents</span></span>](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 <span data-ttu-id="d4c83-106">**GetEventsType**</span><span class="sxs-lookup"><span data-stu-id="d4c83-106">**GetEventsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4c83-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4c83-107">Attributes and elements</span></span>

<span data-ttu-id="d4c83-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4c83-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4c83-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4c83-109">Attributes</span></span>

<span data-ttu-id="d4c83-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4c83-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4c83-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4c83-111">Child elements</span></span>

|<span data-ttu-id="d4c83-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4c83-112">**Element**</span></span>|<span data-ttu-id="d4c83-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4c83-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4c83-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="d4c83-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="d4c83-115">Représente l’identificateur d’un abonnement est interrogé pour les événements.</span><span class="sxs-lookup"><span data-stu-id="d4c83-115">Represents the identifier for a subscription that is queried for events.</span></span>  <br/> |
|[<span data-ttu-id="d4c83-116">Filigrane</span><span class="sxs-lookup"><span data-stu-id="d4c83-116">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="d4c83-117">Représente le dernier filigrane retourné au client.</span><span class="sxs-lookup"><span data-stu-id="d4c83-117">Represents the last watermark returned to the client.</span></span> <span data-ttu-id="d4c83-118">Si GetEvents n’a pas été appelée pour cet abonnement, le client utilise le filigrane renvoyé à partir de la demande Subscribe.</span><span class="sxs-lookup"><span data-stu-id="d4c83-118">If GetEvents has not been called for this subscription, the client uses the watermark returned from the Subscribe request.</span></span> <span data-ttu-id="d4c83-119">Dans le cas contraire, la limite à partir du dernier événement de la dernière réponse GetEvents est utilisée.</span><span class="sxs-lookup"><span data-stu-id="d4c83-119">Otherwise, the watermark from the last event in the last GetEvents response is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4c83-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4c83-120">Parent elements</span></span>

<span data-ttu-id="d4c83-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4c83-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d4c83-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="d4c83-122">Remarks</span></span>

<span data-ttu-id="d4c83-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d4c83-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4c83-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4c83-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4c83-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4c83-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d4c83-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4c83-126">Schema name</span></span>  <br/> |<span data-ttu-id="d4c83-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d4c83-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d4c83-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4c83-128">Validation file</span></span>  <br/> |<span data-ttu-id="d4c83-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d4c83-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d4c83-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4c83-130">Can be empty</span></span>  <br/> |<span data-ttu-id="d4c83-131">false</span><span class="sxs-lookup"><span data-stu-id="d4c83-131">false</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4c83-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4c83-132">See also</span></span>



[<span data-ttu-id="d4c83-133">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="d4c83-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d4c83-134">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="d4c83-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d4c83-135">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="d4c83-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

