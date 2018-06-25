---
title: Mise à jour (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 4e204446-1c80-44f9-b93b-77ce630a01a5
description: L’élément de mise à jour identifie un seul élément à mettre à jour dans le magasin de client local.
ms.openlocfilehash: ef1bd46906152affbe54372472766afc2a6ae8c1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838851"
---
# <a name="update-itemsync"></a><span data-ttu-id="4df08-103">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="4df08-103">Update (ItemSync)</span></span>

<span data-ttu-id="4df08-104">L’élément **Update** identifie un élément unique pour mettre à jour dans le magasin de client local.</span><span class="sxs-lookup"><span data-stu-id="4df08-104">The **Update** element identifies a single item to update in the local client store.</span></span> 
  
[<span data-ttu-id="4df08-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="4df08-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md)
  
[<span data-ttu-id="4df08-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4df08-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="4df08-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4df08-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
[<span data-ttu-id="4df08-108">Modifications (éléments)</span><span class="sxs-lookup"><span data-stu-id="4df08-108">Changes (Items)</span></span>](changes-items.md)
  
[<span data-ttu-id="4df08-109">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="4df08-109">Update (ItemSync)</span></span>](update-itemsync.md)
  
```xml
<Update>
   <Item/>
</Update>
```

 <span data-ttu-id="4df08-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="4df08-110">**SyncFolderItemsCreateOrUpdateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4df08-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4df08-111">Attributes and elements</span></span>

<span data-ttu-id="4df08-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4df08-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4df08-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="4df08-113">Attributes</span></span>

<span data-ttu-id="4df08-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4df08-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4df08-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4df08-115">Child elements</span></span>

|<span data-ttu-id="4df08-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4df08-116">**Element**</span></span>|<span data-ttu-id="4df08-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="4df08-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4df08-118">Item</span><span class="sxs-lookup"><span data-stu-id="4df08-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="4df08-119">Représente un élément Exchange générique pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="4df08-119">Represents a generic Exchange item to update.</span></span>  <br/> |
|[<span data-ttu-id="4df08-120">Message</span><span class="sxs-lookup"><span data-stu-id="4df08-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4df08-121">Représente un message électronique d’Exchange pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="4df08-121">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="4df08-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="4df08-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="4df08-123">Représente un élément de calendrier Exchange pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="4df08-123">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="4df08-124">Contact</span><span class="sxs-lookup"><span data-stu-id="4df08-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="4df08-125">Représente un élément de contact Exchange pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="4df08-125">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="4df08-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="4df08-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="4df08-127">Représente une liste de distribution pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="4df08-127">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="4df08-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="4df08-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="4df08-129">Représente un message de réunion pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="4df08-129">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="4df08-130">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="4df08-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="4df08-131">Représente une demande de réunion pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="4df08-131">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="4df08-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="4df08-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="4df08-133">Représente une réponse à une réunion à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="4df08-133">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="4df08-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="4df08-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="4df08-135">Représente une annulation de réunion pour mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="4df08-135">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="4df08-136">Tâche</span><span class="sxs-lookup"><span data-stu-id="4df08-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="4df08-137">Représente une tâche à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="4df08-137">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4df08-138">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4df08-138">Parent elements</span></span>

|<span data-ttu-id="4df08-139">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4df08-139">**Element**</span></span>|<span data-ttu-id="4df08-140">**Description**</span><span class="sxs-lookup"><span data-stu-id="4df08-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4df08-141">Modifications (éléments)</span><span class="sxs-lookup"><span data-stu-id="4df08-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="4df08-142">Contient un tableau de séquence de types de modification qui représente le type des différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="4df08-142">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4df08-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="4df08-143">Remarks</span></span>

<span data-ttu-id="4df08-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4df08-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4df08-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4df08-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4df08-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4df08-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4df08-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4df08-147">Schema name</span></span>  <br/> |<span data-ttu-id="4df08-148">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4df08-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="4df08-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4df08-149">Validation file</span></span>  <br/> |<span data-ttu-id="4df08-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4df08-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4df08-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4df08-151">Can be empty</span></span>  <br/> |<span data-ttu-id="4df08-152">False</span><span class="sxs-lookup"><span data-stu-id="4df08-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4df08-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4df08-153">See also</span></span>



[<span data-ttu-id="4df08-154">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="4df08-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="4df08-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4df08-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

