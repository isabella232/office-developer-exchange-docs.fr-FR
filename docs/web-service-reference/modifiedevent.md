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
description: L’élément ModifiedEvent représente un événement dans lequel un élément ou un dossier est modifié.
ms.openlocfilehash: 1a798773601a0857b9064c7fa6a532a7a36517ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468550"
---
# <a name="modifiedevent"></a><span data-ttu-id="65aaf-103">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="65aaf-103">ModifiedEvent</span></span>

<span data-ttu-id="65aaf-104">L’élément **ModifiedEvent** représente un événement dans lequel un élément ou un dossier est modifié.</span><span class="sxs-lookup"><span data-stu-id="65aaf-104">The **ModifiedEvent** element represents an event in which an item or folder is modified.</span></span> 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/> 
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

<span data-ttu-id="65aaf-105">**ModifiedEventType**</span><span class="sxs-lookup"><span data-stu-id="65aaf-105">**ModifiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="65aaf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="65aaf-106">Attributes and elements</span></span>

<span data-ttu-id="65aaf-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="65aaf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65aaf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="65aaf-108">Attributes</span></span>

<span data-ttu-id="65aaf-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="65aaf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65aaf-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="65aaf-110">Child elements</span></span>

|<span data-ttu-id="65aaf-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65aaf-111">**Element**</span></span>|<span data-ttu-id="65aaf-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="65aaf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65aaf-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="65aaf-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="65aaf-114">Représente un signet d’événement dans la table des événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="65aaf-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="65aaf-115">Dates</span><span class="sxs-lookup"><span data-stu-id="65aaf-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="65aaf-116">Représente l’horodatage d’un événement d’élément ou de boîte aux lettres de dossier modifié.</span><span class="sxs-lookup"><span data-stu-id="65aaf-116">Represents the timestamp of a modified item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="65aaf-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="65aaf-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="65aaf-118">Représente l’identificateur du dossier modifié.</span><span class="sxs-lookup"><span data-stu-id="65aaf-118">Represents the identifier of the modified folder.</span></span>  <br/> |
|[<span data-ttu-id="65aaf-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="65aaf-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="65aaf-120">Représente l’identificateur de l’élément modifié.</span><span class="sxs-lookup"><span data-stu-id="65aaf-120">Represents the identifier of the modified item.</span></span>  <br/> |
|[<span data-ttu-id="65aaf-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="65aaf-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="65aaf-122">Représente l’identificateur du dossier parent de l’élément ou du dossier modifié.</span><span class="sxs-lookup"><span data-stu-id="65aaf-122">Represents the identifier of the parent folder of the modified item or folder.</span></span>  <br/> |
|[<span data-ttu-id="65aaf-123">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="65aaf-123">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="65aaf-124">Représente le nombre d’éléments non lus dans un dossier donné.</span><span class="sxs-lookup"><span data-stu-id="65aaf-124">Represents the count of unread items within a given folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="65aaf-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="65aaf-125">Parent elements</span></span>

|<span data-ttu-id="65aaf-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65aaf-126">**Element**</span></span>|<span data-ttu-id="65aaf-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="65aaf-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65aaf-128">Notification</span><span class="sxs-lookup"><span data-stu-id="65aaf-128">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="65aaf-129">Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="65aaf-129">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="65aaf-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="65aaf-130">Remarks</span></span>

<span data-ttu-id="65aaf-131">Deux événements modifiés sont générés pour chaque modification d’un élément dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="65aaf-131">Two modified events are generated for each modification of an item in a folder.</span></span> <span data-ttu-id="65aaf-132">Un événement est pertinent pour l’élément qui a été modifié.</span><span class="sxs-lookup"><span data-stu-id="65aaf-132">One event is relevant to the item that changed.</span></span> <span data-ttu-id="65aaf-133">L’autre événement est pertinent pour le dossier parent de l’élément.</span><span class="sxs-lookup"><span data-stu-id="65aaf-133">The other event is relevant to the parent folder of the item.</span></span> <span data-ttu-id="65aaf-134">Il s’agit du même dossier que celui sur lequel l’abonnement a été créé.</span><span class="sxs-lookup"><span data-stu-id="65aaf-134">This is the same folder that the subscription was created against.</span></span> <span data-ttu-id="65aaf-135">L’événement associé au dossier est utilisé pour communiquer une modification potentielle de la propriété [UnreadCount](unreadcount.md) sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="65aaf-135">The event that is associated with the folder is used to communicate a potential change to the [UnreadCount](unreadcount.md) property on the folder.</span></span> 
  
<span data-ttu-id="65aaf-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="65aaf-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65aaf-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="65aaf-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65aaf-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="65aaf-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="65aaf-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="65aaf-139">Schema name</span></span>  <br/> |<span data-ttu-id="65aaf-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="65aaf-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="65aaf-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="65aaf-141">Validation file</span></span>  <br/> |<span data-ttu-id="65aaf-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="65aaf-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="65aaf-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="65aaf-143">Can be empty</span></span>  <br/> |<span data-ttu-id="65aaf-144">False</span><span class="sxs-lookup"><span data-stu-id="65aaf-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65aaf-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65aaf-145">See also</span></span>

- [<span data-ttu-id="65aaf-146">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="65aaf-146">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="65aaf-147">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="65aaf-147">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="65aaf-148">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="65aaf-148">Unsubscribe operation</span></span>](unsubscribe-operation.md)

