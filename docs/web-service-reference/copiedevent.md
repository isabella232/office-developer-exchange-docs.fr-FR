---
title: CopiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopiedEvent
api_type:
- schema
ms.assetid: 82f2fcac-deaa-4ff8-801f-4fe28d8a19f5
description: L’élément CopiedEvent représente un événement dans lequel un élément ou un dossier est copié.
ms.openlocfilehash: 89ca9fb1fd2f4187efdec0e087d840bfee197a29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755658"
---
# <a name="copiedevent"></a><span data-ttu-id="ed1ae-103">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="ed1ae-103">CopiedEvent</span></span>

<span data-ttu-id="ed1ae-104">L’élément **CopiedEvent** représente un événement dans lequel un élément ou un dossier est copié.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-104">The **CopiedEvent** element represents an event in which an item or folder is copied.</span></span> 
  
```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

 <span data-ttu-id="ed1ae-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="ed1ae-105">**MovedCopiedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed1ae-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ed1ae-106">Attributes and elements</span></span>

<span data-ttu-id="ed1ae-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed1ae-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ed1ae-108">Attributes</span></span>

<span data-ttu-id="ed1ae-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed1ae-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ed1ae-110">Child elements</span></span>

|<span data-ttu-id="ed1ae-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ed1ae-111">**Element**</span></span>|<span data-ttu-id="ed1ae-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ed1ae-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed1ae-113">Filigrane</span><span class="sxs-lookup"><span data-stu-id="ed1ae-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="ed1ae-114">Représente un signet d’événements dans la table d’événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="ed1ae-115">Horodatage</span><span class="sxs-lookup"><span data-stu-id="ed1ae-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="ed1ae-116">Représente l’horodatage d’un événement de boîte aux lettres de dossier d’éléments de copie.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-116">Represents the timestamp of a copy item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="ed1ae-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="ed1ae-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="ed1ae-118">Représente l’identificateur du dossier.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-118">Represents the identifier of the folder.</span></span>  <br/> |
|[<span data-ttu-id="ed1ae-119">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="ed1ae-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ed1ae-120">Représente l’identificateur de l’élément.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-120">Represents the identifier of the item.</span></span>  <br/> |
|[<span data-ttu-id="ed1ae-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ed1ae-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ed1ae-122">Représente l’identificateur du dossier qui contient la copie.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-122">Represents the identifier of the folder that contains the copy.</span></span>  <br/> |
|[<span data-ttu-id="ed1ae-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="ed1ae-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="ed1ae-124">Représente l’identificateur de dossier du dossier d’origine avant qu’il a été copié.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-124">Represents the folder identifier of the original folder before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="ed1ae-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="ed1ae-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="ed1ae-126">Contient l’identificateur unique de l’élément d’origine avant qu’il a été copié.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-126">Contains the unique identifier of the original item before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="ed1ae-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ed1ae-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="ed1ae-128">Contient l’identificateur du dossier parent d’origine d’un élément ou d’un dossier qui a été copié.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-128">Contains the identifier of the original parent folder of an item or folder that was copied.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed1ae-129">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ed1ae-129">Parent elements</span></span>

|<span data-ttu-id="ed1ae-130">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ed1ae-130">**Element**</span></span>|<span data-ttu-id="ed1ae-131">**Description**</span><span class="sxs-lookup"><span data-stu-id="ed1ae-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed1ae-132">Notification</span><span class="sxs-lookup"><span data-stu-id="ed1ae-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ed1ae-133">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ed1ae-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="ed1ae-134">Remarks</span></span>

<span data-ttu-id="ed1ae-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ed1ae-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed1ae-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ed1ae-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed1ae-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ed1ae-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed1ae-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ed1ae-138">Schema name</span></span>  <br/> |<span data-ttu-id="ed1ae-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ed1ae-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="ed1ae-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ed1ae-140">Validation file</span></span>  <br/> |<span data-ttu-id="ed1ae-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ed1ae-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed1ae-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ed1ae-142">Can be empty</span></span>  <br/> |<span data-ttu-id="ed1ae-143">False</span><span class="sxs-lookup"><span data-stu-id="ed1ae-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed1ae-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ed1ae-144">See also</span></span>



[<span data-ttu-id="ed1ae-145">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="ed1ae-145">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="ed1ae-146">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="ed1ae-146">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="ed1ae-147">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="ed1ae-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="ed1ae-148">À l’aide d’abonnement</span><span class="sxs-lookup"><span data-stu-id="ed1ae-148">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="ed1ae-149">Exemple d'application de notification Push</span><span class="sxs-lookup"><span data-stu-id="ed1ae-149">Push Notification Sample Application</span></span>](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

