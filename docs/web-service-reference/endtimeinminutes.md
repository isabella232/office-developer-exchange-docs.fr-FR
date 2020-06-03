---
title: EndTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTimeInMinutes
api_type:
- schema
ms.assetid: ef05bdda-7a66-44db-bb73-a2ce8316c257
description: L’élément EndTimeInMinutes représente la fin de la journée de travail pour un utilisateur de boîte aux lettres.
ms.openlocfilehash: cb564f9de944848734749a30c813a94d6b5c4187
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459650"
---
# <a name="endtimeinminutes"></a><span data-ttu-id="cd7bb-103">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="cd7bb-103">EndTimeInMinutes</span></span>

<span data-ttu-id="cd7bb-104">L’élément **EndTimeInMinutes** représente la fin de la journée de travail pour un utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cd7bb-104">The **EndTimeInMinutes** element represents the end of the working day for a mailbox user.</span></span> 
  
[<span data-ttu-id="cd7bb-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cd7bb-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="cd7bb-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="cd7bb-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="cd7bb-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="cd7bb-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="cd7bb-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="cd7bb-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="cd7bb-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="cd7bb-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="cd7bb-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="cd7bb-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="cd7bb-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="cd7bb-111">WorkingPeriod</span></span>](workingperiod.md)
  
[<span data-ttu-id="cd7bb-112">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="cd7bb-112">EndTimeInMinutes</span></span>](endtimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

 <span data-ttu-id="cd7bb-113">**int**</span><span class="sxs-lookup"><span data-stu-id="cd7bb-113">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd7bb-114">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cd7bb-114">Attributes and elements</span></span>

<span data-ttu-id="cd7bb-115">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cd7bb-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd7bb-116">Attributs</span><span class="sxs-lookup"><span data-stu-id="cd7bb-116">Attributes</span></span>

<span data-ttu-id="cd7bb-117">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cd7bb-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd7bb-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cd7bb-118">Child elements</span></span>

<span data-ttu-id="cd7bb-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cd7bb-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd7bb-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cd7bb-120">Parent elements</span></span>

|<span data-ttu-id="cd7bb-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cd7bb-121">**Element**</span></span>|<span data-ttu-id="cd7bb-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="cd7bb-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd7bb-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="cd7bb-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="cd7bb-124">Contient les jours et les heures de travail de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cd7bb-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="cd7bb-125">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="cd7bb-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cd7bb-126">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="cd7bb-126">Text value</span></span>

<span data-ttu-id="cd7bb-127">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="cd7bb-127">A text value is required.</span></span> <span data-ttu-id="cd7bb-128">La valeur de texte représente la fin du jour ouvré en nombre de minutes écoulées depuis le début du jour.</span><span class="sxs-lookup"><span data-stu-id="cd7bb-128">The text value represents the end of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="cd7bb-129">Par exemple, une heure de fin de 18 heures.</span><span class="sxs-lookup"><span data-stu-id="cd7bb-129">For example, an end time of 6 P.M.</span></span> <span data-ttu-id="cd7bb-130">est représenté par 1080 minutes.</span><span class="sxs-lookup"><span data-stu-id="cd7bb-130">is represented by 1080 minutes.</span></span>
  
<span data-ttu-id="cd7bb-131">La plage de valeurs possibles pour cet élément est comprise entre 0 et 1440.</span><span class="sxs-lookup"><span data-stu-id="cd7bb-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cd7bb-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="cd7bb-132">Remarks</span></span>

<span data-ttu-id="cd7bb-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="cd7bb-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd7bb-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cd7bb-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd7bb-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cd7bb-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd7bb-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cd7bb-136">Schema Name</span></span>  <br/> |<span data-ttu-id="cd7bb-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cd7bb-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="cd7bb-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cd7bb-138">Validation File</span></span>  <br/> |<span data-ttu-id="cd7bb-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cd7bb-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd7bb-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cd7bb-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="cd7bb-141">False</span><span class="sxs-lookup"><span data-stu-id="cd7bb-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd7bb-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cd7bb-142">See also</span></span>



[<span data-ttu-id="cd7bb-143">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="cd7bb-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="cd7bb-144">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cd7bb-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="cd7bb-145">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="cd7bb-145">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

