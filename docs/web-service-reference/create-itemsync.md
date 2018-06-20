---
title: Créer (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: L’élément créer identifie un élément unique à créer dans le magasin du client local.
ms.openlocfilehash: 39056bcaab3577b1b729421118a45571910922fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755679"
---
# <a name="create-itemsync"></a><span data-ttu-id="31a42-103">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="31a42-103">Create (ItemSync)</span></span>

<span data-ttu-id="31a42-104">L’élément **créer** identifie un élément unique à créer dans le magasin du client local.</span><span class="sxs-lookup"><span data-stu-id="31a42-104">The **Create** element identifies a single item to create in the local client store.</span></span> 
  
[<span data-ttu-id="31a42-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="31a42-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="31a42-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="31a42-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="31a42-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="31a42-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="31a42-108">Modifications (éléments)</span><span class="sxs-lookup"><span data-stu-id="31a42-108">Changes (Items)</span></span>](changes-items.md)
  
[<span data-ttu-id="31a42-109">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="31a42-109">Create (ItemSync)</span></span>](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

 <span data-ttu-id="31a42-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="31a42-110">**SyncFolderItemsCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31a42-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="31a42-111">Attributes and elements</span></span>

<span data-ttu-id="31a42-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="31a42-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31a42-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="31a42-113">Attributes</span></span>

<span data-ttu-id="31a42-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="31a42-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31a42-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="31a42-115">Child elements</span></span>

|<span data-ttu-id="31a42-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="31a42-116">**Element**</span></span>|<span data-ttu-id="31a42-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="31a42-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31a42-118">Item</span><span class="sxs-lookup"><span data-stu-id="31a42-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="31a42-119">Représente un élément Exchange générique à créer.</span><span class="sxs-lookup"><span data-stu-id="31a42-119">Represents a generic Exchange item to create.</span></span>  <br/> |
|[<span data-ttu-id="31a42-120">Message</span><span class="sxs-lookup"><span data-stu-id="31a42-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="31a42-121">Représente un message électronique d’Exchange à créer.</span><span class="sxs-lookup"><span data-stu-id="31a42-121">Represents an Exchange e-mail message to create.</span></span>  <br/> |
|[<span data-ttu-id="31a42-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="31a42-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="31a42-123">Représente un élément de calendrier Exchange à créer.</span><span class="sxs-lookup"><span data-stu-id="31a42-123">Represents an Exchange calendar item to create.</span></span>  <br/> |
|[<span data-ttu-id="31a42-124">Contact</span><span class="sxs-lookup"><span data-stu-id="31a42-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="31a42-125">Représente un élément de contact Exchange à créer.</span><span class="sxs-lookup"><span data-stu-id="31a42-125">Represents an Exchange contact item to create.</span></span>  <br/> |
|[<span data-ttu-id="31a42-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="31a42-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="31a42-127">Représente une liste de distribution à créer.</span><span class="sxs-lookup"><span data-stu-id="31a42-127">Represents a distribution list to create.</span></span>  <br/> |
|[<span data-ttu-id="31a42-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="31a42-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="31a42-129">Représente un message de réunion à créer.</span><span class="sxs-lookup"><span data-stu-id="31a42-129">Represents a meeting message to create.</span></span>  <br/> |
|[<span data-ttu-id="31a42-130">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="31a42-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="31a42-131">Représente une demande de réunion à créer.</span><span class="sxs-lookup"><span data-stu-id="31a42-131">Represents a meeting request to create.</span></span>  <br/> |
|[<span data-ttu-id="31a42-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="31a42-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="31a42-133">Représente une réponse à une réunion à créer.</span><span class="sxs-lookup"><span data-stu-id="31a42-133">Represents a meeting response to create.</span></span>  <br/> |
|[<span data-ttu-id="31a42-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="31a42-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="31a42-135">Représente une annulation de réunion à créer.</span><span class="sxs-lookup"><span data-stu-id="31a42-135">Represents a meeting cancellation to create.</span></span>  <br/> |
|[<span data-ttu-id="31a42-136">Tâche</span><span class="sxs-lookup"><span data-stu-id="31a42-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="31a42-137">Représente une tâche à créer.</span><span class="sxs-lookup"><span data-stu-id="31a42-137">Represents a task to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="31a42-138">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="31a42-138">Parent elements</span></span>

|<span data-ttu-id="31a42-139">**Élément**</span><span class="sxs-lookup"><span data-stu-id="31a42-139">**Element**</span></span>|<span data-ttu-id="31a42-140">**Description**</span><span class="sxs-lookup"><span data-stu-id="31a42-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31a42-141">Modifications (éléments)</span><span class="sxs-lookup"><span data-stu-id="31a42-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="31a42-142">Contient un tableau de séquence de types de modification qui représentent les types de différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="31a42-142">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="31a42-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="31a42-143">Remarks</span></span>

<span data-ttu-id="31a42-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="31a42-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31a42-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="31a42-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31a42-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="31a42-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31a42-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="31a42-147">Schema name</span></span>  <br/> |<span data-ttu-id="31a42-148">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="31a42-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="31a42-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="31a42-149">Validation file</span></span>  <br/> |<span data-ttu-id="31a42-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="31a42-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="31a42-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="31a42-151">Can be empty</span></span>  <br/> |<span data-ttu-id="31a42-152">False</span><span class="sxs-lookup"><span data-stu-id="31a42-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31a42-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="31a42-153">See also</span></span>



[<span data-ttu-id="31a42-154">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="31a42-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="31a42-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="31a42-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

