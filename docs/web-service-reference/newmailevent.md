---
title: NewMailEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewMailEvent
api_type:
- schema
ms.assetid: 45057945-a3ec-4dac-92db-f0dc5fcfc34d
description: L’élément NewMailEvent représente un événement qui est déclenché par un nouvel élément de messagerie dans une boîte aux lettres.
ms.openlocfilehash: 8df3e4a218a8eaa9d129854e4816a3a43beddafa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828527"
---
# <a name="newmailevent"></a><span data-ttu-id="3ae27-103">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="3ae27-103">NewMailEvent</span></span>

<span data-ttu-id="3ae27-104">L’élément **NewMailEvent** représente un événement qui est déclenché par un nouvel élément de messagerie dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3ae27-104">The **NewMailEvent** element represents an event that is triggered by a new mail item in a mailbox.</span></span> 
  
```xml
<NewMailEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</NewMailEvent>
```

 <span data-ttu-id="3ae27-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="3ae27-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3ae27-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3ae27-106">Attributes and elements</span></span>

<span data-ttu-id="3ae27-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3ae27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3ae27-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3ae27-108">Attributes</span></span>

<span data-ttu-id="3ae27-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3ae27-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3ae27-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3ae27-110">Child elements</span></span>

|<span data-ttu-id="3ae27-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3ae27-111">**Element**</span></span>|<span data-ttu-id="3ae27-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3ae27-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ae27-113">Filigrane</span><span class="sxs-lookup"><span data-stu-id="3ae27-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="3ae27-114">Représente un signet d’événements dans la table d’événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3ae27-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="3ae27-115">Horodatage</span><span class="sxs-lookup"><span data-stu-id="3ae27-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="3ae27-116">Représente l’horodatage de l’arrivée d’un nouvel élément de messagerie dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3ae27-116">Represents the timestamp of the arrival of a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="3ae27-117">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="3ae27-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3ae27-118">Représente l’identificateur d’un nouvel élément de messagerie.</span><span class="sxs-lookup"><span data-stu-id="3ae27-118">Represents the identifier of a new mail item.</span></span>  <br/> |
|[<span data-ttu-id="3ae27-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="3ae27-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="3ae27-120">Représente l’identificateur du dossier parent du nouvel élément de messagerie.</span><span class="sxs-lookup"><span data-stu-id="3ae27-120">Represents the identifier of the parent folder of the new mail item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3ae27-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3ae27-121">Parent elements</span></span>

|<span data-ttu-id="3ae27-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3ae27-122">**Element**</span></span>|<span data-ttu-id="3ae27-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="3ae27-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ae27-124">Notification</span><span class="sxs-lookup"><span data-stu-id="3ae27-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3ae27-125">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="3ae27-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3ae27-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="3ae27-126">Remarks</span></span>

<span data-ttu-id="3ae27-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3ae27-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3ae27-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3ae27-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3ae27-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3ae27-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3ae27-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3ae27-130">Schema name</span></span>  <br/> |<span data-ttu-id="3ae27-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3ae27-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="3ae27-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3ae27-132">Validation file</span></span>  <br/> |<span data-ttu-id="3ae27-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3ae27-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3ae27-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3ae27-134">Can be empty</span></span>  <br/> |<span data-ttu-id="3ae27-135">False</span><span class="sxs-lookup"><span data-stu-id="3ae27-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3ae27-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3ae27-136">See also</span></span>



[<span data-ttu-id="3ae27-137">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="3ae27-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="3ae27-138">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="3ae27-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="3ae27-139">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="3ae27-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

