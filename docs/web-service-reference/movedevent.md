---
title: MovedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MovedEvent
api_type:
- schema
ms.assetid: 572f8b40-dfa8-47bc-b0c1-e1a7138506fd
description: L’élément MovedEvent représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent à un autre dossier parent.
ms.openlocfilehash: 07f9c02ea194187a9fdfb1e27b19eb311392f51f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353258"
---
# <a name="movedevent"></a><span data-ttu-id="97828-103">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="97828-103">MovedEvent</span></span>

<span data-ttu-id="97828-104">L’élément **MovedEvent** représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent à un autre dossier parent.</span><span class="sxs-lookup"><span data-stu-id="97828-104">The **MovedEvent** element represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span> 
  
```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldItemId/>
   <OldParentFolderId/>
</MovedEvent>
```

```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</MovedEvent>
```


<span data-ttu-id="97828-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="97828-105">**MovedCopiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="97828-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="97828-106">Attributes and elements</span></span>

<span data-ttu-id="97828-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="97828-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97828-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="97828-108">Attributes</span></span>

<span data-ttu-id="97828-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="97828-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97828-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="97828-110">Child elements</span></span>

|<span data-ttu-id="97828-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="97828-111">**Element**</span></span>|<span data-ttu-id="97828-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="97828-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97828-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="97828-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="97828-114">Représente un signet d’événements dans la table d’événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="97828-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="97828-115">TimeStamp</span><span class="sxs-lookup"><span data-stu-id="97828-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="97828-116">Représente l’horodatage d’un événement de boîte aux lettres de dossier d’éléments de déplacement.</span><span class="sxs-lookup"><span data-stu-id="97828-116">Represents the timestamp of a move item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="97828-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="97828-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="97828-118">Représente l’identificateur du dossier déplacé.</span><span class="sxs-lookup"><span data-stu-id="97828-118">Represents the identifier of the moved folder.</span></span>  <br/> |
|[<span data-ttu-id="97828-119">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="97828-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="97828-120">Représente l’identificateur de l’élément déplacé.</span><span class="sxs-lookup"><span data-stu-id="97828-120">Represents the identifier of the moved item.</span></span>  <br/> |
|[<span data-ttu-id="97828-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="97828-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="97828-122">Représente l’identificateur du dossier qui contient l’élément déplacé ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="97828-122">Represents the identifier of the folder that contains the moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="97828-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="97828-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="97828-124">Contient l’identificateur de dossier du dossier d’origine avant qu’il a été déplacé ou copié.</span><span class="sxs-lookup"><span data-stu-id="97828-124">Contains the folder identifier of the original folder before it was moved or copied.</span></span>  <br/> |
|[<span data-ttu-id="97828-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="97828-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="97828-126">Contient l’identificateur unique de l’élément d’origine avant d’être déplacée.</span><span class="sxs-lookup"><span data-stu-id="97828-126">Contains the unique identifier of the original item before it was moved.</span></span>  <br/> |
|[<span data-ttu-id="97828-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="97828-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="97828-128">Contient l’identificateur du dossier parent d’origine d’un élément ou d’un dossier qui a été déplacé.</span><span class="sxs-lookup"><span data-stu-id="97828-128">Contains the identifier of the original parent folder of an item or folder that was moved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97828-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="97828-129">Parent elements</span></span>

|<span data-ttu-id="97828-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="97828-130">**Element**</span></span>|<span data-ttu-id="97828-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="97828-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97828-132">Notification</span><span class="sxs-lookup"><span data-stu-id="97828-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="97828-133">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="97828-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97828-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="97828-134">Remarks</span></span>

<span data-ttu-id="97828-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="97828-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97828-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="97828-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97828-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="97828-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97828-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="97828-138">Schema name</span></span>  <br/> |<span data-ttu-id="97828-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="97828-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="97828-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="97828-140">Validation file</span></span>  <br/> |<span data-ttu-id="97828-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="97828-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97828-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="97828-142">Can be empty</span></span>  <br/> |<span data-ttu-id="97828-143">False</span><span class="sxs-lookup"><span data-stu-id="97828-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97828-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="97828-144">See also</span></span>

- [<span data-ttu-id="97828-145">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="97828-145">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="97828-146">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="97828-146">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="97828-147">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="97828-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)

