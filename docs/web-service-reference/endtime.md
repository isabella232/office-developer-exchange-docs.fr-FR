---
title: Heure de fin
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTime
api_type:
- schema
ms.assetid: 82e4ef4f-a557-4044-b9b7-d91622f4ac55
description: L’élément EndTime représente la fin d’un intervalle de temps.
ms.openlocfilehash: 7d3d186618a7bcc05ad82532e13e03d2e67a0e40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756196"
---
# <a name="endtime"></a><span data-ttu-id="b33fd-103">Heure de fin</span><span class="sxs-lookup"><span data-stu-id="b33fd-103">EndTime</span></span>

<span data-ttu-id="b33fd-104">L’élément **EndTime** représente la fin d’un intervalle de temps.</span><span class="sxs-lookup"><span data-stu-id="b33fd-104">The **EndTime** element represents the end of a time span.</span></span> 
  
```xml
<EndTime>dateTime</EndTime>
```

 <span data-ttu-id="b33fd-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="b33fd-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b33fd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b33fd-106">Attributes and elements</span></span>

<span data-ttu-id="b33fd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b33fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b33fd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b33fd-108">Attributes</span></span>

<span data-ttu-id="b33fd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b33fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b33fd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b33fd-110">Child elements</span></span>

<span data-ttu-id="b33fd-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b33fd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b33fd-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b33fd-112">Parent elements</span></span>

|<span data-ttu-id="b33fd-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b33fd-113">**Element**</span></span>|<span data-ttu-id="b33fd-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b33fd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b33fd-115">Durée</span><span class="sxs-lookup"><span data-stu-id="b33fd-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="b33fd-116">Identifie l’intervalle de temps interrogé pour les informations de disponibilité utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b33fd-116">Identifies the time span queried for the user availability information.</span></span><br/><br/> <span data-ttu-id="b33fd-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="b33fd-117">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="b33fd-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="b33fd-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="b33fd-119">Identifie l’intervalle de temps qui est interrogé pour des informations détaillées sur les heures de réunion suggérée.</span><span class="sxs-lookup"><span data-stu-id="b33fd-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span><br/><br/> <span data-ttu-id="b33fd-120">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="b33fd-120">The following is the XPath expression to this element:</span></span><br/><br/>  <span data-ttu-id="b33fd-121">`/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.</span><span class="sxs-lookup"><span data-stu-id="b33fd-121"></span></span>  <br/> |
|[<span data-ttu-id="b33fd-122">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="b33fd-122">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="b33fd-123">Spécifie la durée pour laquelle le statut d’absence du bureau (OOF) est activé si l’élément [OofState](oofstate.md) est défini sur **planifiée**.</span><span class="sxs-lookup"><span data-stu-id="b33fd-123">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="b33fd-124">Les expressions XPath possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="b33fd-124">The following are the possible XPath expressions to this element:</span></span><br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="b33fd-125">Occurrence</span><span class="sxs-lookup"><span data-stu-id="b33fd-125">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="b33fd-126">Représente une seule occurrence de modification d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="b33fd-126">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b33fd-127">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="b33fd-127">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="b33fd-128">Représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="b33fd-128">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="b33fd-129">Il est utilisé pour les recherches de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="b33fd-129">This is used for Availability inquiries.</span></span> <span data-ttu-id="b33fd-130">L’élément **EndTime** est requis dans l’élément **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="b33fd-130">The **EndTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="b33fd-131">L’élément de **l’heure de fin** dans l’élément **CalendarEvent** est unique pour le type **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="b33fd-131">The **EndTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type.</span></span><br/><br/> <span data-ttu-id="b33fd-132">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="b33fd-132">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b33fd-133">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b33fd-133">Text value</span></span>

<span data-ttu-id="b33fd-134">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="b33fd-134">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b33fd-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="b33fd-135">Remarks</span></span>

<span data-ttu-id="b33fd-136">L’élément [StartTime](starttime.md) représente le début d’un intervalle de temps.</span><span class="sxs-lookup"><span data-stu-id="b33fd-136">The [StartTime](starttime.md) element represents the beginning of a time span.</span></span> 
  
<span data-ttu-id="b33fd-137">L’heure de fin représente la durée du client.</span><span class="sxs-lookup"><span data-stu-id="b33fd-137">The end time represents the client's time.</span></span>
  
<span data-ttu-id="b33fd-138">Le schéma inclut de nombreux éléments de [l’heure de fin](endtime.md) .</span><span class="sxs-lookup"><span data-stu-id="b33fd-138">The schema includes many [EndTime](endtime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b33fd-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b33fd-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b33fd-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b33fd-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b33fd-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b33fd-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b33fd-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b33fd-142">Schema Name</span></span>  <br/> |<span data-ttu-id="b33fd-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b33fd-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="b33fd-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b33fd-144">Validation File</span></span>  <br/> |<span data-ttu-id="b33fd-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b33fd-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b33fd-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b33fd-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="b33fd-147">False</span><span class="sxs-lookup"><span data-stu-id="b33fd-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b33fd-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b33fd-148">See also</span></span>

- [<span data-ttu-id="b33fd-149">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b33fd-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="b33fd-150">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="b33fd-150">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

