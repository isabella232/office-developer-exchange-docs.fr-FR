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
description: L’élément RemoveItem représente un objet de réponse qui est utilisé pour supprimer un élément de réunion lorsqu’un message MeetingCancellation est reçu.
ms.openlocfilehash: 6897363eba602e6a135ad255822197f9296dd44a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829108"
---
# <a name="removeitem"></a><span data-ttu-id="bbea5-103">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="bbea5-103">RemoveItem</span></span>

<span data-ttu-id="bbea5-104">L’élément **RemoveItem** représente un objet de réponse qui est utilisé pour supprimer un élément de réunion lorsqu’un message MeetingCancellation est reçu.</span><span class="sxs-lookup"><span data-stu-id="bbea5-104">The **RemoveItem** element represents a response object that is used to remove a meeting item when a MeetingCancellation message is received.</span></span> 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 <span data-ttu-id="bbea5-105">**RemoveItemType**</span><span class="sxs-lookup"><span data-stu-id="bbea5-105">**RemoveItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bbea5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bbea5-106">Attributes and elements</span></span>

<span data-ttu-id="bbea5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bbea5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bbea5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bbea5-108">Attributes</span></span>

|<span data-ttu-id="bbea5-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bbea5-109">**Attribute**</span></span>|<span data-ttu-id="bbea5-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="bbea5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bbea5-111">**ObjectName**</span><span class="sxs-lookup"><span data-stu-id="bbea5-111">**ObjectName**</span></span> <br/> |<span data-ttu-id="bbea5-112">Représente le nom de la classe d’objet RemoveItem réponse sous la forme d’une chaîne en anglais.</span><span class="sxs-lookup"><span data-stu-id="bbea5-112">Represents the name of the RemoveItem reply object class as an English string.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bbea5-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bbea5-113">Child elements</span></span>

|<span data-ttu-id="bbea5-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bbea5-114">**Element**</span></span>|<span data-ttu-id="bbea5-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="bbea5-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bbea5-116">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="bbea5-116">ReferenceItemId</span></span>](referenceitemid.md) <br/> |<span data-ttu-id="bbea5-117">Identifie l’élément auquel l’objet de réponse RemoveItem fait référence.</span><span class="sxs-lookup"><span data-stu-id="bbea5-117">Identifies the item to which the RemoveItem response object refers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bbea5-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bbea5-118">Parent elements</span></span>

|<span data-ttu-id="bbea5-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bbea5-119">**Element**</span></span>|<span data-ttu-id="bbea5-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="bbea5-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bbea5-121">Éléments (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="bbea5-121">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="bbea5-122">Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).</span><span class="sxs-lookup"><span data-stu-id="bbea5-122">Contains an array of items to create in the folder that is identified by the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span>  <br/> |
|[<span data-ttu-id="bbea5-123">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="bbea5-123">ResponseObjects</span></span>](responseobjects.md) <br/> |<span data-ttu-id="bbea5-124">Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="bbea5-124">Contains a collection of all the response objects that are associated with an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bbea5-125">Note</span><span class="sxs-lookup"><span data-stu-id="bbea5-125">Remarks</span></span>

 <span data-ttu-id="bbea5-126">**RemoveItem** est valide uniquement pour un [MeetingCancellation](meetingcancellation.md).</span><span class="sxs-lookup"><span data-stu-id="bbea5-126">**RemoveItem** is valid only for a [MeetingCancellation](meetingcancellation.md).</span></span> <span data-ttu-id="bbea5-127">Dans le cas contraire, une erreur est générée.</span><span class="sxs-lookup"><span data-stu-id="bbea5-127">Otherwise, an error is thrown.</span></span>
  
> [!NOTE]
> <span data-ttu-id="bbea5-128">[ItemClass](itemclass.md) pour une annulation de réunion est IPM. Schedule.Meeting.Canceled.</span><span class="sxs-lookup"><span data-stu-id="bbea5-128">The [ItemClass](itemclass.md) for a meeting cancellation is IPM.Schedule.Meeting.Canceled.</span></span> 
  
<span data-ttu-id="bbea5-129">Pour supprimer un [MeetingRequest](meetingrequest.md) et le associée [CalendarItem](calendaritem.md), utilisez l’objet de réponse [DeclineItem](declineitem.md) au lieu de **RemoveItem**.</span><span class="sxs-lookup"><span data-stu-id="bbea5-129">To remove a [MeetingRequest](meetingrequest.md) and the associated [CalendarItem](calendaritem.md), use the [DeclineItem](declineitem.md) response object instead of **RemoveItem**.</span></span>
  
 <span data-ttu-id="bbea5-130">**RemoveItem** n’est pas pris en charge pour l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="bbea5-130">**RemoveItem** is not supported for delegate access.</span></span> 
  
<span data-ttu-id="bbea5-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="bbea5-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bbea5-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bbea5-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bbea5-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bbea5-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bbea5-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bbea5-134">Schema Name</span></span>  <br/> |<span data-ttu-id="bbea5-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bbea5-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="bbea5-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bbea5-136">Validation File</span></span>  <br/> |<span data-ttu-id="bbea5-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bbea5-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bbea5-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bbea5-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="bbea5-139">False</span><span class="sxs-lookup"><span data-stu-id="bbea5-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bbea5-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bbea5-140">See also</span></span>



- [<span data-ttu-id="bbea5-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bbea5-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

