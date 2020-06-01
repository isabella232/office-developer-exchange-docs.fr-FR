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
description: L’élément AdjacentMeetings identifie tous les éléments de calendrier adjacents à une heure de réunion.
ms.openlocfilehash: 7c89095e24af799df22a848be06a0fd65d53be7f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463579"
---
# <a name="adjacentmeetings"></a><span data-ttu-id="2000a-103">AdjacentMeetings</span><span class="sxs-lookup"><span data-stu-id="2000a-103">AdjacentMeetings</span></span>

<span data-ttu-id="2000a-104">L’élément **AdjacentMeetings** identifie tous les éléments de calendrier adjacents à une heure de réunion.</span><span class="sxs-lookup"><span data-stu-id="2000a-104">The **AdjacentMeetings** element identifies all calendar items that are adjacent to a meeting time.</span></span> 
  
```xml
<AdjacentMeetings>
   <CalendarItem/>
</AdjacentMeetings>
```

 <span data-ttu-id="2000a-105">**NonEmptyArrayOfAllItemsType**</span><span class="sxs-lookup"><span data-stu-id="2000a-105">**NonEmptyArrayOfAllItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2000a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2000a-106">Attributes and elements</span></span>

<span data-ttu-id="2000a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2000a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2000a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2000a-108">Attributes</span></span>

<span data-ttu-id="2000a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2000a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2000a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2000a-110">Child elements</span></span>

|<span data-ttu-id="2000a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2000a-111">**Element**</span></span>|<span data-ttu-id="2000a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2000a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2000a-113">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2000a-113">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2000a-114">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="2000a-114">Represents an Exchange calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2000a-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2000a-115">Parent elements</span></span>

|<span data-ttu-id="2000a-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2000a-116">**Element**</span></span>|<span data-ttu-id="2000a-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="2000a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2000a-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2000a-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2000a-119">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="2000a-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2000a-120">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="2000a-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2000a-121">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2000a-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2000a-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="2000a-122">Remarks</span></span>

<span data-ttu-id="2000a-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2000a-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="2000a-124">Bien que des éléments enfants supplémentaires soient valides par schéma, l’élément [CalendarItem](calendaritem.md) est le seul élément enfant renvoyé par les services Web Exchange (EWS) à l’intérieur de l’élément **AdjacentMeetings** .</span><span class="sxs-lookup"><span data-stu-id="2000a-124">Although additional child elements are valid per the schema, the [CalendarItem](calendaritem.md) element is the only child element that Exchange Web Services (EWS) will return within the **AdjacentMeetings** element.</span></span> <span data-ttu-id="2000a-125">Cette rubrique ne répertorie pas les éléments enfants qui sont valides par le schéma, mais qui ne sont pas renvoyés par EWS.</span><span class="sxs-lookup"><span data-stu-id="2000a-125">This topic does not list child elements that are valid per the schema but will not be returned by EWS.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="2000a-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2000a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2000a-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2000a-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2000a-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2000a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="2000a-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2000a-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="2000a-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2000a-130">Validation File</span></span>  <br/> |<span data-ttu-id="2000a-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2000a-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2000a-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2000a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="2000a-133">False</span><span class="sxs-lookup"><span data-stu-id="2000a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2000a-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2000a-134">See also</span></span>

- [<span data-ttu-id="2000a-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2000a-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

