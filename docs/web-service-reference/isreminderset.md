---
title: IsReminderSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReminderSet
api_type:
- schema
ms.assetid: 6aea4cb7-ca14-4949-8e7f-660b565f6556
description: L’élément IsReminderSet indique si un rappel a été défini pour l’événement de calendrier.
ms.openlocfilehash: 589178072baca652bff2779e64a212fb90478247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828100"
---
# <a name="isreminderset"></a><span data-ttu-id="0faf7-103">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="0faf7-103">IsReminderSet</span></span>

<span data-ttu-id="0faf7-104">L’élément **IsReminderSet** indique si un rappel a été défini pour l’événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0faf7-104">The **IsReminderSet** element indicates whether a reminder has been set for the calendar event.</span></span> 
  
[<span data-ttu-id="0faf7-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0faf7-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="0faf7-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="0faf7-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="0faf7-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="0faf7-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="0faf7-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="0faf7-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="0faf7-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="0faf7-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="0faf7-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="0faf7-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="0faf7-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="0faf7-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="0faf7-112">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="0faf7-112">IsReminderSet</span></span>](isreminderset.md)
  
```xml
<IsReminderSet>true or false</IsReminderSet>
```

 <span data-ttu-id="0faf7-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="0faf7-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0faf7-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0faf7-114">Attributes and elements</span></span>

<span data-ttu-id="0faf7-115">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0faf7-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0faf7-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="0faf7-116">Attributes</span></span>

<span data-ttu-id="0faf7-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0faf7-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0faf7-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0faf7-118">Child elements</span></span>

<span data-ttu-id="0faf7-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0faf7-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0faf7-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0faf7-120">Parent elements</span></span>

|<span data-ttu-id="0faf7-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0faf7-121">**Element**</span></span>|<span data-ttu-id="0faf7-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="0faf7-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0faf7-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="0faf7-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="0faf7-124">Fournit des informations supplémentaires sur un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0faf7-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="0faf7-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="0faf7-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0faf7-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0faf7-126">Text value</span></span>

<span data-ttu-id="0faf7-127">Une valeur de texte est obligatoire si cet élément est retourné dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="0faf7-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="0faf7-128">Cet élément est obligatoire si l’élément [CalendarEventDetails](calendareventdetails.md) est utilisé, sauf si l’élément [IsPrivate](isprivate.md) est défini sur **true**.</span><span class="sxs-lookup"><span data-stu-id="0faf7-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used unless the [IsPrivate](isprivate.md) element is set to **true**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0faf7-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="0faf7-129">Remarks</span></span>

<span data-ttu-id="0faf7-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0faf7-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0faf7-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0faf7-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0faf7-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0faf7-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0faf7-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0faf7-133">Schema Name</span></span>  <br/> |<span data-ttu-id="0faf7-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0faf7-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="0faf7-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0faf7-135">Validation File</span></span>  <br/> |<span data-ttu-id="0faf7-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0faf7-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0faf7-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0faf7-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="0faf7-138">False</span><span class="sxs-lookup"><span data-stu-id="0faf7-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0faf7-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0faf7-139">See also</span></span>



[<span data-ttu-id="0faf7-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0faf7-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="0faf7-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0faf7-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="0faf7-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="0faf7-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

