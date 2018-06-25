---
title: Notifications
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notifications
api_type:
- schema
ms.assetid: 153cc420-d2fe-42f1-afb2-9a31ee09a750
description: L’élément de Notifications contient un tableau d’informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.
ms.openlocfilehash: f576bf579c91b77dcde8646a6af7fdc47145aef7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828550"
---
# <a name="notifications"></a><span data-ttu-id="e3bd9-103">Notifications</span><span class="sxs-lookup"><span data-stu-id="e3bd9-103">Notifications</span></span>

<span data-ttu-id="e3bd9-104">L’élément de **Notifications** contient un tableau d’informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="e3bd9-104">The **Notifications** element contains an array of information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notifications>
   <Notification/>
</Notifications>
```

 <span data-ttu-id="e3bd9-105">**NonEmptyArrayOfNotificationsType**</span><span class="sxs-lookup"><span data-stu-id="e3bd9-105">**NonEmptyArrayOfNotificationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3bd9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e3bd9-106">Attributes and elements</span></span>

<span data-ttu-id="e3bd9-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e3bd9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3bd9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e3bd9-108">Attributes</span></span>

<span data-ttu-id="e3bd9-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e3bd9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3bd9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e3bd9-110">Child elements</span></span>

|<span data-ttu-id="e3bd9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e3bd9-111">**Element**</span></span>|<span data-ttu-id="e3bd9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e3bd9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3bd9-113">Notification</span><span class="sxs-lookup"><span data-stu-id="e3bd9-113">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e3bd9-114">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="e3bd9-114">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3bd9-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e3bd9-115">Parent elements</span></span>

|<span data-ttu-id="e3bd9-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e3bd9-116">**Element**</span></span>|<span data-ttu-id="e3bd9-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="e3bd9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3bd9-118">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e3bd9-118">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md) <br/> |<span data-ttu-id="e3bd9-119">Contient l’état et les résultats d’une seule demande [d’opération GetStreamingEvents](getstreamingevents-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="e3bd9-119">Contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e3bd9-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e3bd9-120">Text value</span></span>

<span data-ttu-id="e3bd9-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e3bd9-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e3bd9-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="e3bd9-122">Remarks</span></span>

<span data-ttu-id="e3bd9-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e3bd9-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3bd9-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e3bd9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3bd9-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e3bd9-125">Namespace</span></span>  <br/> |<span data-ttu-id="e3bd9-126">http://schemas.microsoft.com/exchange/services/2006/messages et http://schemas.microsoft.com/exchange/services/2006/types</span><span class="sxs-lookup"><span data-stu-id="e3bd9-126">http://schemas.microsoft.com/exchange/services/2006/messages and http://schemas.microsoft.com/exchange/services/2006/types</span></span>  <br/> |
|<span data-ttu-id="e3bd9-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e3bd9-127">Schema Name</span></span>  <br/> |<span data-ttu-id="e3bd9-128">Schéma des messages ; Schéma de types</span><span class="sxs-lookup"><span data-stu-id="e3bd9-128">Messages schema; Types schema</span></span>  <br/> |
|<span data-ttu-id="e3bd9-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e3bd9-129">Validation File</span></span>  <br/> |<span data-ttu-id="e3bd9-130">Messages.xsd ; Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e3bd9-130">Messages.xsd; Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e3bd9-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e3bd9-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3bd9-132">False</span><span class="sxs-lookup"><span data-stu-id="e3bd9-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3bd9-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e3bd9-133">See also</span></span>



[<span data-ttu-id="e3bd9-134">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="e3bd9-134">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="e3bd9-135">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="e3bd9-135">DeleteFolder operation</span></span>](deletefolder-operation.md)
  
[<span data-ttu-id="e3bd9-136">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="e3bd9-136">MoveFolder operation</span></span>](movefolder-operation.md)
  
[<span data-ttu-id="e3bd9-137">Opération CopyFolder</span><span class="sxs-lookup"><span data-stu-id="e3bd9-137">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="e3bd9-138">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="e3bd9-138">Subscribe operation</span></span>](subscribe-operation.md)

