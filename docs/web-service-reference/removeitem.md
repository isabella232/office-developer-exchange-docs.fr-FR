---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: L’élément RemoveItem représente un objet de réponse qui est utilisé pour supprimer un élément de réunion lors de la réception d’un message MeetingCancellation.
ms.openlocfilehash: c0cd5c1f9894287ee78c2f7a65b8f4d3b943414e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467689"
---
# <a name="removeitem"></a><span data-ttu-id="94ea4-103">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="94ea4-103">RemoveItem</span></span>

<span data-ttu-id="94ea4-104">L’élément **RemoveItem** représente un objet de réponse qui est utilisé pour supprimer un élément de réunion lors de la réception d’un message MeetingCancellation.</span><span class="sxs-lookup"><span data-stu-id="94ea4-104">The **RemoveItem** element represents a response object that is used to remove a meeting item when a MeetingCancellation message is received.</span></span> 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 <span data-ttu-id="94ea4-105">**RemoveItemType**</span><span class="sxs-lookup"><span data-stu-id="94ea4-105">**RemoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94ea4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="94ea4-106">Attributes and elements</span></span>

<span data-ttu-id="94ea4-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="94ea4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94ea4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="94ea4-108">Attributes</span></span>

|<span data-ttu-id="94ea4-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="94ea4-109">**Attribute**</span></span>|<span data-ttu-id="94ea4-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="94ea4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="94ea4-111">**ObjectName**</span><span class="sxs-lookup"><span data-stu-id="94ea4-111">**ObjectName**</span></span> <br/> |<span data-ttu-id="94ea4-112">Représente le nom de la classe d’objet de réponse RemoveItem sous la forme d’une chaîne en anglais.</span><span class="sxs-lookup"><span data-stu-id="94ea4-112">Represents the name of the RemoveItem reply object class as an English string.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="94ea4-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="94ea4-113">Child elements</span></span>

|<span data-ttu-id="94ea4-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="94ea4-114">**Element**</span></span>|<span data-ttu-id="94ea4-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="94ea4-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94ea4-116">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="94ea4-116">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="94ea4-117">Identifie l’élément auquel l’objet de réponse RemoveItem fait référence.</span><span class="sxs-lookup"><span data-stu-id="94ea4-117">Identifies the item to which the RemoveItem response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="94ea4-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="94ea4-118">Parent elements</span></span>

|<span data-ttu-id="94ea4-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="94ea4-119">**Element**</span></span>|<span data-ttu-id="94ea4-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="94ea4-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94ea4-121">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="94ea4-121">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="94ea4-122">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="94ea4-122">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="94ea4-123">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="94ea4-123">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="94ea4-124">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="94ea4-124">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="94ea4-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="94ea4-125">Remarks</span></span>

 <span data-ttu-id="94ea4-126">**RemoveItem** est valide uniquement pour un [MeetingCancellation](meetingcancellation.md).</span><span class="sxs-lookup"><span data-stu-id="94ea4-126">**RemoveItem** is valid only for a [MeetingCancellation](meetingcancellation.md).</span></span> <span data-ttu-id="94ea4-127">Sinon, une erreur est générée.</span><span class="sxs-lookup"><span data-stu-id="94ea4-127">Otherwise, an error is thrown.</span></span>
  
> [!NOTE]
> <span data-ttu-id="94ea4-128">Le [ItemClass](itemclass.md) pour une annulation de réunion est IPM. Schedule. Meeting. Canceled.</span><span class="sxs-lookup"><span data-stu-id="94ea4-128">The [ItemClass](itemclass.md) for a meeting cancellation is IPM.Schedule.Meeting.Canceled.</span></span> 
  
<span data-ttu-id="94ea4-129">Pour supprimer un [propriété meetingrequest](meetingrequest.md) et les [CalendarItem](calendaritem.md)associés, utilisez l’objet Response [DeclineItem](declineitem.md) au lieu de **RemoveItem**.</span><span class="sxs-lookup"><span data-stu-id="94ea4-129">To remove a [MeetingRequest](meetingrequest.md) and the associated [CalendarItem](calendaritem.md), use the [DeclineItem](declineitem.md) response object instead of **RemoveItem**.</span></span>
  
 <span data-ttu-id="94ea4-130">**RemoveItem** n’est pas pris en charge pour l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="94ea4-130">**RemoveItem** is not supported for delegate access.</span></span> 
  
<span data-ttu-id="94ea4-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="94ea4-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94ea4-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="94ea4-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94ea4-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="94ea4-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94ea4-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="94ea4-134">Schema Name</span></span>  <br/> |<span data-ttu-id="94ea4-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="94ea4-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="94ea4-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="94ea4-136">Validation File</span></span>  <br/> |<span data-ttu-id="94ea4-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="94ea4-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94ea4-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="94ea4-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="94ea4-139">False</span><span class="sxs-lookup"><span data-stu-id="94ea4-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94ea4-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="94ea4-140">See also</span></span>



- [<span data-ttu-id="94ea4-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="94ea4-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

