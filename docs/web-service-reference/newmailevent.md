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
description: L’élément NewMailEvent représente un événement qui est déclenché par un nouvel élément de courrier dans une boîte aux lettres.
ms.openlocfilehash: aa562b60a7299543af8653bbc767edf329075644
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466814"
---
# <a name="newmailevent"></a><span data-ttu-id="d5365-103">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="d5365-103">NewMailEvent</span></span>

<span data-ttu-id="d5365-104">L’élément **NewMailEvent** représente un événement qui est déclenché par un nouvel élément de courrier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d5365-104">The **NewMailEvent** element represents an event that is triggered by a new mail item in a mailbox.</span></span> 
  
```xml
<NewMailEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</NewMailEvent>
```

 <span data-ttu-id="d5365-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="d5365-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5365-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d5365-106">Attributes and elements</span></span>

<span data-ttu-id="d5365-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d5365-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5365-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d5365-108">Attributes</span></span>

<span data-ttu-id="d5365-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d5365-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5365-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d5365-110">Child elements</span></span>

|<span data-ttu-id="d5365-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d5365-111">**Element**</span></span>|<span data-ttu-id="d5365-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d5365-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5365-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="d5365-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="d5365-114">Représente un signet d’événement dans la table des événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d5365-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="d5365-115">Dates</span><span class="sxs-lookup"><span data-stu-id="d5365-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="d5365-116">Représente l’horodatage de l’arrivée d’un nouvel élément de courrier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d5365-116">Represents the timestamp of the arrival of a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d5365-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="d5365-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d5365-118">Représente l’identificateur d’un nouvel élément de courrier.</span><span class="sxs-lookup"><span data-stu-id="d5365-118">Represents the identifier of a new mail item.</span></span>  <br/> |
|[<span data-ttu-id="d5365-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="d5365-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="d5365-120">Représente l’identificateur du dossier parent du nouvel élément de courrier.</span><span class="sxs-lookup"><span data-stu-id="d5365-120">Represents the identifier of the parent folder of the new mail item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5365-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d5365-121">Parent elements</span></span>

|<span data-ttu-id="d5365-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d5365-122">**Element**</span></span>|<span data-ttu-id="d5365-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="d5365-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5365-124">Notification</span><span class="sxs-lookup"><span data-stu-id="d5365-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d5365-125">Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="d5365-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d5365-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="d5365-126">Remarks</span></span>

<span data-ttu-id="d5365-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d5365-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5365-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d5365-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5365-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d5365-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d5365-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d5365-130">Schema name</span></span>  <br/> |<span data-ttu-id="d5365-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d5365-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d5365-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d5365-132">Validation file</span></span>  <br/> |<span data-ttu-id="d5365-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d5365-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d5365-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d5365-134">Can be empty</span></span>  <br/> |<span data-ttu-id="d5365-135">False</span><span class="sxs-lookup"><span data-stu-id="d5365-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5365-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d5365-136">See also</span></span>



[<span data-ttu-id="d5365-137">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="d5365-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d5365-138">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="d5365-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d5365-139">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="d5365-139">Unsubscribe operation</span></span>](unsubscribe-operation.md)

