---
title: FreeBusyView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: L’élément FreeBusyView contient les informations de disponibilité d’un utilisateur spécifique.
ms.openlocfilehash: e5cc3bea6b57d5c400dd9be44bf9f9aaf9e43eb9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456100"
---
# <a name="freebusyview"></a><span data-ttu-id="eab96-103">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="eab96-103">FreeBusyView</span></span>

<span data-ttu-id="eab96-104">L’élément **FreeBusyView** contient les informations de disponibilité d’un utilisateur spécifique.</span><span class="sxs-lookup"><span data-stu-id="eab96-104">The **FreeBusyView** element contains availability information for a specific user.</span></span> 
  
[<span data-ttu-id="eab96-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="eab96-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="eab96-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="eab96-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="eab96-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="eab96-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="eab96-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="eab96-108">FreeBusyView</span></span>](freebusyview.md)
  
```xml
<FreeBusyView>
   <FreeBusyViewType>...</FreeBusyViewType>
   <MergedFreeBusy>...</MergedFreeBusy>
   <CalendarEventArray>...</CalendarEventArray>
   <WorkingHours>...</WorkingHours>
</FreeBusyView>
```

 <span data-ttu-id="eab96-109">**FreeBusyView**</span><span class="sxs-lookup"><span data-stu-id="eab96-109">**FreeBusyView**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eab96-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="eab96-110">Attributes and elements</span></span>

<span data-ttu-id="eab96-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="eab96-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eab96-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="eab96-112">Attributes</span></span>

<span data-ttu-id="eab96-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="eab96-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eab96-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="eab96-114">Child elements</span></span>

|<span data-ttu-id="eab96-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eab96-115">**Element**</span></span>|<span data-ttu-id="eab96-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="eab96-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eab96-117">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="eab96-117">FreeBusyViewType</span></span>](freebusyviewtype.md) <br/> |<span data-ttu-id="eab96-118">Représente le type des informations de disponibilité demandées renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="eab96-118">Represents the type of requested free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="eab96-119">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="eab96-119">MergedFreeBusy</span></span>](mergedfreebusy.md) <br/> |<span data-ttu-id="eab96-120">Contient le flux de données de disponibilité fusionné.</span><span class="sxs-lookup"><span data-stu-id="eab96-120">Contains the merged free/busy stream of data.</span></span>  <br/> |
|[<span data-ttu-id="eab96-121">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="eab96-121">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="eab96-122">Contient un ensemble d’occurrences d’éléments de calendrier uniques qui représentent la disponibilité de l’utilisateur demandé.</span><span class="sxs-lookup"><span data-stu-id="eab96-122">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> |
|[<span data-ttu-id="eab96-123">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="eab96-123">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="eab96-124">Représente les paramètres de fuseau horaire et les heures de travail de l’utilisateur de boîte aux lettres demandé.</span><span class="sxs-lookup"><span data-stu-id="eab96-124">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eab96-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="eab96-125">Parent elements</span></span>

|<span data-ttu-id="eab96-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eab96-126">**Element**</span></span>|<span data-ttu-id="eab96-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="eab96-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eab96-128">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="eab96-128">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="eab96-129">Contient les informations de disponibilité pour un utilisateur de boîte aux lettres unique.</span><span class="sxs-lookup"><span data-stu-id="eab96-129">Contains the free/busy information for a single mailbox user.</span></span>  <br/> <span data-ttu-id="eab96-130">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="eab96-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eab96-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="eab96-131">Remarks</span></span>

<span data-ttu-id="eab96-132">Tous les éléments enfants sont répertoriés dans l’ordre dans lequel ils se produisent.</span><span class="sxs-lookup"><span data-stu-id="eab96-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="eab96-133">Le niveau de détail fourni par cet élément dépend des autorisations accordées au demandeur.</span><span class="sxs-lookup"><span data-stu-id="eab96-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="eab96-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="eab96-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eab96-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="eab96-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eab96-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="eab96-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eab96-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="eab96-137">Schema Name</span></span>  <br/> |<span data-ttu-id="eab96-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="eab96-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="eab96-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="eab96-139">Validation File</span></span>  <br/> |<span data-ttu-id="eab96-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eab96-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eab96-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="eab96-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="eab96-142">False</span><span class="sxs-lookup"><span data-stu-id="eab96-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eab96-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="eab96-143">See also</span></span>



[<span data-ttu-id="eab96-144">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="eab96-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="eab96-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="eab96-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="eab96-146">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="eab96-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

