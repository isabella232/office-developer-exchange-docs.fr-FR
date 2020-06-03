---
title: CreatedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreatedEvent
api_type:
- schema
ms.assetid: f0e53a53-c352-42a5-8280-cd808b0e961b
description: L’élément CreatedEvent représente un événement dans lequel un élément ou un dossier est créé.
ms.openlocfilehash: 546dde782b3b20cd76acb625067b5f2d8f568854
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44445320"
---
# <a name="createdevent"></a><span data-ttu-id="24f08-103">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="24f08-103">CreatedEvent</span></span>

<span data-ttu-id="24f08-104">L’élément **CreatedEvent** représente un événement dans lequel un élément ou un dossier est créé.</span><span class="sxs-lookup"><span data-stu-id="24f08-104">The **CreatedEvent** element represents an event in which an item or folder is created.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
</CreatedEvent>
```

<span data-ttu-id="24f08-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="24f08-105">**BaseObjectChangedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="24f08-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="24f08-106">Attributes and elements</span></span>

<span data-ttu-id="24f08-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="24f08-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24f08-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="24f08-108">Attributes</span></span>

<span data-ttu-id="24f08-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="24f08-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24f08-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="24f08-110">Child elements</span></span>

|<span data-ttu-id="24f08-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="24f08-111">**Element**</span></span>|<span data-ttu-id="24f08-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="24f08-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24f08-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="24f08-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="24f08-114">Représente un signet d’événement dans la table des événements de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="24f08-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="24f08-115">Dates</span><span class="sxs-lookup"><span data-stu-id="24f08-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="24f08-116">Représente l’horodatage d’un événement de boîte aux lettres d’élément ou de dossier créé.</span><span class="sxs-lookup"><span data-stu-id="24f08-116">Represents the timestamp of a created item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="24f08-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="24f08-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="24f08-118">Représente l’identificateur du dossier créé.</span><span class="sxs-lookup"><span data-stu-id="24f08-118">Represents the identifier of the created folder.</span></span>  <br/> |
|[<span data-ttu-id="24f08-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="24f08-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="24f08-120">Représente l’identificateur de l’élément créé.</span><span class="sxs-lookup"><span data-stu-id="24f08-120">Represents the identifier of the created item.</span></span>  <br/> |
|[<span data-ttu-id="24f08-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="24f08-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="24f08-122">Représente l’identificateur du dossier parent de l’élément ou du dossier créé.</span><span class="sxs-lookup"><span data-stu-id="24f08-122">Represents the identifier of the parent folder of the created item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24f08-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="24f08-123">Parent elements</span></span>

|<span data-ttu-id="24f08-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="24f08-124">**Element**</span></span>|<span data-ttu-id="24f08-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="24f08-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24f08-126">Notification</span><span class="sxs-lookup"><span data-stu-id="24f08-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="24f08-127">Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.</span><span class="sxs-lookup"><span data-stu-id="24f08-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="24f08-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="24f08-128">Remarks</span></span>

<span data-ttu-id="24f08-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="24f08-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24f08-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="24f08-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24f08-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="24f08-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="24f08-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="24f08-132">Schema name</span></span>  <br/> |<span data-ttu-id="24f08-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="24f08-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="24f08-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="24f08-134">Validation file</span></span>  <br/> |<span data-ttu-id="24f08-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="24f08-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="24f08-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="24f08-136">Can be empty</span></span>  <br/> |<span data-ttu-id="24f08-137">False</span><span class="sxs-lookup"><span data-stu-id="24f08-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24f08-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="24f08-138">See also</span></span>

- [<span data-ttu-id="24f08-139">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="24f08-139">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="24f08-140">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="24f08-140">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="24f08-141">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="24f08-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="24f08-142">Utilisation des abonnements extraits</span><span class="sxs-lookup"><span data-stu-id="24f08-142">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [<span data-ttu-id="24f08-143">Notifications d’événements dans EWS</span><span class="sxs-lookup"><span data-stu-id="24f08-143">Event notifications in EWS</span></span>](https://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

