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
description: L’élément BusyType représente l’état de disponibilité défini pour un événement de calendrier.
ms.openlocfilehash: 7c2d18c21156a8603d3caeeb796a56c5d8afcba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459082"
---
# <a name="busytype"></a><span data-ttu-id="b0a31-103">BusyType</span><span class="sxs-lookup"><span data-stu-id="b0a31-103">BusyType</span></span>

<span data-ttu-id="b0a31-104">L’élément **BusyType** représente l’état de disponibilité défini pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="b0a31-104">The **BusyType** element represents the free/busy status set for a calendar event.</span></span> 
  
```xml
<BusyType>Free or Tentative or Busy or OOF or NoData</BusyType>
```

 <span data-ttu-id="b0a31-105">**BusyType**</span><span class="sxs-lookup"><span data-stu-id="b0a31-105">**BusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0a31-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b0a31-106">Attributes and elements</span></span>

<span data-ttu-id="b0a31-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b0a31-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0a31-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b0a31-108">Attributes</span></span>

<span data-ttu-id="b0a31-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b0a31-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0a31-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b0a31-110">Child elements</span></span>

<span data-ttu-id="b0a31-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b0a31-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b0a31-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b0a31-112">Parent elements</span></span>

|<span data-ttu-id="b0a31-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b0a31-113">**Element**</span></span>|<span data-ttu-id="b0a31-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b0a31-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0a31-115">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="b0a31-115">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="b0a31-116">Contient le statut de disponibilité d’un utilisateur ou d’un contact pour une fenêtre de temps qui se produit en même temps que la réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="b0a31-116">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time.</span></span>  <br/> <span data-ttu-id="b0a31-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="b0a31-117">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/IndividualAttendeeConflictData` <br/> |
|[<span data-ttu-id="b0a31-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="b0a31-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="b0a31-119">Représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="b0a31-119">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="b0a31-120">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="b0a31-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b0a31-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="b0a31-121">Text value</span></span>

<span data-ttu-id="b0a31-122">Une valeur de texte est requise pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="b0a31-122">A text value is required for this element.</span></span> <span data-ttu-id="b0a31-123">La valeur est un type de chaîne.</span><span class="sxs-lookup"><span data-stu-id="b0a31-123">The value is a string type.</span></span> <span data-ttu-id="b0a31-124">Les valeurs possibles pour l’élément [BusyType](busytype.md) sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="b0a31-124">The following are the possible values for the [BusyType](busytype.md) element:</span></span> 
  
- <span data-ttu-id="b0a31-125">Gratuit</span><span class="sxs-lookup"><span data-stu-id="b0a31-125">Free</span></span>
    
- <span data-ttu-id="b0a31-126">Provisoire</span><span class="sxs-lookup"><span data-stu-id="b0a31-126">Tentative</span></span>
    
- <span data-ttu-id="b0a31-127">Occupé(e)</span><span class="sxs-lookup"><span data-stu-id="b0a31-127">Busy</span></span>
    
- <span data-ttu-id="b0a31-128">Bureau</span><span class="sxs-lookup"><span data-stu-id="b0a31-128">OOF</span></span>
    
- <span data-ttu-id="b0a31-129">NoData</span><span class="sxs-lookup"><span data-stu-id="b0a31-129">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="b0a31-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="b0a31-130">Remarks</span></span>

<span data-ttu-id="b0a31-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b0a31-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0a31-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b0a31-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0a31-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b0a31-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0a31-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b0a31-134">Schema Name</span></span>  <br/> |<span data-ttu-id="b0a31-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b0a31-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0a31-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b0a31-136">Validation File</span></span>  <br/> |<span data-ttu-id="b0a31-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b0a31-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0a31-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b0a31-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0a31-139">False</span><span class="sxs-lookup"><span data-stu-id="b0a31-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0a31-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b0a31-140">See also</span></span>



[<span data-ttu-id="b0a31-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b0a31-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b0a31-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b0a31-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b0a31-143">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="b0a31-143">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

