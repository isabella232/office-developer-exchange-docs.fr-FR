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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829560"
---
# <a name="starttime"></a><span data-ttu-id="cf71f-103">Heure de début</span><span class="sxs-lookup"><span data-stu-id="cf71f-103">StartTime</span></span>

<span data-ttu-id="cf71f-104">L’élément **StartTime** représente le début d’un intervalle de temps.</span><span class="sxs-lookup"><span data-stu-id="cf71f-104">The **StartTime** element represents the start of a time span.</span></span> 
  
```xml
<StartTime/
```

<span data-ttu-id="cf71f-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="cf71f-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cf71f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cf71f-106">Attributes and elements</span></span>

<span data-ttu-id="cf71f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cf71f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf71f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cf71f-108">Attributes</span></span>

<span data-ttu-id="cf71f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cf71f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf71f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cf71f-110">Child elements</span></span>

<span data-ttu-id="cf71f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cf71f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf71f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cf71f-112">Parent elements</span></span>

|<span data-ttu-id="cf71f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cf71f-113">**Element**</span></span>|<span data-ttu-id="cf71f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="cf71f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf71f-115">Durée</span><span class="sxs-lookup"><span data-stu-id="cf71f-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="cf71f-116">Identifie l’intervalle de temps interrogé pour les informations de disponibilité utilisateur.</span><span class="sxs-lookup"><span data-stu-id="cf71f-116">Identifies the time span queried for the user availability information.</span></span>  <br/><br/> <span data-ttu-id="cf71f-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="cf71f-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="cf71f-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="cf71f-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="cf71f-119">Identifie l’intervalle de temps qui est interrogé pour des informations détaillées sur les heures de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="cf71f-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/><br/> <span data-ttu-id="cf71f-120">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="cf71f-120">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[<span data-ttu-id="cf71f-121">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="cf71f-121">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="cf71f-122">Spécifie la durée pour laquelle le statut d’absence du bureau (OOF) est activé si l’élément [OofState](oofstate.md) est défini sur **planifiée**.</span><span class="sxs-lookup"><span data-stu-id="cf71f-122">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="cf71f-123">Les expressions XPath possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="cf71f-123">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="cf71f-124">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="cf71f-124">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="cf71f-125">Représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="cf71f-125">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="cf71f-126">Il est utilisé pour les recherches de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="cf71f-126">This is used for Availability inquiries.</span></span> <span data-ttu-id="cf71f-127">L’élément **StartTime** est requis dans l’élément **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="cf71f-127">The **StartTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="cf71f-128">L’élément **StartTime** dans l’élément **CalendarEvent** est unique pour le type **CalendarEvent** bien qu’il contient les mêmes valeurs de facettes qui contiennent les éléments de **l’heure de début** dans le type de **durée** .</span><span class="sxs-lookup"><span data-stu-id="cf71f-128">The **StartTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type although it contains the same facet values that the **StartTime** elements in the **Duration** type contain.</span></span>  <br/><br/> <span data-ttu-id="cf71f-129">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="cf71f-129">The following is the XPath expression to this element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf71f-130">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="cf71f-130">Text value</span></span>

<span data-ttu-id="cf71f-131">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="cf71f-131">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cf71f-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="cf71f-132">Remarks</span></span>

<span data-ttu-id="cf71f-133">L’élément [EndTime](endtime.md) représente la fin de l’intervalle de temps.</span><span class="sxs-lookup"><span data-stu-id="cf71f-133">The [EndTime](endtime.md) element represents the end of the time span.</span></span> 
  
<span data-ttu-id="cf71f-134">Le schéma inclut de nombreux éléments de [l’heure de début](starttime.md) .</span><span class="sxs-lookup"><span data-stu-id="cf71f-134">The schema includes many [StartTime](starttime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="cf71f-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="cf71f-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="cf71f-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cf71f-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf71f-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cf71f-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf71f-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cf71f-138">Schema Name</span></span>  <br/> |<span data-ttu-id="cf71f-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cf71f-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf71f-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cf71f-140">Validation File</span></span>  <br/> |<span data-ttu-id="cf71f-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cf71f-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf71f-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cf71f-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf71f-143">False</span><span class="sxs-lookup"><span data-stu-id="cf71f-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf71f-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cf71f-144">See also</span></span>

- [<span data-ttu-id="cf71f-145">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="cf71f-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="cf71f-146">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="cf71f-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

