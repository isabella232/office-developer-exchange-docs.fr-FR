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
ms.openlocfilehash: e103386f466d65717878b4a6c811f3c3ad6e7c7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465351"
---
# <a name="subscriptionid-getevents"></a><span data-ttu-id="24722-103">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="24722-103">SubscriptionId (GetEvents)</span></span>

<span data-ttu-id="24722-104">L’élément **SubscriptionId** représente l’identificateur d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="24722-104">The **SubscriptionId** element represents the identifier for a subscription.</span></span> 
  
```xml
<SubscriptionId/>
```

 <span data-ttu-id="24722-105">**SubscriptionIdType**</span><span class="sxs-lookup"><span data-stu-id="24722-105">**SubscriptionIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24722-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="24722-106">Attributes and elements</span></span>

<span data-ttu-id="24722-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="24722-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24722-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="24722-108">Attributes</span></span>

<span data-ttu-id="24722-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="24722-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24722-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="24722-110">Child elements</span></span>

<span data-ttu-id="24722-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="24722-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="24722-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="24722-112">Parent elements</span></span>

|<span data-ttu-id="24722-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="24722-113">**Element**</span></span>|<span data-ttu-id="24722-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="24722-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24722-115">GetEvents</span><span class="sxs-lookup"><span data-stu-id="24722-115">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="24722-116">Représente l’opération utilisée par les clients de type pull pour demander des notifications à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="24722-116">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="24722-117">Notification</span><span class="sxs-lookup"><span data-stu-id="24722-117">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="24722-118">Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="24722-118">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="24722-119">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="24722-119">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="24722-120">Contient l’État et le résultat d’une demande subscribe.</span><span class="sxs-lookup"><span data-stu-id="24722-120">Contains the status and result of a Subscribe request.</span></span>  <br/> |
|[<span data-ttu-id="24722-121">Se désabonner</span><span class="sxs-lookup"><span data-stu-id="24722-121">Unsubscribe</span></span>](unsubscribe.md) <br/> |<span data-ttu-id="24722-122">Contient les propriétés utilisées pour annuler l’abonnement à un abonnement.</span><span class="sxs-lookup"><span data-stu-id="24722-122">Contains the properties used to unsubscribe from a subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="24722-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="24722-123">Text value</span></span>

<span data-ttu-id="24722-124">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="24722-124">A text value is required.</span></span> <span data-ttu-id="24722-125">La valeur texte est un GUID.</span><span class="sxs-lookup"><span data-stu-id="24722-125">The text value is a GUID.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="24722-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="24722-126">Remarks</span></span>

<span data-ttu-id="24722-127">Le GUID qui représente l’identificateur d’abonnement est généré par le serveur d’accès au client lors de la création de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="24722-127">The GUID that represents the subscription identifier is generated by the Client Access server when the subscription is created.</span></span>
  
<span data-ttu-id="24722-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="24722-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24722-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="24722-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24722-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="24722-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="24722-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="24722-131">Schema name</span></span>  <br/> |<span data-ttu-id="24722-132">schéma des messages</span><span class="sxs-lookup"><span data-stu-id="24722-132">messages schema</span></span>  <br/> |
|<span data-ttu-id="24722-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="24722-133">Validation file</span></span>  <br/> |<span data-ttu-id="24722-134">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="24722-134">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="24722-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="24722-135">Can be empty</span></span>  <br/> |<span data-ttu-id="24722-136">False</span><span class="sxs-lookup"><span data-stu-id="24722-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24722-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="24722-137">See also</span></span>



[<span data-ttu-id="24722-138">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="24722-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="24722-139">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="24722-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="24722-140">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="24722-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

