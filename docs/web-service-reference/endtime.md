---
title: EndTime
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
description: L’élément EndTime représente la fin d’une plage de temps.
ms.openlocfilehash: 5a30b32ecfeafe582cd07dd662aacb0a960257c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462991"
---
# <a name="endtime"></a><span data-ttu-id="b4fee-103">EndTime</span><span class="sxs-lookup"><span data-stu-id="b4fee-103">EndTime</span></span>

<span data-ttu-id="b4fee-104">L’élément **EndTime** représente la fin d’une plage de temps.</span><span class="sxs-lookup"><span data-stu-id="b4fee-104">The **EndTime** element represents the end of a time span.</span></span> 
  
```xml
<EndTime>dateTime</EndTime>
```

 <span data-ttu-id="b4fee-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="b4fee-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b4fee-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b4fee-106">Attributes and elements</span></span>

<span data-ttu-id="b4fee-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b4fee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4fee-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b4fee-108">Attributes</span></span>

<span data-ttu-id="b4fee-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b4fee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4fee-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b4fee-110">Child elements</span></span>

<span data-ttu-id="b4fee-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b4fee-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b4fee-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b4fee-112">Parent elements</span></span>

|<span data-ttu-id="b4fee-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b4fee-113">**Element**</span></span>|<span data-ttu-id="b4fee-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b4fee-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4fee-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="b4fee-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="b4fee-116">Identifie la période interrogée pour les informations de disponibilité de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="b4fee-116">Identifies the time span queried for the user availability information.</span></span><br/><br/> <span data-ttu-id="b4fee-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="b4fee-117">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="b4fee-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="b4fee-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="b4fee-119">Identifie l’intervalle de temps interrogé pour obtenir des informations détaillées sur les heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="b4fee-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span><br/><br/> <span data-ttu-id="b4fee-120">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="b4fee-120">The following is the XPath expression to this element:</span></span><br/><br/>  <span data-ttu-id="b4fee-121">`/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.</span><span class="sxs-lookup"><span data-stu-id="b4fee-121">`/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.</span></span>  <br/> |
|[<span data-ttu-id="b4fee-122">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="b4fee-122">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="b4fee-123">Spécifie la durée pendant laquelle l’État absent (absent du bureau) est activé si l’élément [OofState](oofstate.md) est défini sur **Planifié**.</span><span class="sxs-lookup"><span data-stu-id="b4fee-123">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="b4fee-124">Voici les expressions XPath possibles pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="b4fee-124">The following are the possible XPath expressions to this element:</span></span><br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="b4fee-125">Réunions</span><span class="sxs-lookup"><span data-stu-id="b4fee-125">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="b4fee-126">Représente une occurrence modifiée unique d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="b4fee-126">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="b4fee-127">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="b4fee-127">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="b4fee-128">Représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="b4fee-128">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="b4fee-129">Cette information est utilisée pour les demandes de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="b4fee-129">This is used for Availability inquiries.</span></span> <span data-ttu-id="b4fee-130">L’élément **EndTime** est requis dans l’élément **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="b4fee-130">The **EndTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="b4fee-131">L’élément **EndTime** de l’élément **CalendarEvent** est propre au type **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="b4fee-131">The **EndTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type.</span></span><br/><br/> <span data-ttu-id="b4fee-132">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="b4fee-132">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b4fee-133">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="b4fee-133">Text value</span></span>

<span data-ttu-id="b4fee-134">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="b4fee-134">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b4fee-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="b4fee-135">Remarks</span></span>

<span data-ttu-id="b4fee-136">L’élément [StartTime](starttime.md) représente le début d’une période.</span><span class="sxs-lookup"><span data-stu-id="b4fee-136">The [StartTime](starttime.md) element represents the beginning of a time span.</span></span> 
  
<span data-ttu-id="b4fee-137">L’heure de fin représente l’heure du client.</span><span class="sxs-lookup"><span data-stu-id="b4fee-137">The end time represents the client's time.</span></span>
  
<span data-ttu-id="b4fee-138">Le schéma comprend de nombreux éléments [EndTime](endtime.md) .</span><span class="sxs-lookup"><span data-stu-id="b4fee-138">The schema includes many [EndTime](endtime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b4fee-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b4fee-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b4fee-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b4fee-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4fee-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b4fee-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b4fee-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b4fee-142">Schema Name</span></span>  <br/> |<span data-ttu-id="b4fee-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b4fee-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="b4fee-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b4fee-144">Validation File</span></span>  <br/> |<span data-ttu-id="b4fee-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b4fee-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b4fee-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b4fee-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="b4fee-147">False</span><span class="sxs-lookup"><span data-stu-id="b4fee-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b4fee-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b4fee-148">See also</span></span>

- [<span data-ttu-id="b4fee-149">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b4fee-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="b4fee-150">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="b4fee-150">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

