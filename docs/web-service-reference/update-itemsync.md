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
description: L’élément Update identifie un élément unique à mettre à jour dans le magasin client local.
ms.openlocfilehash: 12248cbbd5d47a19e36d49fcebe6d4753a2e162f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468886"
---
# <a name="update-itemsync"></a><span data-ttu-id="b89ee-103">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="b89ee-103">Update (ItemSync)</span></span>

<span data-ttu-id="b89ee-104">L’élément **Update** identifie un élément unique à mettre à jour dans le magasin client local.</span><span class="sxs-lookup"><span data-stu-id="b89ee-104">The **Update** element identifies a single item to update in the local client store.</span></span> 
  
- [<span data-ttu-id="b89ee-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="b89ee-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="b89ee-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b89ee-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="b89ee-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b89ee-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="b89ee-108">Changes (éléments)</span><span class="sxs-lookup"><span data-stu-id="b89ee-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="b89ee-109">Mise à jour (ItemSync)</span><span class="sxs-lookup"><span data-stu-id="b89ee-109">Update (ItemSync)</span></span>](update-itemsync.md)
  
```xml
<Update>
   <Item/>
</Update>
```

```xml
<Update>
   <MeetingRequest/>
</Update>
```

```xml
<Update>
   <MeetingCancellation/>
</Update>
```

```xml
<Update>
   <Task/>
</Update>
```

```xml
<Update>
   <CalendarItem/>
</Update>
```

```xml
<Update>
   <MeetingResponse/>
</Update>
```

```xml
<Update>
   <Message/>
</Update>
```

```xml
<Update>
   <DistributionList/>
</Update>
```

```xml
<Update>
   <MeetingMessage/>
</Update>
```

```xml
<Update>
   <Contact/> 
</Update>
```

<span data-ttu-id="b89ee-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="b89ee-110">**SyncFolderItemsCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b89ee-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b89ee-111">Attributes and elements</span></span>

<span data-ttu-id="b89ee-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b89ee-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b89ee-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="b89ee-113">Attributes</span></span>

<span data-ttu-id="b89ee-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b89ee-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b89ee-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b89ee-115">Child elements</span></span>

|<span data-ttu-id="b89ee-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b89ee-116">**Element**</span></span>|<span data-ttu-id="b89ee-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="b89ee-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b89ee-118">Item</span><span class="sxs-lookup"><span data-stu-id="b89ee-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="b89ee-119">Représente un élément Exchange générique à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="b89ee-119">Represents a generic Exchange item to update.</span></span>  <br/> |
|[<span data-ttu-id="b89ee-120">Message</span><span class="sxs-lookup"><span data-stu-id="b89ee-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b89ee-121">Représente un message électronique Exchange à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="b89ee-121">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="b89ee-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="b89ee-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b89ee-123">Représente un élément de calendrier Exchange à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="b89ee-123">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="b89ee-124">Contact</span><span class="sxs-lookup"><span data-stu-id="b89ee-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b89ee-125">Représente un contact Exchange à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="b89ee-125">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="b89ee-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="b89ee-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="b89ee-127">Représente une liste de distribution à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="b89ee-127">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="b89ee-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b89ee-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b89ee-129">Représente un message de réunion à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="b89ee-129">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="b89ee-130">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="b89ee-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b89ee-131">Représente une demande de réunion à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="b89ee-131">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="b89ee-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b89ee-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b89ee-133">Représente une réponse à une réunion à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="b89ee-133">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="b89ee-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b89ee-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b89ee-135">Représente une annulation de réunion à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="b89ee-135">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="b89ee-136">Task</span><span class="sxs-lookup"><span data-stu-id="b89ee-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="b89ee-137">Représente une tâche à mettre à jour.</span><span class="sxs-lookup"><span data-stu-id="b89ee-137">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b89ee-138">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b89ee-138">Parent elements</span></span>

|<span data-ttu-id="b89ee-139">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b89ee-139">**Element**</span></span>|<span data-ttu-id="b89ee-140">**Description**</span><span class="sxs-lookup"><span data-stu-id="b89ee-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b89ee-141">Changes (éléments)</span><span class="sxs-lookup"><span data-stu-id="b89ee-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="b89ee-142">Contient un tableau de séquence de types de modifications qui représentent le type de différences entre les éléments sur le client et les éléments sur le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="b89ee-142">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b89ee-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="b89ee-143">Remarks</span></span>

<span data-ttu-id="b89ee-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b89ee-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b89ee-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b89ee-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b89ee-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b89ee-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b89ee-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b89ee-147">Schema name</span></span>  <br/> |<span data-ttu-id="b89ee-148">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b89ee-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="b89ee-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b89ee-149">Validation file</span></span>  <br/> |<span data-ttu-id="b89ee-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b89ee-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b89ee-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b89ee-151">Can be empty</span></span>  <br/> |<span data-ttu-id="b89ee-152">False</span><span class="sxs-lookup"><span data-stu-id="b89ee-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b89ee-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b89ee-153">See also</span></span>

- [<span data-ttu-id="b89ee-154">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="b89ee-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="b89ee-155">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b89ee-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

