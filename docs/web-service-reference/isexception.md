---
title: IsException
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsException
api_type:
- schema
ms.assetid: e7bd8ae2-2643-411e-ae08-358bac445800
description: L’élément IsException indique si une instance d’un élément de calendrier périodique est modifiée à partir de la forme de base.
ms.openlocfilehash: bb884110fd3642bebbc03504aef369f9e0412714
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828009"
---
# <a name="isexception"></a><span data-ttu-id="456ef-103">IsException</span><span class="sxs-lookup"><span data-stu-id="456ef-103">IsException</span></span>

<span data-ttu-id="456ef-104">L’élément **IsException** indique si une instance d’un élément de calendrier périodique est modifiée à partir de la forme de base.</span><span class="sxs-lookup"><span data-stu-id="456ef-104">The **IsException** element indicates whether an instance of a recurring calendar item is changed from the master.</span></span> 
  
[<span data-ttu-id="456ef-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="456ef-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="456ef-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="456ef-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="456ef-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="456ef-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="456ef-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="456ef-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="456ef-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="456ef-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="456ef-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="456ef-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="456ef-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="456ef-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="456ef-112">IsException</span><span class="sxs-lookup"><span data-stu-id="456ef-112">IsException</span></span>](isexception.md)
  
```xml
<IsException/>
```

 <span data-ttu-id="456ef-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="456ef-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="456ef-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="456ef-114">Attributes and elements</span></span>

<span data-ttu-id="456ef-115">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="456ef-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="456ef-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="456ef-116">Attributes</span></span>

<span data-ttu-id="456ef-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="456ef-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="456ef-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="456ef-118">Child elements</span></span>

<span data-ttu-id="456ef-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="456ef-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="456ef-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="456ef-120">Parent elements</span></span>

|<span data-ttu-id="456ef-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="456ef-121">**Element**</span></span>|<span data-ttu-id="456ef-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="456ef-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="456ef-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="456ef-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="456ef-124">Fournit des informations supplémentaires sur un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="456ef-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="456ef-125">Vous trouverez ci-dessous l’expression XPath 2.0 pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="456ef-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="456ef-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="456ef-126">Text value</span></span>

<span data-ttu-id="456ef-127">Une valeur de texte est obligatoire si cet élément est retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="456ef-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="456ef-128">Cet élément est obligatoire si l’élément [CalendarEventDetails](calendareventdetails.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="456ef-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="456ef-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="456ef-129">Remarks</span></span>

<span data-ttu-id="456ef-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="456ef-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="456ef-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="456ef-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="456ef-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="456ef-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="456ef-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="456ef-133">Schema Name</span></span>  <br/> |<span data-ttu-id="456ef-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="456ef-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="456ef-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="456ef-135">Validation File</span></span>  <br/> |<span data-ttu-id="456ef-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="456ef-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="456ef-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="456ef-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="456ef-138">False</span><span class="sxs-lookup"><span data-stu-id="456ef-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="456ef-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="456ef-139">See also</span></span>



[<span data-ttu-id="456ef-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="456ef-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="456ef-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="456ef-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="456ef-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="456ef-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

