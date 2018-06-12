---
title: ConflictingMeetingCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: L’élément ConflictingMeetingCount représente le nombre de réunions entre en conflit avec l’élément de calendrier.
ms.openlocfilehash: ace800982c284cf65ff22d92c711197ee5ee1d06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755536"
---
# <a name="conflictingmeetingcount"></a><span data-ttu-id="a5694-103">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="a5694-103">ConflictingMeetingCount</span></span>

<span data-ttu-id="a5694-104">L’élément **ConflictingMeetingCount** représente le nombre de réunions entre en conflit avec l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="a5694-104">The **ConflictingMeetingCount** element represents the number of meetings that conflict with the calendar item.</span></span> 
  
```xml
<ConflictingMeetingCount/>
```

 <span data-ttu-id="a5694-105">**int**</span><span class="sxs-lookup"><span data-stu-id="a5694-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5694-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a5694-106">Attributes and elements</span></span>

<span data-ttu-id="a5694-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a5694-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5694-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a5694-108">Attributes</span></span>

<span data-ttu-id="a5694-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a5694-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5694-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a5694-110">Child elements</span></span>

<span data-ttu-id="a5694-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a5694-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a5694-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a5694-112">Parent elements</span></span>

|<span data-ttu-id="a5694-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a5694-113">**Element**</span></span>|<span data-ttu-id="a5694-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a5694-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5694-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a5694-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a5694-116">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5694-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a5694-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a5694-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a5694-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5694-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a5694-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a5694-119">Text value</span></span>

<span data-ttu-id="a5694-120">La valeur de texte représente un entier.</span><span class="sxs-lookup"><span data-stu-id="a5694-120">The text value represents an integer.</span></span> <span data-ttu-id="a5694-121">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="a5694-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a5694-122">Note</span><span class="sxs-lookup"><span data-stu-id="a5694-122">Remarks</span></span>

<span data-ttu-id="a5694-123">Un élément de calendrier est considéré comme en conflit si elle a lieu, au moins en partie, en même temps en tant qu’un autre élément de calendrier dans le même dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="a5694-123">A calendar item is considered conflicting if it occurs, at least in part, at the same time as another calendar item in the same calendar folder.</span></span> <span data-ttu-id="a5694-124">Si un élément de calendrier se trouve dans un dossier noncalendar, il est comparé aux éléments de calendrier dans le dossier calendrier par défaut.</span><span class="sxs-lookup"><span data-stu-id="a5694-124">If a calendar item is in a noncalendar folder, it is compared with calendar items in the default calendar folder.</span></span> <span data-ttu-id="a5694-125">Demandes de réunion sont comparées avec les éléments de calendrier dans le dossier calendrier par défaut.</span><span class="sxs-lookup"><span data-stu-id="a5694-125">Meeting requests are compared with calendar items in the default calendar folder.</span></span>
  
<span data-ttu-id="a5694-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a5694-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5694-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a5694-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5694-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a5694-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a5694-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a5694-129">Schema name</span></span>  <br/> |<span data-ttu-id="a5694-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a5694-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="a5694-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a5694-131">Validation file</span></span>  <br/> |<span data-ttu-id="a5694-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a5694-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a5694-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a5694-133">Can be empty</span></span>  <br/> |<span data-ttu-id="a5694-134">False</span><span class="sxs-lookup"><span data-stu-id="a5694-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5694-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a5694-135">See also</span></span>



- [<span data-ttu-id="a5694-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a5694-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

