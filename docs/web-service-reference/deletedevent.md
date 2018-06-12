---
title: DeletedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedEvent
api_type:
- schema
ms.assetid: c4565eb4-b537-466c-b1ff-11602533812b
description: L’élément DeletedEvent représente un événement dans lequel un élément ou un dossier est supprimé.
ms.openlocfilehash: f06ca0727916f415c648e876f88bf7eacef5a5ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755853"
---
# <a name="deletedevent"></a><span data-ttu-id="4301a-103">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="4301a-103">DeletedEvent</span></span>

<span data-ttu-id="4301a-104">L’élément **DeletedEvent** représente un événement dans lequel un élément ou un dossier est supprimé.</span><span class="sxs-lookup"><span data-stu-id="4301a-104">The **DeletedEvent** element represents an event in which an item or folder is deleted.</span></span> 
  
```xml
<DeletedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</DeletedEvent>
```

<span data-ttu-id="4301a-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="4301a-105">**BaseObjectChangedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4301a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4301a-106">Attributes and elements</span></span>

<span data-ttu-id="4301a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4301a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4301a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4301a-108">Attributes</span></span>

<span data-ttu-id="4301a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4301a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4301a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4301a-110">Child elements</span></span>

|<span data-ttu-id="4301a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4301a-111">**Element**</span></span>|<span data-ttu-id="4301a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4301a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4301a-113">Filigrane</span><span class="sxs-lookup"><span data-stu-id="4301a-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="4301a-114">Représente un signet d’événements dans la table d’événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4301a-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="4301a-115">Horodatage</span><span class="sxs-lookup"><span data-stu-id="4301a-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="4301a-116">Représente l’horodatage d’un événement de boîte aux lettres supprimé élément ou un dossier.</span><span class="sxs-lookup"><span data-stu-id="4301a-116">Represents the timestamp of a deleted item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="4301a-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="4301a-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="4301a-118">Représente l’identificateur du dossier supprimé.</span><span class="sxs-lookup"><span data-stu-id="4301a-118">Represents the identifier of the deleted folder.</span></span>  <br/> |
|[<span data-ttu-id="4301a-119">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="4301a-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="4301a-120">Représente l’identificateur de l’élément supprimé.</span><span class="sxs-lookup"><span data-stu-id="4301a-120">Represents the identifier of the deleted item.</span></span>  <br/> |
|[<span data-ttu-id="4301a-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="4301a-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="4301a-122">Représente l’identificateur du dossier parent de l’élément supprimé ou du dossier avant la suppression.</span><span class="sxs-lookup"><span data-stu-id="4301a-122">Represents the identifier of the parent folder of the deleted item or folder before deletion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4301a-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4301a-123">Parent elements</span></span>

|<span data-ttu-id="4301a-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4301a-124">**Element**</span></span>|<span data-ttu-id="4301a-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="4301a-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4301a-126">Notification</span><span class="sxs-lookup"><span data-stu-id="4301a-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="4301a-127">Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="4301a-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4301a-128">Note</span><span class="sxs-lookup"><span data-stu-id="4301a-128">Remarks</span></span>

<span data-ttu-id="4301a-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4301a-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4301a-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4301a-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4301a-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4301a-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4301a-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4301a-132">Schema name</span></span>  <br/> |<span data-ttu-id="4301a-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4301a-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="4301a-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4301a-134">Validation file</span></span>  <br/> |<span data-ttu-id="4301a-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4301a-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4301a-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4301a-136">Can be empty</span></span>  <br/> |<span data-ttu-id="4301a-137">False</span><span class="sxs-lookup"><span data-stu-id="4301a-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4301a-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4301a-138">See also</span></span>

- [<span data-ttu-id="4301a-139">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="4301a-139">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="4301a-140">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="4301a-140">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="4301a-141">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="4301a-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)

