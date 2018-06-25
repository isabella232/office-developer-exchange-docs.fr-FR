---
title: Durée
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeWindow
api_type:
- schema
ms.assetid: 49c79266-353a-4036-a8e2-8a4660d0d8ea
description: L’élément durée identifie l’intervalle de temps interrogé pour les informations de disponibilité utilisateur.
ms.openlocfilehash: 05858b4d62b72b3ff9904c90652bb1bff78ceb41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838725"
---
# <a name="timewindow"></a><span data-ttu-id="eb2c7-103">Durée</span><span class="sxs-lookup"><span data-stu-id="eb2c7-103">TimeWindow</span></span>

<span data-ttu-id="eb2c7-104">L’élément **durée** identifie l’intervalle de temps interrogé pour les informations de disponibilité utilisateur.</span><span class="sxs-lookup"><span data-stu-id="eb2c7-104">The **TimeWindow** element identifies the time span queried for the user availability information.</span></span> 
  
[<span data-ttu-id="eb2c7-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="eb2c7-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="eb2c7-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="eb2c7-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="eb2c7-107">Durée</span><span class="sxs-lookup"><span data-stu-id="eb2c7-107">TimeWindow</span></span>](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 <span data-ttu-id="eb2c7-108">**Durée**</span><span class="sxs-lookup"><span data-stu-id="eb2c7-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb2c7-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="eb2c7-109">Attributes and elements</span></span>

<span data-ttu-id="eb2c7-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="eb2c7-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb2c7-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="eb2c7-111">Attributes</span></span>

<span data-ttu-id="eb2c7-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="eb2c7-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb2c7-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="eb2c7-113">Child elements</span></span>

|<span data-ttu-id="eb2c7-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eb2c7-114">**Element**</span></span>|<span data-ttu-id="eb2c7-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="eb2c7-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb2c7-116">Heure de début</span><span class="sxs-lookup"><span data-stu-id="eb2c7-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="eb2c7-117">Représente le début d’une période interrogé pour les informations de disponibilité utilisateur.</span><span class="sxs-lookup"><span data-stu-id="eb2c7-117">Represents the start of a time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="eb2c7-118">Heure de fin</span><span class="sxs-lookup"><span data-stu-id="eb2c7-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="eb2c7-119">Représente la fin d’une période interrogée pour les informations de disponibilité utilisateur.</span><span class="sxs-lookup"><span data-stu-id="eb2c7-119">Represents the end of a time span queried for the user availability information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb2c7-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="eb2c7-120">Parent elements</span></span>

|<span data-ttu-id="eb2c7-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eb2c7-121">**Element**</span></span>|<span data-ttu-id="eb2c7-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="eb2c7-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb2c7-123">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="eb2c7-123">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="eb2c7-124">Spécifie le type d’informations disponible/occupé retournés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="eb2c7-124">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="eb2c7-125">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="eb2c7-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eb2c7-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="eb2c7-126">Remarks</span></span>

<span data-ttu-id="eb2c7-127">La valeur maximale pour cette période est de 42 jours.</span><span class="sxs-lookup"><span data-stu-id="eb2c7-127">The maximum value for this time period is 42 days.</span></span> <span data-ttu-id="eb2c7-128">Cette valeur maximale peut être modifiée.</span><span class="sxs-lookup"><span data-stu-id="eb2c7-128">This maximum value can be modified.</span></span> <span data-ttu-id="eb2c7-129">Toutes les demandes des informations de disponibilité utilisateur au-delà de la valeur maximale renverra une erreur.</span><span class="sxs-lookup"><span data-stu-id="eb2c7-129">Any requests for user availability information beyond the maximum value will return an error.</span></span> <span data-ttu-id="eb2c7-130">Si aucun rendez-vous sont partiellement dans la période définie par les éléments [StartTime](starttime.md) et [EndTime](endtime.md) , ce rendez-vous est inclus dans son intégralité.</span><span class="sxs-lookup"><span data-stu-id="eb2c7-130">If any appointments are partially in the time span defined by the [StartTime](starttime.md) and [EndTime](endtime.md) elements, that appointment is included in its entirety.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="eb2c7-131">Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute Microsoft® Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="eb2c7-131">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="eb2c7-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="eb2c7-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb2c7-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="eb2c7-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eb2c7-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="eb2c7-134">Schema Name</span></span>  <br/> |<span data-ttu-id="eb2c7-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="eb2c7-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="eb2c7-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="eb2c7-136">Validation File</span></span>  <br/> |<span data-ttu-id="eb2c7-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eb2c7-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eb2c7-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="eb2c7-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb2c7-139">False</span><span class="sxs-lookup"><span data-stu-id="eb2c7-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb2c7-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="eb2c7-140">See also</span></span>



[<span data-ttu-id="eb2c7-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="eb2c7-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="eb2c7-142">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="eb2c7-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

