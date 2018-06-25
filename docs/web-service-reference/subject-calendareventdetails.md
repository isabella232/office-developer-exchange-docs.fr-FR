---
title: Sujet (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subject
api_type:
- schema
ms.assetid: 05e955b5-8e90-4043-b06b-6ce523eaed9b
description: L’élément Subject représente l’objet d’un élément de calendrier.
ms.openlocfilehash: 5303a7568e017999f2be69c50588832748b5668a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829610"
---
# <a name="subject-calendareventdetails"></a><span data-ttu-id="ba20b-103">Sujet (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="ba20b-103">Subject (CalendarEventDetails)</span></span>

<span data-ttu-id="ba20b-104">L’élément **Subject** représente l’objet d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ba20b-104">The **Subject** element represents the subject of a calendar item.</span></span> 
  
[<span data-ttu-id="ba20b-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ba20b-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="ba20b-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="ba20b-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="ba20b-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="ba20b-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="ba20b-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="ba20b-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="ba20b-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="ba20b-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="ba20b-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="ba20b-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="ba20b-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="ba20b-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="ba20b-112">Sujet (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="ba20b-112">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md)
  
```xml
<Subject/>
```

 <span data-ttu-id="ba20b-113">**string**</span><span class="sxs-lookup"><span data-stu-id="ba20b-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba20b-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ba20b-114">Attributes and elements</span></span>

<span data-ttu-id="ba20b-115">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ba20b-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba20b-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="ba20b-116">Attributes</span></span>

<span data-ttu-id="ba20b-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba20b-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ba20b-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ba20b-118">Child elements</span></span>

<span data-ttu-id="ba20b-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ba20b-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba20b-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ba20b-120">Parent elements</span></span>

|<span data-ttu-id="ba20b-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ba20b-121">**Element**</span></span>|<span data-ttu-id="ba20b-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="ba20b-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ba20b-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="ba20b-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="ba20b-124">Fournit des informations supplémentaires pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="ba20b-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="ba20b-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="ba20b-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ba20b-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ba20b-126">Text value</span></span>

<span data-ttu-id="ba20b-127">Une valeur de texte est obligatoire si cet élément est retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="ba20b-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="ba20b-128">Cet élément ne sera pas retourné si la valeur de l’élément [IsPrivate](isprivate.md) est égale à **true**.</span><span class="sxs-lookup"><span data-stu-id="ba20b-128">This element will not be returned if the [IsPrivate](isprivate.md) element value is equal to **true**.</span></span> <span data-ttu-id="ba20b-129">Cet élément peut contenir une chaîne vide.</span><span class="sxs-lookup"><span data-stu-id="ba20b-129">This element can contain an empty string.</span></span> <span data-ttu-id="ba20b-130">Cet élément est facultatif si l’élément [CalendarEventDetails](calendareventdetails.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="ba20b-130">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ba20b-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="ba20b-131">Remarks</span></span>

<span data-ttu-id="ba20b-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ba20b-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba20b-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ba20b-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba20b-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ba20b-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba20b-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ba20b-135">Schema Name</span></span>  <br/> |<span data-ttu-id="ba20b-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ba20b-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba20b-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ba20b-137">Validation File</span></span>  <br/> |<span data-ttu-id="ba20b-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ba20b-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba20b-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ba20b-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba20b-140">False</span><span class="sxs-lookup"><span data-stu-id="ba20b-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba20b-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ba20b-141">See also</span></span>



[<span data-ttu-id="ba20b-142">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ba20b-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="ba20b-143">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ba20b-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="ba20b-144">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="ba20b-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

