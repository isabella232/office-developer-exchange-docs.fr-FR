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
description: L’élément location représente le champ d’emplacement de l’élément de calendrier.
ms.openlocfilehash: 4a590c315d2211ce9128305a514e68f1c785596c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467997"
---
# <a name="location-calendareventdetails"></a><span data-ttu-id="12aff-103">Emplacement (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="12aff-103">Location (CalendarEventDetails)</span></span>

<span data-ttu-id="12aff-104">L’élément **location** représente le champ d’emplacement de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="12aff-104">The **Location** element represents the location field of the calendar item.</span></span> 
  
[<span data-ttu-id="12aff-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="12aff-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="12aff-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="12aff-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="12aff-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="12aff-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="12aff-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="12aff-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="12aff-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="12aff-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="12aff-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="12aff-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="12aff-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="12aff-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="12aff-112">Emplacement (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="12aff-112">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
  
```xml
<Location/>
```

 <span data-ttu-id="12aff-113">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="12aff-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12aff-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="12aff-114">Attributes and elements</span></span>

<span data-ttu-id="12aff-115">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="12aff-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12aff-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="12aff-116">Attributes</span></span>

<span data-ttu-id="12aff-117">Aucune.</span><span class="sxs-lookup"><span data-stu-id="12aff-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12aff-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="12aff-118">Child elements</span></span>

<span data-ttu-id="12aff-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="12aff-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12aff-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="12aff-120">Parent elements</span></span>

|<span data-ttu-id="12aff-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="12aff-121">**Element**</span></span>|<span data-ttu-id="12aff-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="12aff-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12aff-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="12aff-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="12aff-124">Fournit des informations supplémentaires pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="12aff-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="12aff-125">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="12aff-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12aff-126">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="12aff-126">Text value</span></span>

<span data-ttu-id="12aff-127">Une valeur de texte est requise si cet élément est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="12aff-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="12aff-128">Cet élément peut contenir une chaîne vide.</span><span class="sxs-lookup"><span data-stu-id="12aff-128">This element can contain an empty string.</span></span> <span data-ttu-id="12aff-129">Cet élément est facultatif si l’élément [CalendarEventDetails](calendareventdetails.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="12aff-129">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="12aff-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="12aff-130">Remarks</span></span>

<span data-ttu-id="12aff-131">Cet élément est mappé à une propriété nommée MAPI PR_Location.</span><span class="sxs-lookup"><span data-stu-id="12aff-131">This element maps to a PR_Location MAPI named property.</span></span>
  
<span data-ttu-id="12aff-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="12aff-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12aff-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="12aff-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12aff-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="12aff-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12aff-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="12aff-135">Schema Name</span></span>  <br/> |<span data-ttu-id="12aff-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="12aff-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="12aff-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="12aff-137">Validation File</span></span>  <br/> |<span data-ttu-id="12aff-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="12aff-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12aff-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="12aff-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="12aff-140">False</span><span class="sxs-lookup"><span data-stu-id="12aff-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12aff-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="12aff-141">See also</span></span>



[<span data-ttu-id="12aff-142">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="12aff-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="12aff-143">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="12aff-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="12aff-144">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="12aff-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

