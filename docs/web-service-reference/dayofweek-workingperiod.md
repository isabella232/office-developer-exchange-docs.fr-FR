---
title: DayOfWeek (WorkingPeriod)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 7a8a8cc1-392b-4db5-bb76-710477e31396
description: L’élément DayOfWeek contient la liste des jours de travail planifié pour l’utilisateur de boîte aux lettres.
ms.openlocfilehash: a6a68017291ba13f45b3970307669222d583fcbb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755826"
---
# <a name="dayofweek-workingperiod"></a><span data-ttu-id="5fb55-103">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="5fb55-103">DayOfWeek (WorkingPeriod)</span></span>

<span data-ttu-id="5fb55-104">L’élément **DayOfWeek** contient la liste des jours de travail planifié pour l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5fb55-104">The **DayOfWeek** element contains the list of working days scheduled for the mailbox user.</span></span> 
  
- [<span data-ttu-id="5fb55-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="5fb55-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="5fb55-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="5fb55-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)  
- [<span data-ttu-id="5fb55-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="5fb55-107">FreeBusyResponse</span></span>](freebusyresponse.md)  
- [<span data-ttu-id="5fb55-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="5fb55-108">FreeBusyView</span></span>](freebusyview.md)  
- [<span data-ttu-id="5fb55-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="5fb55-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)  
- [<span data-ttu-id="5fb55-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="5fb55-110">WorkingPeriodArray</span></span>](workingperiodarray.md) 
- [<span data-ttu-id="5fb55-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="5fb55-111">WorkingPeriod</span></span>](workingperiod.md)  
- [<span data-ttu-id="5fb55-112">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="5fb55-112">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
  
```xml
<DayOfWeek>Sunday Monday Tuesday Wednesday Thursday Friday Saturday</DayOfWeek>
```

<span data-ttu-id="5fb55-113">**DaysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="5fb55-113">**DaysOfWeek**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5fb55-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5fb55-114">Attributes and elements</span></span>

<span data-ttu-id="5fb55-115">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5fb55-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5fb55-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="5fb55-116">Attributes</span></span>

<span data-ttu-id="5fb55-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5fb55-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5fb55-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5fb55-118">Child elements</span></span>

<span data-ttu-id="5fb55-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5fb55-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5fb55-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5fb55-120">Parent elements</span></span>

|<span data-ttu-id="5fb55-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5fb55-121">**Element**</span></span>|<span data-ttu-id="5fb55-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="5fb55-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fb55-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="5fb55-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="5fb55-124">Contient la semaine de travail les jours et les heures de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5fb55-124">Contains the work week days and hours of the mailbox user.</span></span><br/><br/><span data-ttu-id="5fb55-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="5fb55-125">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5fb55-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5fb55-126">Text value</span></span>

<span data-ttu-id="5fb55-127">Une valeur de texte est renvoyée si l’utilisateur de boîte aux lettres a jours définissez pour représenter la semaine de travail.</span><span class="sxs-lookup"><span data-stu-id="5fb55-127">A text value is returned if the mailbox user has days set to represent the work week.</span></span> <span data-ttu-id="5fb55-128">Les valeurs possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="5fb55-128">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="5fb55-129">Dimanche</span><span class="sxs-lookup"><span data-stu-id="5fb55-129">Sunday</span></span>    
- <span data-ttu-id="5fb55-130">Lundi</span><span class="sxs-lookup"><span data-stu-id="5fb55-130">Monday</span></span>    
- <span data-ttu-id="5fb55-131">Mardi</span><span class="sxs-lookup"><span data-stu-id="5fb55-131">Tuesday</span></span>    
- <span data-ttu-id="5fb55-132">Mercredi</span><span class="sxs-lookup"><span data-stu-id="5fb55-132">Wednesday</span></span>    
- <span data-ttu-id="5fb55-133">Jeudi</span><span class="sxs-lookup"><span data-stu-id="5fb55-133">Thursday</span></span>    
- <span data-ttu-id="5fb55-134">Vendredi</span><span class="sxs-lookup"><span data-stu-id="5fb55-134">Friday</span></span>    
- <span data-ttu-id="5fb55-135">Samedi</span><span class="sxs-lookup"><span data-stu-id="5fb55-135">Saturday</span></span> 
    
<span data-ttu-id="5fb55-136">Les valeurs de texte seront afficheront dans l’ordre.</span><span class="sxs-lookup"><span data-stu-id="5fb55-136">The text values will be returned in that order.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5fb55-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="5fb55-137">Remarks</span></span>

<span data-ttu-id="5fb55-138">Il est important de noter que la différence entre cet élément et l’élément disponibilité [DayOfWeek (fuseau horaire)](dayofweek-timezone.md) est le type.</span><span class="sxs-lookup"><span data-stu-id="5fb55-138">It is important to note that the difference between this element and the Availability [DayOfWeek (TimeZone)](dayofweek-timezone.md) element is the type.</span></span> 
  
<span data-ttu-id="5fb55-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5fb55-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5fb55-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5fb55-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5fb55-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5fb55-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5fb55-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5fb55-142">Schema Name</span></span>  <br/> |<span data-ttu-id="5fb55-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5fb55-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="5fb55-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5fb55-144">Validation File</span></span>  <br/> |<span data-ttu-id="5fb55-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5fb55-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5fb55-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5fb55-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="5fb55-147">False</span><span class="sxs-lookup"><span data-stu-id="5fb55-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5fb55-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5fb55-148">See also</span></span>

- [<span data-ttu-id="5fb55-149">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="5fb55-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="5fb55-150">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="5fb55-150">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="5fb55-151">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="5fb55-151">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

