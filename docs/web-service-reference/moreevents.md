---
title: MoreEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: L’élément MoreEvents indique s’il existe plusieurs événements dans la file d’attente pour être remis au client.
ms.openlocfilehash: cc3f7ed3b4b5f5ce27a9d45d508506bfa62e5086
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828489"
---
# <a name="moreevents"></a><span data-ttu-id="28614-103">MoreEvents</span><span class="sxs-lookup"><span data-stu-id="28614-103">MoreEvents</span></span>

<span data-ttu-id="28614-104">L’élément **MoreEvents** indique s’il existe plusieurs événements dans la file d’attente pour être remis au client.</span><span class="sxs-lookup"><span data-stu-id="28614-104">The **MoreEvents** element indicates whether there are more events in the queue to be delivered to the client.</span></span> 
  
```xml
<MoreEvents/>
```

 <span data-ttu-id="28614-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="28614-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28614-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="28614-106">Attributes and elements</span></span>

<span data-ttu-id="28614-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="28614-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28614-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="28614-108">Attributes</span></span>

<span data-ttu-id="28614-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28614-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28614-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="28614-110">Child elements</span></span>

<span data-ttu-id="28614-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28614-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="28614-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="28614-112">Parent elements</span></span>

|<span data-ttu-id="28614-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28614-113">**Element**</span></span>|<span data-ttu-id="28614-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="28614-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28614-115">Notification</span><span class="sxs-lookup"><span data-stu-id="28614-115">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="28614-116">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="28614-116">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="28614-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="28614-117">Text value</span></span>

<span data-ttu-id="28614-118">La valeur de texte représente une valeur de type Boolean.</span><span class="sxs-lookup"><span data-stu-id="28614-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="28614-119">La valeur **true** indique que plusieurs événements sont dans la file d’attente.</span><span class="sxs-lookup"><span data-stu-id="28614-119">A value of **true** indicates that more events are in the queue.</span></span> <span data-ttu-id="28614-120">La valeur **false** indique que plus aucun événement ne se trouvent dans la file d’attente.</span><span class="sxs-lookup"><span data-stu-id="28614-120">A value of **false** indicates that no more events are in the queue.</span></span> <span data-ttu-id="28614-121">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="28614-121">This property is read-only.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="28614-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="28614-122">Remarks</span></span>

<span data-ttu-id="28614-123">Dans le cas des notifications de type Pull, la valeur **true** dans cet élément indique au client qu’une autre demande GetEvents doit être émise pour obtenir les autres événements.</span><span class="sxs-lookup"><span data-stu-id="28614-123">In the case of Pull notifications, a **true** value in this element indicates to the client that another GetEvents request should be issued to get the remaining events.</span></span> <span data-ttu-id="28614-124">En supposant que les spécifications client nécessitent latence minimale pour les notifications d’événements, les demandes GetEvents devraient continuer dans une suite continue jusqu'à ce qu’un **faux** valeur **MoreEvents** est retourné.</span><span class="sxs-lookup"><span data-stu-id="28614-124">Assuming that the client specifications require minimum latency for event notifications, GetEvents requests should continue in a continuous succession until a **false** **MoreEvents** value is returned.</span></span> 
  
<span data-ttu-id="28614-125">Dans le cas de notifications Push, la valeur **true** pour **MoreEvents** indique au client qu’un autre notification demande sera envoyée au client pour fournir les autres événements.</span><span class="sxs-lookup"><span data-stu-id="28614-125">In the case of Push notifications, a **true** value for **MoreEvents** indicates to the client that another notification request will be sent to the client to deliver the remaining events.</span></span> <span data-ttu-id="28614-126">Similaire aux notifications de type Pull, ces demandes suivis continuera à la suite continue jusqu'à ce que la file d’attente sur le serveur d’accès au Client est vide.</span><span class="sxs-lookup"><span data-stu-id="28614-126">Similar to Pull notifications, these follow-up requests will continue in continuous succession until the event queue on the Client Access server is empty.</span></span> 
  
<span data-ttu-id="28614-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="28614-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28614-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="28614-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28614-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="28614-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="28614-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="28614-130">Schema Name</span></span>  <br/> |<span data-ttu-id="28614-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="28614-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="28614-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="28614-132">Validation File</span></span>  <br/> |<span data-ttu-id="28614-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="28614-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="28614-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="28614-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="28614-135">False</span><span class="sxs-lookup"><span data-stu-id="28614-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28614-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="28614-136">See also</span></span>



[<span data-ttu-id="28614-137">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="28614-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="28614-138">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="28614-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="28614-139">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="28614-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

