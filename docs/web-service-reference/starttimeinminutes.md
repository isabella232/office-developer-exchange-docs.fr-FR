---
title: StartTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeInMinutes
api_type:
- schema
ms.assetid: 0fb60a78-6e79-4601-8e2f-5bd245c46d69
description: L’élément StartTimeInMinutes représente le début de la journée de travail pour un utilisateur de boîte aux lettres.
ms.openlocfilehash: f3f1d26731d0406ff8a0fd45fc0243a9feabf886
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829558"
---
# <a name="starttimeinminutes"></a><span data-ttu-id="3d717-103">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="3d717-103">StartTimeInMinutes</span></span>

<span data-ttu-id="3d717-104">L’élément **StartTimeInMinutes** représente le début de la journée de travail pour un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3d717-104">The **StartTimeInMinutes** element represents the start of the working day for a mailbox user.</span></span> 
  
- [<span data-ttu-id="3d717-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3d717-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="3d717-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="3d717-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
- [<span data-ttu-id="3d717-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="3d717-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
- [<span data-ttu-id="3d717-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="3d717-108">FreeBusyView</span></span>](freebusyview.md)
  
- [<span data-ttu-id="3d717-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="3d717-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
- [<span data-ttu-id="3d717-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="3d717-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
- [<span data-ttu-id="3d717-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="3d717-111">WorkingPeriod</span></span>](workingperiod.md)
  
- [<span data-ttu-id="3d717-112">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="3d717-112">StartTimeInMinutes</span></span>](starttimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

<span data-ttu-id="3d717-113">**int**</span><span class="sxs-lookup"><span data-stu-id="3d717-113">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3d717-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3d717-114">Attributes and elements</span></span>

<span data-ttu-id="3d717-115">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3d717-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d717-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="3d717-116">Attributes</span></span>

<span data-ttu-id="3d717-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3d717-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3d717-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3d717-118">Child elements</span></span>

<span data-ttu-id="3d717-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3d717-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3d717-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3d717-120">Parent elements</span></span>

|<span data-ttu-id="3d717-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3d717-121">**Element**</span></span>|<span data-ttu-id="3d717-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="3d717-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d717-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="3d717-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="3d717-124">Contient la semaine de travail les jours et les heures de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3d717-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="3d717-125">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="3d717-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3d717-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3d717-126">Text value</span></span>

<span data-ttu-id="3d717-127">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="3d717-127">A text value is required.</span></span> <span data-ttu-id="3d717-128">La valeur de texte représente le début de la journée de travail par le nombre de minutes se sont écoulées depuis le début de la journée.</span><span class="sxs-lookup"><span data-stu-id="3d717-128">The text value represents the start of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="3d717-129">Par exemple, une heure de début de 8 h 00</span><span class="sxs-lookup"><span data-stu-id="3d717-129">For example, a start time of 8 A.M.</span></span> <span data-ttu-id="3d717-130">est représenté par 480 minutes.</span><span class="sxs-lookup"><span data-stu-id="3d717-130">is represented by 480 minutes.</span></span>
  
<span data-ttu-id="3d717-131">La plage de valeurs possibles pour cet élément est 0 et 1440.</span><span class="sxs-lookup"><span data-stu-id="3d717-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3d717-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="3d717-132">Remarks</span></span>

<span data-ttu-id="3d717-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3d717-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d717-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3d717-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d717-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3d717-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3d717-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3d717-136">Schema Name</span></span>  <br/> |<span data-ttu-id="3d717-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3d717-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="3d717-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3d717-138">Validation File</span></span>  <br/> |<span data-ttu-id="3d717-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3d717-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3d717-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3d717-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="3d717-141">False</span><span class="sxs-lookup"><span data-stu-id="3d717-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3d717-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3d717-142">See also</span></span>

- [<span data-ttu-id="3d717-143">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3d717-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="3d717-144">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3d717-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="3d717-145">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="3d717-145">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

