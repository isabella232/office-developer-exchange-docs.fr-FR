---
title: Emplacement (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Location
api_type:
- schema
ms.assetid: 883cce6e-66b8-4dbc-935c-83ef5100a953
description: L’élément Location représente le champ emplacement de l’élément de calendrier.
ms.openlocfilehash: 3678bd94851633fcca9817c020106670b57d110c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828245"
---
# <a name="location-calendareventdetails"></a><span data-ttu-id="c1389-103">Emplacement (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="c1389-103">Location (CalendarEventDetails)</span></span>

<span data-ttu-id="c1389-104">L’élément **Location** représente le champ emplacement de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="c1389-104">The **Location** element represents the location field of the calendar item.</span></span> 
  
[<span data-ttu-id="c1389-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c1389-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="c1389-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="c1389-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="c1389-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="c1389-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="c1389-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="c1389-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="c1389-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="c1389-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="c1389-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="c1389-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="c1389-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="c1389-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="c1389-112">Emplacement (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="c1389-112">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
  
```xml
<Location/>
```

 <span data-ttu-id="c1389-113">**string**</span><span class="sxs-lookup"><span data-stu-id="c1389-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1389-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c1389-114">Attributes and elements</span></span>

<span data-ttu-id="c1389-115">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c1389-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1389-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="c1389-116">Attributes</span></span>

<span data-ttu-id="c1389-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c1389-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1389-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c1389-118">Child elements</span></span>

<span data-ttu-id="c1389-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c1389-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c1389-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c1389-120">Parent elements</span></span>

|<span data-ttu-id="c1389-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c1389-121">**Element**</span></span>|<span data-ttu-id="c1389-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="c1389-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1389-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="c1389-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="c1389-124">Fournit des informations supplémentaires pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="c1389-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="c1389-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="c1389-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c1389-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c1389-126">Text value</span></span>

<span data-ttu-id="c1389-127">Une valeur de texte est obligatoire si cet élément est retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="c1389-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="c1389-128">Cet élément peut contenir une chaîne vide.</span><span class="sxs-lookup"><span data-stu-id="c1389-128">This element can contain an empty string.</span></span> <span data-ttu-id="c1389-129">Cet élément est facultatif si l’élément [CalendarEventDetails](calendareventdetails.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="c1389-129">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c1389-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="c1389-130">Remarks</span></span>

<span data-ttu-id="c1389-131">Cet élément est mappé à un MAPI EMPLACEMENT_PR propriété nommée.</span><span class="sxs-lookup"><span data-stu-id="c1389-131">This element maps to a PR_Location MAPI named property.</span></span>
  
<span data-ttu-id="c1389-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c1389-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1389-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c1389-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1389-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c1389-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c1389-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c1389-135">Schema Name</span></span>  <br/> |<span data-ttu-id="c1389-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c1389-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="c1389-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c1389-137">Validation File</span></span>  <br/> |<span data-ttu-id="c1389-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c1389-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c1389-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c1389-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="c1389-140">False</span><span class="sxs-lookup"><span data-stu-id="c1389-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1389-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c1389-141">See also</span></span>



[<span data-ttu-id="c1389-142">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c1389-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="c1389-143">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c1389-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="c1389-144">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="c1389-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

