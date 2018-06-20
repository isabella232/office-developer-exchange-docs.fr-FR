---
title: ConflictingMeetings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetings
api_type:
- schema
ms.assetid: cfff7a11-7b3a-4995-9815-afedd45ebb0f
description: L’élément ConflictingMeetings identifie tous les éléments de calendrier qui entre en conflit avec une heure de réunion.
ms.openlocfilehash: 1d2558dba41ec3e7ae2711bb2dc26f54cada827a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755538"
---
# <a name="conflictingmeetings"></a><span data-ttu-id="533f3-103">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="533f3-103">ConflictingMeetings</span></span>

<span data-ttu-id="533f3-104">L’élément **ConflictingMeetings** identifie tous les éléments de calendrier qui entre en conflit avec une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="533f3-104">The **ConflictingMeetings** element identifies all calendar items that conflict with a meeting time.</span></span> 
  
```xml
<ConflictingMeetings>
   <CalendarItem/>
</ConflictingMeetings>
```

 <span data-ttu-id="533f3-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="533f3-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="533f3-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="533f3-106">Attributes and elements</span></span>

<span data-ttu-id="533f3-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="533f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="533f3-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="533f3-108">Attributes</span></span>

<span data-ttu-id="533f3-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="533f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="533f3-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="533f3-110">Child elements</span></span>

|<span data-ttu-id="533f3-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="533f3-111">**Element**</span></span>|<span data-ttu-id="533f3-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="533f3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="533f3-113">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="533f3-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="533f3-114">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="533f3-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="533f3-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="533f3-115">Parent elements</span></span>

|<span data-ttu-id="533f3-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="533f3-116">**Element**</span></span>|<span data-ttu-id="533f3-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="533f3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="533f3-118">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="533f3-118">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="533f3-119">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="533f3-119">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="533f3-120">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="533f3-120">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="533f3-121">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="533f3-121">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="533f3-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="533f3-122">Remarks</span></span>

<span data-ttu-id="533f3-123">Si cet élément est utilisé, il doit contenir un ou plusieurs éléments enfants.</span><span class="sxs-lookup"><span data-stu-id="533f3-123">If this element is used, it must contain one or more child elements.</span></span>
  
<span data-ttu-id="533f3-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="533f3-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="533f3-125">Bien que les éléments enfants supplémentaires sont valides par rapport au schéma, l’élément [CalendarItem](calendaritem.md) est le seul élément enfant renvoyant des Exchange Web Services (EWS) dans l’élément **ConflictingMeetings** .</span><span class="sxs-lookup"><span data-stu-id="533f3-125">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **ConflictingMeetings** element.</span></span> <span data-ttu-id="533f3-126">Cette rubrique ne répertorie pas les éléments enfants sont valides par rapport au schéma, mais ne sont pas renvoyés par EWS.</span><span class="sxs-lookup"><span data-stu-id="533f3-126">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="533f3-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="533f3-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="533f3-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="533f3-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="533f3-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="533f3-129">Schema Name</span></span>  <br/> |<span data-ttu-id="533f3-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="533f3-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="533f3-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="533f3-131">Validation File</span></span>  <br/> |<span data-ttu-id="533f3-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="533f3-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="533f3-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="533f3-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="533f3-134">False</span><span class="sxs-lookup"><span data-stu-id="533f3-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="533f3-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="533f3-135">See also</span></span>



- [<span data-ttu-id="533f3-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="533f3-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

