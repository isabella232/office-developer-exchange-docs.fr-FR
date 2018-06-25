---
title: FreeBusyChangedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyChangedEvent
api_type:
- schema
ms.assetid: 63abbfc5-c29f-4110-a922-6b1247187f28
description: L’élément FreeBusyChangedEvent représente un événement dans lequel les temps de disponibilité d’un élément a été modifié.
ms.openlocfilehash: 7271d375526e7614d0150594c2b988666a59eb8d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756485"
---
# <a name="freebusychangedevent"></a><span data-ttu-id="ba62c-103">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="ba62c-103">FreeBusyChangedEvent</span></span>

<span data-ttu-id="ba62c-104">L’élément **FreeBusyChangedEvent** représente un événement dans lequel les temps de disponibilité d’un élément a été modifié.</span><span class="sxs-lookup"><span data-stu-id="ba62c-104">The **FreeBusyChangedEvent** element represents an event in which an item's free/busy time has changed.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

 <span data-ttu-id="ba62c-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="ba62c-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba62c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ba62c-106">Attributes and elements</span></span>

<span data-ttu-id="ba62c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ba62c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba62c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ba62c-108">Attributes</span></span>

<span data-ttu-id="ba62c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba62c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba62c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ba62c-110">Child elements</span></span>

|<span data-ttu-id="ba62c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ba62c-111">**Element**</span></span>|<span data-ttu-id="ba62c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba62c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba62c-113">Filigrane</span><span class="sxs-lookup"><span data-stu-id="ba62c-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="ba62c-114">Représente un signet d’événements dans la table d’événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ba62c-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="ba62c-115">Horodatage</span><span class="sxs-lookup"><span data-stu-id="ba62c-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="ba62c-116">Représente l’horodatage d’un événement de boîte aux lettres d’élément et de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="ba62c-116">Represents the timestamp of a free/busy item mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="ba62c-117">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="ba62c-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ba62c-118">Représente l’identificateur de l’élément et de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="ba62c-118">Represents the identifier of the free/busy item.</span></span>  <br/> |
|[<span data-ttu-id="ba62c-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ba62c-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ba62c-120">Représente l’identificateur du dossier parent de l’élément et de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="ba62c-120">Represents the identifier of the parent folder of the free/busy item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ba62c-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ba62c-121">Parent elements</span></span>

|<span data-ttu-id="ba62c-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ba62c-122">**Element**</span></span>|<span data-ttu-id="ba62c-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba62c-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba62c-124">Notification</span><span class="sxs-lookup"><span data-stu-id="ba62c-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ba62c-125">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="ba62c-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ba62c-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ba62c-126">Text value</span></span>

<span data-ttu-id="ba62c-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba62c-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ba62c-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="ba62c-128">Remarks</span></span>

<span data-ttu-id="ba62c-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ba62c-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba62c-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ba62c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba62c-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ba62c-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba62c-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ba62c-132">Schema name</span></span>  <br/> |<span data-ttu-id="ba62c-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ba62c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba62c-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ba62c-134">Validation file</span></span>  <br/> |<span data-ttu-id="ba62c-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ba62c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba62c-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ba62c-136">Can be empty</span></span>  <br/> |<span data-ttu-id="ba62c-137">False</span><span class="sxs-lookup"><span data-stu-id="ba62c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba62c-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ba62c-138">See also</span></span>



[<span data-ttu-id="ba62c-139">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="ba62c-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="ba62c-140">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="ba62c-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="ba62c-141">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="ba62c-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="ba62c-142">À l’aide d’abonnement</span><span class="sxs-lookup"><span data-stu-id="ba62c-142">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="ba62c-143">Notifications d’événement dans EWS</span><span class="sxs-lookup"><span data-stu-id="ba62c-143">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

