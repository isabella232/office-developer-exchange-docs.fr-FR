---
title: ModifiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedEvent
api_type:
- schema
ms.assetid: ca1309f4-2df7-4289-811c-75c3db0e7072
description: L’élément ModifiedEvent représente un événement auquel un élément ou un dossier est modifiée.
ms.openlocfilehash: fb464fb0a270d8ca7d33d40e5425e260970b2f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828482"
---
# <a name="modifiedevent"></a><span data-ttu-id="5dfda-103">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="5dfda-103">ModifiedEvent</span></span>

<span data-ttu-id="5dfda-104">L’élément **ModifiedEvent** représente un événement auquel un élément ou un dossier est modifiée.</span><span class="sxs-lookup"><span data-stu-id="5dfda-104">The **ModifiedEvent** element represents an event in which an item or folder is modified.</span></span> 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

 <span data-ttu-id="5dfda-105">**ModifiedEventType**</span><span class="sxs-lookup"><span data-stu-id="5dfda-105">**ModifiedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5dfda-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5dfda-106">Attributes and elements</span></span>

<span data-ttu-id="5dfda-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5dfda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5dfda-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5dfda-108">Attributes</span></span>

<span data-ttu-id="5dfda-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5dfda-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5dfda-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5dfda-110">Child elements</span></span>

|<span data-ttu-id="5dfda-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5dfda-111">**Element**</span></span>|<span data-ttu-id="5dfda-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="5dfda-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5dfda-113">Filigrane</span><span class="sxs-lookup"><span data-stu-id="5dfda-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="5dfda-114">Représente un signet d’événements dans la table d’événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5dfda-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="5dfda-115">Horodatage</span><span class="sxs-lookup"><span data-stu-id="5dfda-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="5dfda-116">Représente l’horodatage d’un événement de boîte aux lettres élément ou le dossier modifié.</span><span class="sxs-lookup"><span data-stu-id="5dfda-116">Represents the timestamp of a modified item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="5dfda-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="5dfda-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="5dfda-118">Représente l’identificateur du dossier modifié.</span><span class="sxs-lookup"><span data-stu-id="5dfda-118">Represents the identifier of the modified folder.</span></span>  <br/> |
|[<span data-ttu-id="5dfda-119">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="5dfda-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="5dfda-120">Représente l’identificateur de l’élément modifié.</span><span class="sxs-lookup"><span data-stu-id="5dfda-120">Represents the identifier of the modified item.</span></span>  <br/> |
|[<span data-ttu-id="5dfda-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="5dfda-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="5dfda-122">Représente l’identificateur du dossier parent de l’élément modifié ou d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="5dfda-122">Represents the identifier of the parent folder of the modified item or folder.</span></span>  <br/> |
|[<span data-ttu-id="5dfda-123">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="5dfda-123">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="5dfda-124">Représente le nombre d’éléments non lus dans un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="5dfda-124">Represents the count of unread items within a given folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5dfda-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5dfda-125">Parent elements</span></span>

|<span data-ttu-id="5dfda-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5dfda-126">**Element**</span></span>|<span data-ttu-id="5dfda-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="5dfda-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5dfda-128">Notification</span><span class="sxs-lookup"><span data-stu-id="5dfda-128">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5dfda-129">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="5dfda-129">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5dfda-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="5dfda-130">Remarks</span></span>

<span data-ttu-id="5dfda-131">Deux événements modifiés sont générés pour chaque modification d’un élément dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="5dfda-131">Two modified events are generated for each modification of an item in a folder.</span></span> <span data-ttu-id="5dfda-132">Un événement s’applique à l’élément qui a été modifié.</span><span class="sxs-lookup"><span data-stu-id="5dfda-132">One event is relevant to the item that changed.</span></span> <span data-ttu-id="5dfda-133">L’événement est pertinent pour le dossier parent de l’élément.</span><span class="sxs-lookup"><span data-stu-id="5dfda-133">The other event is relevant to the parent folder of the item.</span></span> <span data-ttu-id="5dfda-134">Voici le même dossier que l’abonnement a été créé par rapport à.</span><span class="sxs-lookup"><span data-stu-id="5dfda-134">This is the same folder that the subscription was created against.</span></span> <span data-ttu-id="5dfda-135">L’événement qui est associé au dossier est utilisé pour communiquer une modification à la propriété [UnreadCount](unreadcount.md) sur le dossier potentielle.</span><span class="sxs-lookup"><span data-stu-id="5dfda-135">The event that is associated with the folder is used to communicate a potential change to the [UnreadCount](unreadcount.md) property on the folder.</span></span> 
  
<span data-ttu-id="5dfda-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5dfda-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5dfda-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5dfda-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5dfda-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5dfda-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5dfda-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5dfda-139">Schema name</span></span>  <br/> |<span data-ttu-id="5dfda-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5dfda-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="5dfda-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5dfda-141">Validation file</span></span>  <br/> |<span data-ttu-id="5dfda-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5dfda-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5dfda-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5dfda-143">Can be empty</span></span>  <br/> |<span data-ttu-id="5dfda-144">False</span><span class="sxs-lookup"><span data-stu-id="5dfda-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5dfda-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5dfda-145">See also</span></span>



[<span data-ttu-id="5dfda-146">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="5dfda-146">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="5dfda-147">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="5dfda-147">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="5dfda-148">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="5dfda-148">Unsubscribe operation</span></span>](unsubscribe-operation.md)

