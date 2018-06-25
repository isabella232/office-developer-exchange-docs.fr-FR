---
title: IsPrivate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsPrivate
api_type:
- schema
ms.assetid: 1712bc94-9789-4507-8521-bde1be51e331
description: L’élément IsPrivate indique si l’élément de calendrier est privé.
ms.openlocfilehash: 37c0357b3eab2314ee74e1c98287b3dc05a3bf26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828095"
---
# <a name="isprivate"></a><span data-ttu-id="fdeeb-103">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="fdeeb-103">IsPrivate</span></span>

<span data-ttu-id="fdeeb-104">L’élément **IsPrivate** indique si l’élément de calendrier est privé.</span><span class="sxs-lookup"><span data-stu-id="fdeeb-104">The **IsPrivate** element indicates whether the calendar item is private.</span></span> 
  
[<span data-ttu-id="fdeeb-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fdeeb-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="fdeeb-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="fdeeb-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="fdeeb-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="fdeeb-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="fdeeb-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="fdeeb-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="fdeeb-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="fdeeb-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="fdeeb-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="fdeeb-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="fdeeb-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="fdeeb-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="fdeeb-112">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="fdeeb-112">IsPrivate</span></span>](isprivate.md)
  
```xml
<IsPrivate>true or false</IsPrivate>
```

 <span data-ttu-id="fdeeb-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="fdeeb-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fdeeb-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fdeeb-114">Attributes and elements</span></span>

<span data-ttu-id="fdeeb-115">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fdeeb-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fdeeb-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="fdeeb-116">Attributes</span></span>

<span data-ttu-id="fdeeb-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fdeeb-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fdeeb-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fdeeb-118">Child elements</span></span>

<span data-ttu-id="fdeeb-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fdeeb-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fdeeb-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fdeeb-120">Parent elements</span></span>

|<span data-ttu-id="fdeeb-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fdeeb-121">**Element**</span></span>|<span data-ttu-id="fdeeb-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="fdeeb-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fdeeb-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="fdeeb-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="fdeeb-124">Fournit des informations supplémentaires sur un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="fdeeb-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="fdeeb-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="fdeeb-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fdeeb-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="fdeeb-126">Text value</span></span>

<span data-ttu-id="fdeeb-127">Une valeur de texte qui représente une valeur Boolean est requise.</span><span class="sxs-lookup"><span data-stu-id="fdeeb-127">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fdeeb-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="fdeeb-128">Remarks</span></span>

<span data-ttu-id="fdeeb-129">Si cet élément est utilisé, les autres éléments dans l’élément [CalendarEventDetails](calendareventdetails.md) ne seront pas être incluses dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="fdeeb-129">If this element is used, the other elements in the [CalendarEventDetails](calendareventdetails.md) element will not be included in the response.</span></span> 
  
<span data-ttu-id="fdeeb-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fdeeb-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fdeeb-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fdeeb-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fdeeb-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fdeeb-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fdeeb-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fdeeb-133">Schema Name</span></span>  <br/> |<span data-ttu-id="fdeeb-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fdeeb-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="fdeeb-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fdeeb-135">Validation File</span></span>  <br/> |<span data-ttu-id="fdeeb-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fdeeb-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fdeeb-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fdeeb-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="fdeeb-138">False</span><span class="sxs-lookup"><span data-stu-id="fdeeb-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fdeeb-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fdeeb-139">See also</span></span>



[<span data-ttu-id="fdeeb-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="fdeeb-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="fdeeb-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fdeeb-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="fdeeb-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="fdeeb-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

