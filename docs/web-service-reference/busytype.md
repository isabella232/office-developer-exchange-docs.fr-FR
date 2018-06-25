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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755461"
---
# <a name="busytype"></a><span data-ttu-id="77c07-103">BusyType</span><span class="sxs-lookup"><span data-stu-id="77c07-103">BusyType</span></span>

<span data-ttu-id="77c07-104">L’élément **BusyType** représente l’état de disponibilité pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="77c07-104">The **BusyType** element represents the free/busy status set for a calendar event.</span></span> 
  
```xml
<BusyType>Free or Tentative or Busy or OOF or NoData</BusyType>
```

 <span data-ttu-id="77c07-105">**BusyType**</span><span class="sxs-lookup"><span data-stu-id="77c07-105">**BusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77c07-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="77c07-106">Attributes and elements</span></span>

<span data-ttu-id="77c07-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="77c07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77c07-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="77c07-108">Attributes</span></span>

<span data-ttu-id="77c07-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="77c07-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77c07-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="77c07-110">Child elements</span></span>

<span data-ttu-id="77c07-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="77c07-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="77c07-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="77c07-112">Parent elements</span></span>

|<span data-ttu-id="77c07-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="77c07-113">**Element**</span></span>|<span data-ttu-id="77c07-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="77c07-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77c07-115">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="77c07-115">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="77c07-116">Contient un utilisateur ou un contact disponibilité pour une fenêtre de temps qui se produit en même temps que l’heure de réunion proposée.</span><span class="sxs-lookup"><span data-stu-id="77c07-116">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time.</span></span>  <br/> <span data-ttu-id="77c07-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="77c07-117">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/IndividualAttendeeConflictData` <br/> |
|[<span data-ttu-id="77c07-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="77c07-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="77c07-119">Représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="77c07-119">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="77c07-120">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="77c07-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="77c07-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="77c07-121">Text value</span></span>

<span data-ttu-id="77c07-122">Une valeur de texte est nécessaire pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="77c07-122">A text value is required for this element.</span></span> <span data-ttu-id="77c07-123">La valeur est de type chaîne.</span><span class="sxs-lookup"><span data-stu-id="77c07-123">The value is a string type.</span></span> <span data-ttu-id="77c07-124">Les valeurs possibles pour l’élément [BusyType](busytype.md) sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="77c07-124">The following are the possible values for the [BusyType](busytype.md) element:</span></span> 
  
- <span data-ttu-id="77c07-125">Gratuit</span><span class="sxs-lookup"><span data-stu-id="77c07-125">Free</span></span>
    
- <span data-ttu-id="77c07-126">Provisoire</span><span class="sxs-lookup"><span data-stu-id="77c07-126">Tentative</span></span>
    
- <span data-ttu-id="77c07-127">Occupé(e)</span><span class="sxs-lookup"><span data-stu-id="77c07-127">Busy</span></span>
    
- <span data-ttu-id="77c07-128">ABSENCE DU BUREAU</span><span class="sxs-lookup"><span data-stu-id="77c07-128">OOF</span></span>
    
- <span data-ttu-id="77c07-129">NoData</span><span class="sxs-lookup"><span data-stu-id="77c07-129">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="77c07-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="77c07-130">Remarks</span></span>

<span data-ttu-id="77c07-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="77c07-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77c07-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="77c07-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77c07-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="77c07-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="77c07-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="77c07-134">Schema Name</span></span>  <br/> |<span data-ttu-id="77c07-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="77c07-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="77c07-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="77c07-136">Validation File</span></span>  <br/> |<span data-ttu-id="77c07-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="77c07-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="77c07-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="77c07-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="77c07-139">False</span><span class="sxs-lookup"><span data-stu-id="77c07-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77c07-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="77c07-140">See also</span></span>



[<span data-ttu-id="77c07-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="77c07-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="77c07-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="77c07-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="77c07-143">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="77c07-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

