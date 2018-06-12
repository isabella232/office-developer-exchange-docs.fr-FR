---
title: BusyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BusyType
api_type:
- schema
ms.assetid: 26d4fae0-8c78-4705-b5e8-d6033712c41e
description: L’élément BusyType représente l’état de disponibilité pour un événement de calendrier.
ms.openlocfilehash: 6484bc70c6a05084e5d2bc1738b575fbebe4c132
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755461"
---
# <a name="busytype"></a><span data-ttu-id="71c97-103">BusyType</span><span class="sxs-lookup"><span data-stu-id="71c97-103">BusyType</span></span>

<span data-ttu-id="71c97-104">L’élément **BusyType** représente l’état de disponibilité pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="71c97-104">The **BusyType** element represents the free/busy status set for a calendar event.</span></span> 
  
```xml
<BusyType>Free or Tentative or Busy or OOF or NoData</BusyType>
```

 <span data-ttu-id="71c97-105">**BusyType**</span><span class="sxs-lookup"><span data-stu-id="71c97-105">**BusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71c97-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="71c97-106">Attributes and elements</span></span>

<span data-ttu-id="71c97-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="71c97-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71c97-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="71c97-108">Attributes</span></span>

<span data-ttu-id="71c97-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="71c97-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71c97-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="71c97-110">Child elements</span></span>

<span data-ttu-id="71c97-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="71c97-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="71c97-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="71c97-112">Parent elements</span></span>

|<span data-ttu-id="71c97-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="71c97-113">**Element**</span></span>|<span data-ttu-id="71c97-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="71c97-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71c97-115">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="71c97-115">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="71c97-116">Contient un utilisateur ou un contact disponibilité pour une fenêtre de temps qui se produit en même temps que l’heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="71c97-116">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time.</span></span>  <br/> <span data-ttu-id="71c97-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="71c97-117">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/IndividualAttendeeConflictData` <br/> |
|[<span data-ttu-id="71c97-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="71c97-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="71c97-119">Représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="71c97-119">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="71c97-120">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="71c97-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="71c97-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="71c97-121">Text value</span></span>

<span data-ttu-id="71c97-122">Une valeur de texte est nécessaire pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="71c97-122">A text value is required for this element.</span></span> <span data-ttu-id="71c97-123">La valeur est de type chaîne.</span><span class="sxs-lookup"><span data-stu-id="71c97-123">The value is a string type.</span></span> <span data-ttu-id="71c97-124">Les valeurs possibles pour l’élément [BusyType](busytype.md) sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="71c97-124">The following are the possible values for the [BusyType](busytype.md) element:</span></span> 
  
- <span data-ttu-id="71c97-125">Gratuit</span><span class="sxs-lookup"><span data-stu-id="71c97-125">Free</span></span>
    
- <span data-ttu-id="71c97-126">Provisoire</span><span class="sxs-lookup"><span data-stu-id="71c97-126">Tentative</span></span>
    
- <span data-ttu-id="71c97-127">Occupé(e)</span><span class="sxs-lookup"><span data-stu-id="71c97-127">Busy</span></span>
    
- <span data-ttu-id="71c97-128">ABSENCE DU BUREAU</span><span class="sxs-lookup"><span data-stu-id="71c97-128">OOF</span></span>
    
- <span data-ttu-id="71c97-129">NoData</span><span class="sxs-lookup"><span data-stu-id="71c97-129">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="71c97-130">Note</span><span class="sxs-lookup"><span data-stu-id="71c97-130">Remarks</span></span>

<span data-ttu-id="71c97-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="71c97-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71c97-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="71c97-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71c97-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="71c97-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71c97-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="71c97-134">Schema Name</span></span>  <br/> |<span data-ttu-id="71c97-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="71c97-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="71c97-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="71c97-136">Validation File</span></span>  <br/> |<span data-ttu-id="71c97-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="71c97-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71c97-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="71c97-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="71c97-139">False</span><span class="sxs-lookup"><span data-stu-id="71c97-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71c97-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="71c97-140">See also</span></span>



[<span data-ttu-id="71c97-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="71c97-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="71c97-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="71c97-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="71c97-143">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="71c97-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

