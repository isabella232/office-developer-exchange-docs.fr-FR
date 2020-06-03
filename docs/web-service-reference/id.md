---
title: ID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ID
api_type:
- schema
ms.assetid: 8caf922f-56bd-466a-a68f-d6cb236f2eec
description: L’élément ID représente l’ID d’entrée de l’élément de calendrier.
ms.openlocfilehash: 429413bbfb0206effc3ea97eb11527449c67211c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456485"
---
# <a name="id"></a><span data-ttu-id="143e2-103">ID</span><span class="sxs-lookup"><span data-stu-id="143e2-103">ID</span></span>

<span data-ttu-id="143e2-104">L’élément **ID** représente l’ID d’entrée de l’élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="143e2-104">The **ID** element represents the entry ID of the calendar item.</span></span> 
  
[<span data-ttu-id="143e2-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="143e2-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="143e2-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="143e2-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="143e2-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="143e2-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="143e2-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="143e2-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="143e2-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="143e2-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="143e2-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="143e2-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="143e2-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="143e2-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="143e2-112">ID</span><span class="sxs-lookup"><span data-stu-id="143e2-112">ID</span></span>](id.md)
  
```xml
<ID>...</ID>
```

 <span data-ttu-id="143e2-113">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="143e2-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="143e2-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="143e2-114">Attributes and elements</span></span>

<span data-ttu-id="143e2-115">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="143e2-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="143e2-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="143e2-116">Attributes</span></span>

<span data-ttu-id="143e2-117">Aucune.</span><span class="sxs-lookup"><span data-stu-id="143e2-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="143e2-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="143e2-118">Child elements</span></span>

<span data-ttu-id="143e2-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="143e2-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="143e2-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="143e2-120">Parent elements</span></span>

|<span data-ttu-id="143e2-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="143e2-121">**Element**</span></span>|<span data-ttu-id="143e2-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="143e2-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="143e2-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="143e2-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="143e2-124">Fournit des informations supplémentaires pour un événement de calendrier.</span><span class="sxs-lookup"><span data-stu-id="143e2-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="143e2-125">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="143e2-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="143e2-126">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="143e2-126">Text value</span></span>

<span data-ttu-id="143e2-127">Une valeur de texte est requise si cet élément est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="143e2-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="143e2-128">Cet élément est requis si l’élément [CalendarEventDetails](calendareventdetails.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="143e2-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="143e2-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="143e2-129">Remarks</span></span>

<span data-ttu-id="143e2-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="143e2-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="143e2-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="143e2-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="143e2-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="143e2-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="143e2-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="143e2-133">Schema Name</span></span>  <br/> |<span data-ttu-id="143e2-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="143e2-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="143e2-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="143e2-135">Validation File</span></span>  <br/> |<span data-ttu-id="143e2-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="143e2-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="143e2-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="143e2-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="143e2-138">False</span><span class="sxs-lookup"><span data-stu-id="143e2-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="143e2-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="143e2-139">See also</span></span>



[<span data-ttu-id="143e2-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="143e2-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="143e2-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="143e2-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="143e2-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="143e2-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

