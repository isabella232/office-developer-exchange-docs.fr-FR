---
title: Heure de début
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: L’élément StartTime représente le début d’un intervalle de temps.
ms.openlocfilehash: 4346797d755bb6e577e1cacb8bec656a7562bf1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829560"
---
# <a name="starttime"></a><span data-ttu-id="d5223-103">Heure de début</span><span class="sxs-lookup"><span data-stu-id="d5223-103">StartTime</span></span>

<span data-ttu-id="d5223-104">L’élément **StartTime** représente le début d’un intervalle de temps.</span><span class="sxs-lookup"><span data-stu-id="d5223-104">The **StartTime** element represents the start of a time span.</span></span> 
  
```xml
<StartTime/
```

<span data-ttu-id="d5223-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="d5223-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d5223-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d5223-106">Attributes and elements</span></span>

<span data-ttu-id="d5223-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d5223-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5223-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d5223-108">Attributes</span></span>

<span data-ttu-id="d5223-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d5223-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5223-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d5223-110">Child elements</span></span>

<span data-ttu-id="d5223-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d5223-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d5223-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d5223-112">Parent elements</span></span>

|<span data-ttu-id="d5223-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d5223-113">**Element**</span></span>|<span data-ttu-id="d5223-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d5223-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5223-115">Durée</span><span class="sxs-lookup"><span data-stu-id="d5223-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="d5223-116">Identifie l’intervalle de temps interrogé pour les informations de disponibilité utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d5223-116">Identifies the time span queried for the user availability information.</span></span>  <br/><br/> <span data-ttu-id="d5223-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="d5223-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="d5223-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="d5223-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="d5223-119">Identifie l’intervalle de temps qui est interrogé pour des informations détaillées sur les heures de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="d5223-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/><br/> <span data-ttu-id="d5223-120">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="d5223-120">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[<span data-ttu-id="d5223-121">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="d5223-121">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="d5223-122">Spécifie la durée pour laquelle le statut d’absence du bureau (OOF) est activé si l’élément [OofState](oofstate.md) est défini sur **planifiée**.</span><span class="sxs-lookup"><span data-stu-id="d5223-122">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="d5223-123">Les expressions XPath possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="d5223-123">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="d5223-124">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="d5223-124">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="d5223-125">Représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="d5223-125">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="d5223-126">Il est utilisé pour les recherches de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="d5223-126">This is used for Availability inquiries.</span></span> <span data-ttu-id="d5223-127">L’élément **StartTime** est requis dans l’élément **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="d5223-127">The **StartTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="d5223-128">L’élément **StartTime** dans l’élément **CalendarEvent** est unique pour le type **CalendarEvent** bien qu’il contient les mêmes valeurs de facettes qui contiennent les éléments de **l’heure de début** dans le type de **durée** .</span><span class="sxs-lookup"><span data-stu-id="d5223-128">The **StartTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type although it contains the same facet values that the **StartTime** elements in the **Duration** type contain.</span></span>  <br/><br/> <span data-ttu-id="d5223-129">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="d5223-129">The following is the XPath expression to this element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d5223-130">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d5223-130">Text value</span></span>

<span data-ttu-id="d5223-131">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="d5223-131">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d5223-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="d5223-132">Remarks</span></span>

<span data-ttu-id="d5223-133">L’élément [EndTime](endtime.md) représente la fin de l’intervalle de temps.</span><span class="sxs-lookup"><span data-stu-id="d5223-133">The [EndTime](endtime.md) element represents the end of the time span.</span></span> 
  
<span data-ttu-id="d5223-134">Le schéma inclut de nombreux éléments de [l’heure de début](starttime.md) .</span><span class="sxs-lookup"><span data-stu-id="d5223-134">The schema includes many [StartTime](starttime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d5223-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d5223-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d5223-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d5223-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5223-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d5223-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d5223-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d5223-138">Schema Name</span></span>  <br/> |<span data-ttu-id="d5223-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d5223-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="d5223-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d5223-140">Validation File</span></span>  <br/> |<span data-ttu-id="d5223-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d5223-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d5223-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d5223-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5223-143">False</span><span class="sxs-lookup"><span data-stu-id="d5223-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5223-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d5223-144">See also</span></span>

- [<span data-ttu-id="d5223-145">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d5223-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="d5223-146">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="d5223-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

