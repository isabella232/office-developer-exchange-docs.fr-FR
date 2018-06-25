---
title: AdjacentMeetings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdjacentMeetings
api_type:
- schema
ms.assetid: 50a9c381-9166-476e-8421-29e51b94499b
description: L’élément AdjacentMeetings identifie tous les éléments de calendrier sont adjacents à une heure de réunion.
ms.openlocfilehash: 9ab818f4f67c32c01101cc595ccb92424a872ef0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755186"
---
# <a name="adjacentmeetings"></a><span data-ttu-id="8d504-103">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="8d504-103">AdjacentMeetings</span></span>

<span data-ttu-id="8d504-104">L’élément **AdjacentMeetings** identifie tous les éléments de calendrier sont adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="8d504-104">The **AdjacentMeetings** element identifies all calendar items that are adjacent to a meeting time.</span></span> 
  
```xml
<AdjacentMeetings>
   <CalendarItem/>
</AdjacentMeetings>
```

 <span data-ttu-id="8d504-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="8d504-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d504-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8d504-106">Attributes and elements</span></span>

<span data-ttu-id="8d504-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8d504-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d504-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8d504-108">Attributes</span></span>

<span data-ttu-id="8d504-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8d504-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d504-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8d504-110">Child elements</span></span>

|<span data-ttu-id="8d504-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8d504-111">**Element**</span></span>|<span data-ttu-id="8d504-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8d504-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d504-113">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="8d504-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8d504-114">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="8d504-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8d504-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8d504-115">Parent elements</span></span>

|<span data-ttu-id="8d504-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8d504-116">**Element**</span></span>|<span data-ttu-id="8d504-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="8d504-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d504-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="8d504-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8d504-119">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="8d504-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8d504-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8d504-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8d504-121">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="8d504-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8d504-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="8d504-122">Remarks</span></span>

<span data-ttu-id="8d504-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="8d504-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="8d504-124">Bien que les éléments enfants supplémentaires sont valides par rapport au schéma, l’élément [CalendarItem](calendaritem.md) est le seul élément enfant renvoyant des Exchange Web Services (EWS) dans l’élément **AdjacentMeetings** .</span><span class="sxs-lookup"><span data-stu-id="8d504-124">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **AdjacentMeetings** element.</span></span> <span data-ttu-id="8d504-125">Cette rubrique ne répertorie pas les éléments enfants sont valides par rapport au schéma, mais ne sont pas renvoyés par EWS.</span><span class="sxs-lookup"><span data-stu-id="8d504-125">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8d504-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8d504-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d504-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8d504-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d504-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8d504-128">Schema Name</span></span>  <br/> |<span data-ttu-id="8d504-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8d504-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d504-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8d504-130">Validation File</span></span>  <br/> |<span data-ttu-id="8d504-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8d504-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d504-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8d504-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d504-133">False</span><span class="sxs-lookup"><span data-stu-id="8d504-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d504-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8d504-134">See also</span></span>

- [<span data-ttu-id="8d504-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8d504-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

