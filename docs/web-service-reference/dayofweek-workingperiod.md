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
description: L’élément DayOfWeek contient la liste des jours ouvrés planifiés pour l’utilisateur de la boîte aux lettres.
ms.openlocfilehash: 06d4a7d5541b3b71fcbf9be9beb7512d06853283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457444"
---
# <a name="dayofweek-workingperiod"></a><span data-ttu-id="a2fe9-103">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="a2fe9-103">DayOfWeek (WorkingPeriod)</span></span>

<span data-ttu-id="a2fe9-104">L’élément **DayOfWeek** contient la liste des jours ouvrés planifiés pour l’utilisateur de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a2fe9-104">The **DayOfWeek** element contains the list of working days scheduled for the mailbox user.</span></span> 
  
- [<span data-ttu-id="a2fe9-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a2fe9-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="a2fe9-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="a2fe9-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)  
- [<span data-ttu-id="a2fe9-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="a2fe9-107">FreeBusyResponse</span></span>](freebusyresponse.md)  
- [<span data-ttu-id="a2fe9-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="a2fe9-108">FreeBusyView</span></span>](freebusyview.md)  
- [<span data-ttu-id="a2fe9-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="a2fe9-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)  
- [<span data-ttu-id="a2fe9-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="a2fe9-110">WorkingPeriodArray</span></span>](workingperiodarray.md) 
- [<span data-ttu-id="a2fe9-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="a2fe9-111">WorkingPeriod</span></span>](workingperiod.md)  
- [<span data-ttu-id="a2fe9-112">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="a2fe9-112">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
  
```xml
<DayOfWeek>Sunday Monday Tuesday Wednesday Thursday Friday Saturday</DayOfWeek>
```

<span data-ttu-id="a2fe9-113">**DaysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="a2fe9-113">**DaysOfWeek**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a2fe9-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a2fe9-114">Attributes and elements</span></span>

<span data-ttu-id="a2fe9-115">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a2fe9-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2fe9-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="a2fe9-116">Attributes</span></span>

<span data-ttu-id="a2fe9-117">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a2fe9-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2fe9-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a2fe9-118">Child elements</span></span>

<span data-ttu-id="a2fe9-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a2fe9-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a2fe9-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a2fe9-120">Parent elements</span></span>

|<span data-ttu-id="a2fe9-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a2fe9-121">**Element**</span></span>|<span data-ttu-id="a2fe9-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="a2fe9-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2fe9-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="a2fe9-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="a2fe9-124">Contient les jours et les heures de travail de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a2fe9-124">Contains the work week days and hours of the mailbox user.</span></span><br/><br/><span data-ttu-id="a2fe9-125">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="a2fe9-125">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a2fe9-126">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="a2fe9-126">Text value</span></span>

<span data-ttu-id="a2fe9-127">Une valeur de texte est renvoyée si l’utilisateur de la boîte aux lettres a défini des jours pour représenter la semaine de travail.</span><span class="sxs-lookup"><span data-stu-id="a2fe9-127">A text value is returned if the mailbox user has days set to represent the work week.</span></span> <span data-ttu-id="a2fe9-128">Les valeurs possibles pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="a2fe9-128">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="a2fe9-129">Warm</span><span class="sxs-lookup"><span data-stu-id="a2fe9-129">Sunday</span></span>    
- <span data-ttu-id="a2fe9-130">Lundi</span><span class="sxs-lookup"><span data-stu-id="a2fe9-130">Monday</span></span>    
- <span data-ttu-id="a2fe9-131">Mardi</span><span class="sxs-lookup"><span data-stu-id="a2fe9-131">Tuesday</span></span>    
- <span data-ttu-id="a2fe9-132">Mercredi</span><span class="sxs-lookup"><span data-stu-id="a2fe9-132">Wednesday</span></span>    
- <span data-ttu-id="a2fe9-133">Jeudi</span><span class="sxs-lookup"><span data-stu-id="a2fe9-133">Thursday</span></span>    
- <span data-ttu-id="a2fe9-134">Vendredi</span><span class="sxs-lookup"><span data-stu-id="a2fe9-134">Friday</span></span>    
- <span data-ttu-id="a2fe9-135">Samedi</span><span class="sxs-lookup"><span data-stu-id="a2fe9-135">Saturday</span></span> 
    
<span data-ttu-id="a2fe9-136">Les valeurs de texte sont renvoyées dans cet ordre.</span><span class="sxs-lookup"><span data-stu-id="a2fe9-136">The text values will be returned in that order.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a2fe9-137">Remarques</span><span class="sxs-lookup"><span data-stu-id="a2fe9-137">Remarks</span></span>

<span data-ttu-id="a2fe9-138">Il est important de noter que la différence entre cet élément et l’élément Availability [DayOfWeek (TimeZone)](dayofweek-timezone.md) est le type.</span><span class="sxs-lookup"><span data-stu-id="a2fe9-138">It is important to note that the difference between this element and the Availability [DayOfWeek (TimeZone)](dayofweek-timezone.md) element is the type.</span></span> 
  
<span data-ttu-id="a2fe9-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a2fe9-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2fe9-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a2fe9-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2fe9-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a2fe9-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2fe9-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a2fe9-142">Schema Name</span></span>  <br/> |<span data-ttu-id="a2fe9-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a2fe9-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="a2fe9-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a2fe9-144">Validation File</span></span>  <br/> |<span data-ttu-id="a2fe9-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a2fe9-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2fe9-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a2fe9-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2fe9-147">False</span><span class="sxs-lookup"><span data-stu-id="a2fe9-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2fe9-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a2fe9-148">See also</span></span>

- [<span data-ttu-id="a2fe9-149">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a2fe9-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="a2fe9-150">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a2fe9-150">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="a2fe9-151">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="a2fe9-151">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

