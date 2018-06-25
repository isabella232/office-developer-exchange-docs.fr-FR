---
title: SubscriptionId (GetEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionId
api_type:
- schema
ms.assetid: 77c0abab-69e8-428e-8c20-22258e4ef71b
description: L’élément SubscriptionId représente l’identificateur d’un abonnement.
ms.openlocfilehash: 8867b7da7c75cfd9d41f708c0481627d5186cc14
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829622"
---
# <a name="subscriptionid-getevents"></a><span data-ttu-id="49dbe-103">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="49dbe-103">SubscriptionId (GetEvents)</span></span>

<span data-ttu-id="49dbe-104">L’élément **SubscriptionId** représente l’identificateur d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="49dbe-104">The **SubscriptionId** element represents the identifier for a subscription.</span></span> 
  
```xml
<SubscriptionId/>
```

 <span data-ttu-id="49dbe-105">**SubscriptionIdType**</span><span class="sxs-lookup"><span data-stu-id="49dbe-105">**SubscriptionIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49dbe-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="49dbe-106">Attributes and elements</span></span>

<span data-ttu-id="49dbe-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="49dbe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49dbe-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="49dbe-108">Attributes</span></span>

<span data-ttu-id="49dbe-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="49dbe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49dbe-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="49dbe-110">Child elements</span></span>

<span data-ttu-id="49dbe-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="49dbe-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="49dbe-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="49dbe-112">Parent elements</span></span>

|<span data-ttu-id="49dbe-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="49dbe-113">**Element**</span></span>|<span data-ttu-id="49dbe-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="49dbe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49dbe-115">GetEvents</span><span class="sxs-lookup"><span data-stu-id="49dbe-115">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="49dbe-116">Représente l’opération utilisée par les clients de l’extraction pour demander des notifications à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="49dbe-116">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="49dbe-117">Notification</span><span class="sxs-lookup"><span data-stu-id="49dbe-117">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="49dbe-118">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="49dbe-118">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="49dbe-119">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="49dbe-119">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="49dbe-120">Contient l’état et les résultats d’une demande Subscribe.</span><span class="sxs-lookup"><span data-stu-id="49dbe-120">Contains the status and result of a Subscribe request.</span></span>  <br/> |
|[<span data-ttu-id="49dbe-121">Annuler l’abonnement</span><span class="sxs-lookup"><span data-stu-id="49dbe-121">Unsubscribe</span></span>](unsubscribe.md) <br/> |<span data-ttu-id="49dbe-122">Contient les propriétés utilisées pour annuler l’abonnement à partir d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="49dbe-122">Contains the properties used to unsubscribe from a subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="49dbe-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="49dbe-123">Text value</span></span>

<span data-ttu-id="49dbe-124">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="49dbe-124">A text value is required.</span></span> <span data-ttu-id="49dbe-125">La valeur de texte est un GUID.</span><span class="sxs-lookup"><span data-stu-id="49dbe-125">The text value is a GUID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="49dbe-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="49dbe-126">Remarks</span></span>

<span data-ttu-id="49dbe-127">Le GUID qui représente l’identificateur d’abonnement est généré par le serveur d’accès au Client lors de la création de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="49dbe-127">The GUID that represents the subscription identifier is generated by the Client Access server when the subscription is created.</span></span>
  
<span data-ttu-id="49dbe-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="49dbe-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49dbe-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="49dbe-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49dbe-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="49dbe-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="49dbe-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="49dbe-131">Schema name</span></span>  <br/> |<span data-ttu-id="49dbe-132">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="49dbe-132">messages schema</span></span>  <br/> |
|<span data-ttu-id="49dbe-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="49dbe-133">Validation file</span></span>  <br/> |<span data-ttu-id="49dbe-134">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="49dbe-134">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="49dbe-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="49dbe-135">Can be empty</span></span>  <br/> |<span data-ttu-id="49dbe-136">False</span><span class="sxs-lookup"><span data-stu-id="49dbe-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49dbe-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="49dbe-137">See also</span></span>



[<span data-ttu-id="49dbe-138">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="49dbe-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="49dbe-139">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="49dbe-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="49dbe-140">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="49dbe-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

