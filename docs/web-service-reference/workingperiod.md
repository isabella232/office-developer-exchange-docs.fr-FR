---
title: WorkingPeriod
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriod
api_type:
- schema
ms.assetid: 3b4e48af-9880-42b9-a0dc-dae7ac43c264
description: L’élément WorkingPeriod contient la semaine de travail jours et les heures de l’utilisateur de boîte aux lettres.
ms.openlocfilehash: 0f2707bede5e49174ed62a35ba704e39c0c48e9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839068"
---
# <a name="workingperiod"></a><span data-ttu-id="47634-103">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="47634-103">WorkingPeriod</span></span>

<span data-ttu-id="47634-104">L’élément **WorkingPeriod** contient la semaine de travail jours et les heures de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="47634-104">The **WorkingPeriod** element contains the work week days and hours of the mailbox user.</span></span> 
  
[<span data-ttu-id="47634-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="47634-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="47634-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="47634-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="47634-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="47634-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="47634-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="47634-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="47634-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="47634-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="47634-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="47634-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="47634-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="47634-111">WorkingPeriod</span></span>](workingperiod.md)
  
```xml
<WorkingPeriod>
   <DayOfWeek>...</DayOfWeek>
   <StartTimeInMinutes>...</StartTimeInMinutes>
   <EndTimeInMinutes>...</EndTimeInMinutes>
</WorkingPeriod>
```

 <span data-ttu-id="47634-112">**WorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="47634-112">**WorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47634-113">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="47634-113">Attributes and elements</span></span>

<span data-ttu-id="47634-114">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="47634-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47634-115">Attributs</span><span class="sxs-lookup"><span data-stu-id="47634-115">Attributes</span></span>

<span data-ttu-id="47634-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="47634-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47634-117">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="47634-117">Child elements</span></span>

|<span data-ttu-id="47634-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="47634-118">**Element**</span></span>|<span data-ttu-id="47634-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="47634-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47634-120">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="47634-120">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md) <br/> |<span data-ttu-id="47634-121">Contient la liste des jours de travail planifié pour l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="47634-121">Contains the list of working days scheduled for the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="47634-122">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="47634-122">StartTimeInMinutes</span></span>](starttimeinminutes.md) <br/> |<span data-ttu-id="47634-123">Représente le début de la journée de travail pour un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="47634-123">Represents the start of the working day for a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="47634-124">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="47634-124">EndTimeInMinutes</span></span>](endtimeinminutes.md) <br/> |<span data-ttu-id="47634-125">Représente la fin de la journée de travail pour un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="47634-125">Represents the end of the working day for a mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47634-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="47634-126">Parent elements</span></span>

|<span data-ttu-id="47634-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="47634-127">**Element**</span></span>|<span data-ttu-id="47634-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="47634-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47634-129">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="47634-129">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="47634-130">Contient des informations sur les périodes de l’utilisateur de boîte aux lettres de travail.</span><span class="sxs-lookup"><span data-stu-id="47634-130">Contains working period information for the mailbox user.</span></span>  <br/> <span data-ttu-id="47634-131">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="47634-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="47634-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="47634-132">Remarks</span></span>

<span data-ttu-id="47634-133">Tous les éléments enfants sont répertoriés dans l’ordre dans lequel elles se produisent.</span><span class="sxs-lookup"><span data-stu-id="47634-133">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="47634-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="47634-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47634-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="47634-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47634-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="47634-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="47634-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="47634-137">Schema Name</span></span>  <br/> |<span data-ttu-id="47634-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="47634-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="47634-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="47634-139">Validation File</span></span>  <br/> |<span data-ttu-id="47634-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="47634-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="47634-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="47634-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="47634-142">False</span><span class="sxs-lookup"><span data-stu-id="47634-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47634-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="47634-143">See also</span></span>



[<span data-ttu-id="47634-144">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="47634-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="47634-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="47634-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="47634-146">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="47634-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

