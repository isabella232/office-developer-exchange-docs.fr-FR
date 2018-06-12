---
title: WorkingPeriodArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriodArray
api_type:
- schema
ms.assetid: 3a3f6393-eacc-4734-b6c9-b67023fe2830
description: L’élément WorkingPeriodArray contient l’utilisation des informations sur les périodes de l’utilisateur de boîte aux lettres.
ms.openlocfilehash: 02712f05dc3373a532d769f476341b78ad25a79c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839067"
---
# <a name="workingperiodarray"></a><span data-ttu-id="d02e6-103">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="d02e6-103">WorkingPeriodArray</span></span>

<span data-ttu-id="d02e6-104">L’élément **WorkingPeriodArray** contient l’utilisation des informations sur les périodes de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d02e6-104">The **WorkingPeriodArray** element contains working period information for the mailbox user.</span></span> 
  
[<span data-ttu-id="d02e6-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d02e6-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d02e6-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="d02e6-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="d02e6-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="d02e6-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="d02e6-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="d02e6-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="d02e6-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="d02e6-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="d02e6-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="d02e6-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
```xml
<WorkingPeriodArray>
   <WorkingPeriod>...</WorkingPeriod>
</WorkingPeriodArray>
```

 <span data-ttu-id="d02e6-111">**ArrayOfWorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="d02e6-111">**ArrayOfWorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d02e6-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d02e6-112">Attributes and elements</span></span>

<span data-ttu-id="d02e6-113">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d02e6-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d02e6-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="d02e6-114">Attributes</span></span>

<span data-ttu-id="d02e6-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d02e6-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d02e6-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d02e6-116">Child elements</span></span>

|<span data-ttu-id="d02e6-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d02e6-117">**Element**</span></span>|<span data-ttu-id="d02e6-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="d02e6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d02e6-119">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="d02e6-119">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="d02e6-120">Contient la semaine de travail les jours et les heures de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d02e6-120">Contains the work week days and hours of the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d02e6-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d02e6-121">Parent elements</span></span>

|<span data-ttu-id="d02e6-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d02e6-122">**Element**</span></span>|<span data-ttu-id="d02e6-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="d02e6-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d02e6-124">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="d02e6-124">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d02e6-125">Représente les paramètres de fuseau horaire et les heures de travail pour l’utilisateur de boîte aux lettres demandée.</span><span class="sxs-lookup"><span data-stu-id="d02e6-125">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="d02e6-126">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="d02e6-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d02e6-127">Note</span><span class="sxs-lookup"><span data-stu-id="d02e6-127">Remarks</span></span>

<span data-ttu-id="d02e6-128">Cet élément est obligatoire si l’élément [WorkingHours](workinghours-ex15websvcsotherref.md) est utilisé.</span><span class="sxs-lookup"><span data-stu-id="d02e6-128">This element is required if the [WorkingHours](workinghours-ex15websvcsotherref.md) element is used.</span></span> <span data-ttu-id="d02e6-129">Tous les éléments enfants sont répertoriés dans l’ordre dans lequel elles se produisent.</span><span class="sxs-lookup"><span data-stu-id="d02e6-129">All the child elements are listed in the sequence in which they occur.</span></span> 
  
<span data-ttu-id="d02e6-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d02e6-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d02e6-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d02e6-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d02e6-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d02e6-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d02e6-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d02e6-133">Schema Name</span></span>  <br/> |<span data-ttu-id="d02e6-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d02e6-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d02e6-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d02e6-135">Validation File</span></span>  <br/> |<span data-ttu-id="d02e6-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d02e6-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d02e6-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d02e6-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="d02e6-138">False</span><span class="sxs-lookup"><span data-stu-id="d02e6-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d02e6-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d02e6-139">See also</span></span>



[<span data-ttu-id="d02e6-140">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d02e6-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d02e6-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d02e6-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d02e6-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="d02e6-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

