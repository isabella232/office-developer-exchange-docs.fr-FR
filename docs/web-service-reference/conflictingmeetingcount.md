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
description: L’élément ConflictingMeetingCount représente le nombre de réunions en conflit avec l’élément de calendrier.
ms.openlocfilehash: d53245e1b5d1f0182b28b15bf55ba9742bbb2a07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463859"
---
# <a name="conflictingmeetingcount"></a><span data-ttu-id="0d192-103">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="0d192-103">ConflictingMeetingCount</span></span>

<span data-ttu-id="0d192-104">L’élément **ConflictingMeetingCount** représente le nombre de réunions en conflit avec l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0d192-104">The **ConflictingMeetingCount** element represents the number of meetings that conflict with the calendar item.</span></span> 
  
```xml
<ConflictingMeetingCount/>
```

 <span data-ttu-id="0d192-105">**int**</span><span class="sxs-lookup"><span data-stu-id="0d192-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d192-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0d192-106">Attributes and elements</span></span>

<span data-ttu-id="0d192-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0d192-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d192-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0d192-108">Attributes</span></span>

<span data-ttu-id="0d192-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0d192-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d192-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0d192-110">Child elements</span></span>

<span data-ttu-id="0d192-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0d192-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0d192-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0d192-112">Parent elements</span></span>

|<span data-ttu-id="0d192-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0d192-113">**Element**</span></span>|<span data-ttu-id="0d192-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0d192-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d192-115">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="0d192-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0d192-116">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d192-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0d192-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="0d192-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="0d192-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d192-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0d192-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0d192-119">Text value</span></span>

<span data-ttu-id="0d192-120">La valeur texte représente un entier.</span><span class="sxs-lookup"><span data-stu-id="0d192-120">The text value represents an integer.</span></span> <span data-ttu-id="0d192-121">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="0d192-121">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0d192-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="0d192-122">Remarks</span></span>

<span data-ttu-id="0d192-123">Un élément de calendrier est considéré comme conflictuel s’il se produit, au moins en partie, en même temps qu’un autre élément de calendrier dans le même dossier de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0d192-123">A calendar item is considered conflicting if it occurs, at least in part, at the same time as another calendar item in the same calendar folder.</span></span> <span data-ttu-id="0d192-124">Si un élément de calendrier se trouve dans un dossier non calendrier, il est comparé aux éléments de calendrier dans le dossier de calendrier par défaut.</span><span class="sxs-lookup"><span data-stu-id="0d192-124">If a calendar item is in a noncalendar folder, it is compared with calendar items in the default calendar folder.</span></span> <span data-ttu-id="0d192-125">Les demandes de réunion sont comparées aux éléments de calendrier dans le dossier calendrier par défaut.</span><span class="sxs-lookup"><span data-stu-id="0d192-125">Meeting requests are compared with calendar items in the default calendar folder.</span></span>
  
<span data-ttu-id="0d192-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0d192-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d192-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0d192-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d192-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0d192-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0d192-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0d192-129">Schema name</span></span>  <br/> |<span data-ttu-id="0d192-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0d192-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="0d192-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0d192-131">Validation file</span></span>  <br/> |<span data-ttu-id="0d192-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0d192-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0d192-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0d192-133">Can be empty</span></span>  <br/> |<span data-ttu-id="0d192-134">False</span><span class="sxs-lookup"><span data-stu-id="0d192-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d192-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0d192-135">See also</span></span>



- [<span data-ttu-id="0d192-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0d192-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

