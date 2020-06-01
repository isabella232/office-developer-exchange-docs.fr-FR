---
title: TimeWindow
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
description: L’élément TimeWindow identifie la période interrogée pour les informations de disponibilité de l’utilisateur.
ms.openlocfilehash: 5c66614520f9d616687d67ad609b3d55d9cf6571
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458928"
---
# <a name="timewindow"></a><span data-ttu-id="0b465-103">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="0b465-103">TimeWindow</span></span>

<span data-ttu-id="0b465-104">L’élément **TimeWindow** identifie la période interrogée pour les informations de disponibilité de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="0b465-104">The **TimeWindow** element identifies the time span queried for the user availability information.</span></span> 
  
[<span data-ttu-id="0b465-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="0b465-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="0b465-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="0b465-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="0b465-107">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="0b465-107">TimeWindow</span></span>](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 <span data-ttu-id="0b465-108">**Duration**</span><span class="sxs-lookup"><span data-stu-id="0b465-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b465-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0b465-109">Attributes and elements</span></span>

<span data-ttu-id="0b465-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0b465-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b465-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="0b465-111">Attributes</span></span>

<span data-ttu-id="0b465-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0b465-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b465-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0b465-113">Child elements</span></span>

|<span data-ttu-id="0b465-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0b465-114">**Element**</span></span>|<span data-ttu-id="0b465-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="0b465-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b465-116">StartTime</span><span class="sxs-lookup"><span data-stu-id="0b465-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="0b465-117">Représente le début d’une période de temps interrogée pour les informations de disponibilité de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="0b465-117">Represents the start of a time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="0b465-118">EndTime</span><span class="sxs-lookup"><span data-stu-id="0b465-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="0b465-119">Représente la fin d’un intervalle de temps interrogé pour les informations de disponibilité de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="0b465-119">Represents the end of a time span queried for the user availability information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b465-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0b465-120">Parent elements</span></span>

|<span data-ttu-id="0b465-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0b465-121">**Element**</span></span>|<span data-ttu-id="0b465-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="0b465-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b465-123">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="0b465-123">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="0b465-124">Spécifie le type d’informations de disponibilité renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="0b465-124">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="0b465-125">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="0b465-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0b465-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="0b465-126">Remarks</span></span>

<span data-ttu-id="0b465-127">La valeur maximale pour cette période de temps est de 42 jours.</span><span class="sxs-lookup"><span data-stu-id="0b465-127">The maximum value for this time period is 42 days.</span></span> <span data-ttu-id="0b465-128">Cette valeur maximale peut être modifiée.</span><span class="sxs-lookup"><span data-stu-id="0b465-128">This maximum value can be modified.</span></span> <span data-ttu-id="0b465-129">Toute demande d’informations de disponibilité de l’utilisateur au-delà de la valeur maximale renverra une erreur.</span><span class="sxs-lookup"><span data-stu-id="0b465-129">Any requests for user availability information beyond the maximum value will return an error.</span></span> <span data-ttu-id="0b465-130">Si des rendez-vous sont partiellement dans l’intervalle de temps défini par les éléments [StartTime](starttime.md) et [EndTime](endtime.md) , ce rendez-vous est inclus dans son intégralité.</span><span class="sxs-lookup"><span data-stu-id="0b465-130">If any appointments are partially in the time span defined by the [StartTime](starttime.md) and [EndTime](endtime.md) elements, that appointment is included in its entirety.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0b465-131">Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur exécutant Microsoft® Exchange Server 2007 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0b465-131">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="0b465-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0b465-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b465-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0b465-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b465-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0b465-134">Schema Name</span></span>  <br/> |<span data-ttu-id="0b465-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0b465-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b465-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0b465-136">Validation File</span></span>  <br/> |<span data-ttu-id="0b465-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0b465-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b465-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0b465-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b465-139">False</span><span class="sxs-lookup"><span data-stu-id="0b465-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b465-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0b465-140">See also</span></span>



[<span data-ttu-id="0b465-141">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0b465-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="0b465-142">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="0b465-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

