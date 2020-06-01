---
title: IsMeeting (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: dd6900e4-e4a3-471a-909d-7240ebec501b
description: L’élément IsMeeting indique si l’événement de calendrier est une réunion ou un rendez-vous.
ms.openlocfilehash: b75dfba203177d6451f3847bf8d1f68014612e1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465995"
---
# <a name="ismeeting-calendareventdetails"></a><span data-ttu-id="9262c-103">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="9262c-103">IsMeeting (CalendarEventDetails)</span></span>

<span data-ttu-id="9262c-104">L’élément **IsMeeting** indique si l’événement de calendrier est une réunion ou un rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="9262c-104">The **IsMeeting** element indicates whether the calendar event is a meeting or an appointment.</span></span> 
  
[<span data-ttu-id="9262c-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="9262c-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="9262c-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="9262c-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="9262c-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="9262c-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="9262c-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="9262c-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="9262c-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="9262c-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="9262c-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="9262c-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="9262c-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="9262c-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="9262c-112">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="9262c-112">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
  
```xml
<IsMeeting>true or false</IsMeeting>
```

 <span data-ttu-id="9262c-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="9262c-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9262c-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9262c-114">Attributes and elements</span></span>

<span data-ttu-id="9262c-115">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9262c-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9262c-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="9262c-116">Attributes</span></span>

<span data-ttu-id="9262c-117">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9262c-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9262c-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9262c-118">Child elements</span></span>

<span data-ttu-id="9262c-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9262c-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9262c-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9262c-120">Parent elements</span></span>

|<span data-ttu-id="9262c-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9262c-121">**Element**</span></span>|<span data-ttu-id="9262c-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="9262c-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9262c-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="9262c-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="9262c-124">Fournit des informations supplémentaires pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="9262c-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="9262c-125">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="9262c-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9262c-126">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="9262c-126">Text value</span></span>

<span data-ttu-id="9262c-127">Une valeur de texte est requise si cet élément est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="9262c-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="9262c-128">Cet élément est requis si l’élément [CalendarEventDetails](calendareventdetails.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="9262c-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9262c-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="9262c-129">Remarks</span></span>

<span data-ttu-id="9262c-130">La différence entre une réunion et un rendez-vous est qu’une réunion est un élément de calendrier qui inclut des participants ; un rendez-vous est un élément de calendrier qui n’inclut pas de participants.</span><span class="sxs-lookup"><span data-stu-id="9262c-130">The difference between a meeting and an appointment is that a meeting is a calendar item that includes attendees; an appointment is a calendar item that does not include attendees.</span></span>
  
<span data-ttu-id="9262c-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="9262c-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9262c-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9262c-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9262c-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9262c-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9262c-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9262c-134">Schema Name</span></span>  <br/> |<span data-ttu-id="9262c-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9262c-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="9262c-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9262c-136">Validation File</span></span>  <br/> |<span data-ttu-id="9262c-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9262c-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9262c-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9262c-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="9262c-139">False</span><span class="sxs-lookup"><span data-stu-id="9262c-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9262c-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9262c-140">See also</span></span>



[<span data-ttu-id="9262c-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="9262c-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="9262c-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="9262c-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="9262c-143">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="9262c-143">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

