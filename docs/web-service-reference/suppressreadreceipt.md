---
title: SuppressReadReceipt
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuppressReadReceipt
api_type:
- schema
ms.assetid: fc09bcc2-c003-4322-8315-d929bd0a9e2e
description: L’élément SuppressReadReceipt est utilisé pour supprimer des confirmations de lecture.
ms.openlocfilehash: b6b4fe5db26195882a7def5cac8266a942def996
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455953"
---
# <a name="suppressreadreceipt"></a><span data-ttu-id="caa64-103">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="caa64-103">SuppressReadReceipt</span></span>

<span data-ttu-id="caa64-104">L’élément **SuppressReadReceipt** est utilisé pour supprimer des confirmations de lecture.</span><span class="sxs-lookup"><span data-stu-id="caa64-104">The **SuppressReadReceipt** element is used to suppress read receipts.</span></span> 
  
```xml
<SuppressReadReceipt>
   <ReferenceItemId/>
</SuppressReadReceipt>
```

 <span data-ttu-id="caa64-105">**SuppressReadReceiptType**</span><span class="sxs-lookup"><span data-stu-id="caa64-105">**SuppressReadReceiptType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="caa64-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="caa64-106">Attributes and elements</span></span>

<span data-ttu-id="caa64-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="caa64-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="caa64-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="caa64-108">Attributes</span></span>

<span data-ttu-id="caa64-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="caa64-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="caa64-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="caa64-110">Child elements</span></span>

|<span data-ttu-id="caa64-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="caa64-111">**Element**</span></span>|<span data-ttu-id="caa64-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="caa64-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="caa64-113">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="caa64-113">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="caa64-114">Identifie l’élément auquel l’objet de réponse fait référence.</span><span class="sxs-lookup"><span data-stu-id="caa64-114">Identifies the item to which the response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="caa64-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="caa64-115">Parent elements</span></span>

|<span data-ttu-id="caa64-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="caa64-116">**Element**</span></span>|<span data-ttu-id="caa64-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="caa64-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="caa64-118">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="caa64-118">AdjacentMeetings</span></span>](adjacentmeetings.md) <br/> | <span data-ttu-id="caa64-119">Décrit tous les éléments adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="caa64-119">Describes all items that are adjacent to a meeting time.</span></span>  <br/><br/>  <span data-ttu-id="caa64-120">Voici quelques-unes des expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="caa64-120">The following are some of the XPath expressions to this element:</span></span><br/>  <br/>  `/CalendarItem/AdjacentMeetings` <br/>  `/MeetingRequest/AdjacentMeetings` <br/>  `/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/AdjacentMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/AdjacentMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/AdjacentMeetings` <br/> |
|[<span data-ttu-id="caa64-121">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="caa64-121">ConflictingMeetings</span></span>](conflictingmeetings.md) <br/> | <span data-ttu-id="caa64-122">Décrit tous les éléments qui sont en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="caa64-122">Describes all items that conflict with a meeting time.</span></span> <br/> <br/>  <span data-ttu-id="caa64-123">Voici quelques-unes des expressions XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="caa64-123">The following are some of the XPath expressions to this element:</span></span> <br/> <br/>  `/CalendarItem/ConflictingMeetings` <br/>  `/MeetingRequest/ConflictingMeetings` <br/>  `/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/AcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/DeclineItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/TentativelyAcceptItem/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/SetItemField/CalendarItem/ConflictingMeetings` <br/>  `/UpdateItem/ItemChanges/ItemChange/Updates/AppendToItemField/CalendarItem/ConflictingMeetings` <br/>  `/CreateAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/>  `/GetAttachmentResponseMessage/Attachments/ItemAttachment/CalendarItem/ConflictingMeetings` <br/> |
|[<span data-ttu-id="caa64-124">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="caa64-124">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="caa64-125">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="caa64-125">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="caa64-126">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="caa64-126">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="caa64-127">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="caa64-127">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="caa64-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="caa64-128">Remarks</span></span>

<span data-ttu-id="caa64-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="caa64-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="caa64-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="caa64-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="caa64-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="caa64-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="caa64-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="caa64-132">Schema Name</span></span>  <br/> |<span data-ttu-id="caa64-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="caa64-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="caa64-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="caa64-134">Validation File</span></span>  <br/> |<span data-ttu-id="caa64-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="caa64-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="caa64-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="caa64-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="caa64-137">False</span><span class="sxs-lookup"><span data-stu-id="caa64-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="caa64-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="caa64-138">See also</span></span>

- [<span data-ttu-id="caa64-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="caa64-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

