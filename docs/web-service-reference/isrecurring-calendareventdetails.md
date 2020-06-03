---
title: IsRecurring (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: 42323940-0ccb-4a05-86e4-262bde5e41b0
description: L’élément IsRecurring indique si l’événement de calendrier est une instance d’un élément de calendrier périodique ou un élément de calendrier unique.
ms.openlocfilehash: f9a9c8b4d2a20d42dbec7cd6fd36935eb0b941f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530252"
---
# <a name="isrecurring-calendareventdetails"></a><span data-ttu-id="bf4a8-103">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="bf4a8-103">IsRecurring (CalendarEventDetails)</span></span>

<span data-ttu-id="bf4a8-104">L’élément **IsRecurring** indique si l’événement de calendrier est une instance d’un élément de calendrier périodique ou un élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="bf4a8-104">The **IsRecurring** element indicates whether the calendar event is an instance of a recurring calendar item or a single calendar item.</span></span> 
  
[<span data-ttu-id="bf4a8-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bf4a8-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="bf4a8-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="bf4a8-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="bf4a8-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="bf4a8-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="bf4a8-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="bf4a8-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="bf4a8-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="bf4a8-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="bf4a8-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="bf4a8-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="bf4a8-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="bf4a8-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="bf4a8-112">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="bf4a8-112">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
  
```xml
<IsRecurring>true or false</IsRecurring>
```

 <span data-ttu-id="bf4a8-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="bf4a8-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bf4a8-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bf4a8-114">Attributes and elements</span></span>

<span data-ttu-id="bf4a8-115">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bf4a8-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf4a8-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="bf4a8-116">Attributes</span></span>

<span data-ttu-id="bf4a8-117">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bf4a8-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf4a8-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bf4a8-118">Child elements</span></span>

<span data-ttu-id="bf4a8-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bf4a8-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bf4a8-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bf4a8-120">Parent elements</span></span>

|<span data-ttu-id="bf4a8-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bf4a8-121">**Element**</span></span>|<span data-ttu-id="bf4a8-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="bf4a8-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf4a8-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="bf4a8-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="bf4a8-124">Fournit des informations supplémentaires sur un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="bf4a8-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="bf4a8-125">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="bf4a8-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bf4a8-126">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="bf4a8-126">Text value</span></span>

<span data-ttu-id="bf4a8-127">Une valeur de texte est requise si cet élément est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="bf4a8-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="bf4a8-128">Cet élément est requis si l’élément [CalendarEventDetails](calendareventdetails.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="bf4a8-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bf4a8-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="bf4a8-129">Remarks</span></span>

<span data-ttu-id="bf4a8-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="bf4a8-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf4a8-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bf4a8-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf4a8-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bf4a8-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf4a8-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bf4a8-133">Schema Name</span></span>  <br/> |<span data-ttu-id="bf4a8-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bf4a8-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="bf4a8-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bf4a8-135">Validation File</span></span>  <br/> |<span data-ttu-id="bf4a8-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bf4a8-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf4a8-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bf4a8-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="bf4a8-138">False</span><span class="sxs-lookup"><span data-stu-id="bf4a8-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf4a8-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bf4a8-139">See also</span></span>



[<span data-ttu-id="bf4a8-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="bf4a8-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="bf4a8-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bf4a8-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="bf4a8-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="bf4a8-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

