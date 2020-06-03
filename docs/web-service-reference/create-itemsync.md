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
description: L’élément Create identifie un élément unique à créer dans le magasin client local.
ms.openlocfilehash: b9c0f28333594a6c17ee9581a227fc4773874fd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460798"
---
# <a name="create-itemsync"></a><span data-ttu-id="0fb53-103">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="0fb53-103">Create (ItemSync)</span></span>

<span data-ttu-id="0fb53-104">L’élément **Create** identifie un élément unique à créer dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="0fb53-104">The **Create** element identifies a single item to create in the local client store.</span></span> 
  
- [<span data-ttu-id="0fb53-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="0fb53-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="0fb53-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0fb53-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="0fb53-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0fb53-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) 
- [<span data-ttu-id="0fb53-108">Changes (éléments)</span><span class="sxs-lookup"><span data-stu-id="0fb53-108">Changes (Items)</span></span>](changes-items.md) 
- [<span data-ttu-id="0fb53-109">Créer (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="0fb53-109">Create (ItemSync)</span></span>](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

```xml
<Create>
   <Task/> 
</Create>
```

```xml
<Create>
   <MeetingResponse/>
</Create>
```

```xml
<Create>
   <CalendarItem/>
</Create>
```

```xml
<Create>
   <MeetingMessage/>
</Create>
```

```xml
<Create>
   <DistributionList/>
</Create>
```

```xml
<Create>
   <MeetingCancellation/>
</Create>
```

```xml
<Create>
   <MeetingRequest/> 
</Create>
```

```xml
<Create>
   <Message/> 
</Create>
```

```xml
<Create>
   <Contact/> 
</Create>
```

<span data-ttu-id="0fb53-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="0fb53-110">**SyncFolderItemsCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0fb53-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0fb53-111">Attributes and elements</span></span>

<span data-ttu-id="0fb53-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0fb53-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0fb53-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="0fb53-113">Attributes</span></span>

<span data-ttu-id="0fb53-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0fb53-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0fb53-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0fb53-115">Child elements</span></span>

|<span data-ttu-id="0fb53-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0fb53-116">**Element**</span></span>|<span data-ttu-id="0fb53-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="0fb53-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fb53-118">Item</span><span class="sxs-lookup"><span data-stu-id="0fb53-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="0fb53-119">Représente un élément Exchange générique à créer.</span><span class="sxs-lookup"><span data-stu-id="0fb53-119">Represents a generic Exchange item to create.</span></span>  <br/> |
|[<span data-ttu-id="0fb53-120">Message</span><span class="sxs-lookup"><span data-stu-id="0fb53-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0fb53-121">Représente un message électronique Exchange à créer.</span><span class="sxs-lookup"><span data-stu-id="0fb53-121">Represents an Exchange e-mail message to create.</span></span>  <br/> |
|[<span data-ttu-id="0fb53-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="0fb53-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="0fb53-123">Représente un élément de calendrier Exchange à créer.</span><span class="sxs-lookup"><span data-stu-id="0fb53-123">Represents an Exchange calendar item to create.</span></span>  <br/> |
|[<span data-ttu-id="0fb53-124">Contact</span><span class="sxs-lookup"><span data-stu-id="0fb53-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="0fb53-125">Représente un élément de contact Exchange à créer.</span><span class="sxs-lookup"><span data-stu-id="0fb53-125">Represents an Exchange contact item to create.</span></span>  <br/> |
|[<span data-ttu-id="0fb53-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="0fb53-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="0fb53-127">Représente une liste de distribution à créer.</span><span class="sxs-lookup"><span data-stu-id="0fb53-127">Represents a distribution list to create.</span></span>  <br/> |
|[<span data-ttu-id="0fb53-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="0fb53-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="0fb53-129">Représente un message de réunion à créer.</span><span class="sxs-lookup"><span data-stu-id="0fb53-129">Represents a meeting message to create.</span></span>  <br/> |
|[<span data-ttu-id="0fb53-130">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="0fb53-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0fb53-131">Représente une demande de réunion à créer.</span><span class="sxs-lookup"><span data-stu-id="0fb53-131">Represents a meeting request to create.</span></span>  <br/> |
|[<span data-ttu-id="0fb53-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="0fb53-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0fb53-133">Représente une réponse à une réunion à créer.</span><span class="sxs-lookup"><span data-stu-id="0fb53-133">Represents a meeting response to create.</span></span>  <br/> |
|[<span data-ttu-id="0fb53-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="0fb53-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0fb53-135">Représente une annulation de réunion à créer.</span><span class="sxs-lookup"><span data-stu-id="0fb53-135">Represents a meeting cancellation to create.</span></span>  <br/> |
|[<span data-ttu-id="0fb53-136">Task</span><span class="sxs-lookup"><span data-stu-id="0fb53-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="0fb53-137">Représente une tâche à créer.</span><span class="sxs-lookup"><span data-stu-id="0fb53-137">Represents a task to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0fb53-138">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0fb53-138">Parent elements</span></span>

|<span data-ttu-id="0fb53-139">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0fb53-139">**Element**</span></span>|<span data-ttu-id="0fb53-140">**Description**</span><span class="sxs-lookup"><span data-stu-id="0fb53-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0fb53-141">Changes (éléments)</span><span class="sxs-lookup"><span data-stu-id="0fb53-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="0fb53-142">Contient un tableau de séquence de types de modifications qui représentent les types de différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="0fb53-142">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0fb53-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="0fb53-143">Remarks</span></span>

<span data-ttu-id="0fb53-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0fb53-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0fb53-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0fb53-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0fb53-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0fb53-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0fb53-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0fb53-147">Schema name</span></span>  <br/> |<span data-ttu-id="0fb53-148">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0fb53-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="0fb53-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0fb53-149">Validation file</span></span>  <br/> |<span data-ttu-id="0fb53-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0fb53-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0fb53-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0fb53-151">Can be empty</span></span>  <br/> |<span data-ttu-id="0fb53-152">False</span><span class="sxs-lookup"><span data-stu-id="0fb53-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0fb53-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0fb53-153">See also</span></span>

- [<span data-ttu-id="0fb53-154">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0fb53-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="0fb53-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0fb53-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

