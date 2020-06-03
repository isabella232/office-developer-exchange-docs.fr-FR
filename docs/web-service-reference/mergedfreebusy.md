---
title: MergedFreeBusy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: L’élément MergedFreeBusy contient le flux de disponibilité de données fusionné.
ms.openlocfilehash: a1483449534f0d886e3c97a23d28c5d78f865042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468725"
---
# <a name="mergedfreebusy"></a><span data-ttu-id="ace9f-103">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="ace9f-103">MergedFreeBusy</span></span>

<span data-ttu-id="ace9f-104">L’élément **MergedFreeBusy** contient le flux de disponibilité de données fusionné.</span><span class="sxs-lookup"><span data-stu-id="ace9f-104">The **MergedFreeBusy** element contains the merged free/busy stream of data.</span></span> 
  
[<span data-ttu-id="ace9f-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ace9f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="ace9f-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="ace9f-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="ace9f-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="ace9f-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="ace9f-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="ace9f-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="ace9f-109">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="ace9f-109">MergedFreeBusy</span></span>](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 <span data-ttu-id="ace9f-110">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="ace9f-110">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ace9f-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ace9f-111">Attributes and elements</span></span>

<span data-ttu-id="ace9f-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ace9f-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ace9f-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="ace9f-113">Attributes</span></span>

<span data-ttu-id="ace9f-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ace9f-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ace9f-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ace9f-115">Child elements</span></span>

<span data-ttu-id="ace9f-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ace9f-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ace9f-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ace9f-117">Parent elements</span></span>

|<span data-ttu-id="ace9f-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ace9f-118">**Element**</span></span>|<span data-ttu-id="ace9f-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="ace9f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ace9f-120">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="ace9f-120">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="ace9f-121">Contient les informations de disponibilité d’un utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="ace9f-121">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="ace9f-122">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="ace9f-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ace9f-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ace9f-123">Text value</span></span>

<span data-ttu-id="ace9f-124">Une valeur de texte est fournie par le serveur si la valeur de l’élément [FreeBusyViewType](freebusyviewtype.md) est l’une des valeurs suivantes :</span><span class="sxs-lookup"><span data-stu-id="ace9f-124">A text value is provided by the server if the value for the [FreeBusyViewType](freebusyviewtype.md) element is one of the following:</span></span> 
  
- <span data-ttu-id="ace9f-125">DetailedMerged</span><span class="sxs-lookup"><span data-stu-id="ace9f-125">DetailedMerged</span></span>
    
- <span data-ttu-id="ace9f-126">FreeBusyMerged</span><span class="sxs-lookup"><span data-stu-id="ace9f-126">FreeBusyMerged</span></span>
    
- <span data-ttu-id="ace9f-127">MergedOnly</span><span class="sxs-lookup"><span data-stu-id="ace9f-127">MergedOnly</span></span>
    
<span data-ttu-id="ace9f-128">La valeur de texte est un flux d’informations de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="ace9f-128">The text value is a stream of free/busy information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ace9f-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="ace9f-129">Remarks</span></span>

<span data-ttu-id="ace9f-130">Le flux de données fourni par cet élément est défini par les éléments [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) et [TimeWindow](timewindow.md) .</span><span class="sxs-lookup"><span data-stu-id="ace9f-130">The stream of data provided by this element is defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) and [TimeWindow](timewindow.md) elements.</span></span> <span data-ttu-id="ace9f-131">L’élément [TimeWindow](timewindow.md) définit la période interrogée pour la disponibilité.</span><span class="sxs-lookup"><span data-stu-id="ace9f-131">The [TimeWindow](timewindow.md) element defines the time span queried for availability.</span></span> <span data-ttu-id="ace9f-132">L’élément [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) définit la manière dont l’heure de l’élément [TimeWindow](timewindow.md) est divisée en intervalles renvoyés dans l’élément **MergedFreeBusy** .</span><span class="sxs-lookup"><span data-stu-id="ace9f-132">The [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element defines how the time from the [TimeWindow](timewindow.md) element is broken into intervals returned in the **MergedFreeBusy** element.</span></span> <span data-ttu-id="ace9f-133">Chaque nombre dans le flux **MergedFreeBusy** représente un intervalle unique défini par l’élément [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) .</span><span class="sxs-lookup"><span data-stu-id="ace9f-133">Each number in the **MergedFreeBusy** stream represents a single interval defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element.</span></span> <span data-ttu-id="ace9f-134">Le tableau suivant répertorie les valeurs possibles pour un intervalle individuel.</span><span class="sxs-lookup"><span data-stu-id="ace9f-134">The following table lists the possible values for an individual interval.</span></span> 
  
|<span data-ttu-id="ace9f-135">**Numérique**</span><span class="sxs-lookup"><span data-stu-id="ace9f-135">**Digit**</span></span>|<span data-ttu-id="ace9f-136">**Disponibilité**</span><span class="sxs-lookup"><span data-stu-id="ace9f-136">**Availability**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ace9f-137">0</span><span class="sxs-lookup"><span data-stu-id="ace9f-137">0</span></span>  <br/> |<span data-ttu-id="ace9f-138">Gratuit</span><span class="sxs-lookup"><span data-stu-id="ace9f-138">Free</span></span>  <br/> |
|<span data-ttu-id="ace9f-139">1 </span><span class="sxs-lookup"><span data-stu-id="ace9f-139">1</span></span>  <br/> |<span data-ttu-id="ace9f-140">Provisoire</span><span class="sxs-lookup"><span data-stu-id="ace9f-140">Tentative</span></span>  <br/> |
|<span data-ttu-id="ace9f-141">n°2</span><span class="sxs-lookup"><span data-stu-id="ace9f-141">2</span></span>  <br/> |<span data-ttu-id="ace9f-142">Occupé(e)</span><span class="sxs-lookup"><span data-stu-id="ace9f-142">Busy</span></span>  <br/> |
|<span data-ttu-id="ace9f-143">3</span><span class="sxs-lookup"><span data-stu-id="ace9f-143">3</span></span>  <br/> |<span data-ttu-id="ace9f-144">Absent(e) du bureau</span><span class="sxs-lookup"><span data-stu-id="ace9f-144">Out of Office (OOF)</span></span>  <br/> |
|<span data-ttu-id="ace9f-145">4 </span><span class="sxs-lookup"><span data-stu-id="ace9f-145">4</span></span>  <br/> |<span data-ttu-id="ace9f-146">Aucune donnée</span><span class="sxs-lookup"><span data-stu-id="ace9f-146">No data</span></span>  <br/> |
   
<span data-ttu-id="ace9f-147">Par exemple, une demande de données de disponibilité inclut un élément [TimeWindow](timewindow.md) qui représente quatre heures et un élément [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) qui représente 60 minutes.</span><span class="sxs-lookup"><span data-stu-id="ace9f-147">For example, a request for free/busy data includes a [TimeWindow](timewindow.md) element that represents four hours and a [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element that represents 60 minutes.</span></span> <span data-ttu-id="ace9f-148">Si le calendrier de l’utilisateur demandé est absent du Bureau pour les 60 premières minutes, occupé pour les 90 minutes suivantes et non planifié pendant les 90 minutes finales dans la fenêtre de temps, le flux **MergedFreeBusy** sera 3220.</span><span class="sxs-lookup"><span data-stu-id="ace9f-148">If the requested user's calendar is OOF for the first 60 minutes, busy for the following 90 minutes, and unscheduled for the final 90 minutes in the time window, the **MergedFreeBusy** stream will be 3220.</span></span> <span data-ttu-id="ace9f-149">Si un intervalle contient plus d’une classification de disponibilité, le nombre le plus élevé est utilisé pour classer cet intervalle.</span><span class="sxs-lookup"><span data-stu-id="ace9f-149">If an interval contains more than one availability classification, the highest number is used to classify that interval.</span></span> 
  
<span data-ttu-id="ace9f-150">Le niveau de détail fourni par cet élément dépend des autorisations accordées au demandeur.</span><span class="sxs-lookup"><span data-stu-id="ace9f-150">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="ace9f-151">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ace9f-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ace9f-152">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ace9f-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ace9f-153">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ace9f-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ace9f-154">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ace9f-154">Schema Name</span></span>  <br/> |<span data-ttu-id="ace9f-155">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ace9f-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="ace9f-156">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ace9f-156">Validation File</span></span>  <br/> |<span data-ttu-id="ace9f-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ace9f-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ace9f-158">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ace9f-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="ace9f-159">False</span><span class="sxs-lookup"><span data-stu-id="ace9f-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ace9f-160">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ace9f-160">See also</span></span>



[<span data-ttu-id="ace9f-161">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ace9f-161">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="ace9f-162">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ace9f-162">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="ace9f-163">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="ace9f-163">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

