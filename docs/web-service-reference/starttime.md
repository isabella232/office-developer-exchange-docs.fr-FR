---
title: StartTime
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
description: L’élément StartTime représente le début d’une période.
ms.openlocfilehash: 16bee698b65dc512a709e2af9ddfe8629347fee3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458564"
---
# <a name="starttime"></a><span data-ttu-id="bf819-103">StartTime</span><span class="sxs-lookup"><span data-stu-id="bf819-103">StartTime</span></span>

<span data-ttu-id="bf819-104">L’élément **StartTime** représente le début d’une période.</span><span class="sxs-lookup"><span data-stu-id="bf819-104">The **StartTime** element represents the start of a time span.</span></span> 
  
```xml
<StartTime/
```

<span data-ttu-id="bf819-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="bf819-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bf819-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bf819-106">Attributes and elements</span></span>

<span data-ttu-id="bf819-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bf819-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf819-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bf819-108">Attributes</span></span>

<span data-ttu-id="bf819-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bf819-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf819-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bf819-110">Child elements</span></span>

<span data-ttu-id="bf819-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bf819-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bf819-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bf819-112">Parent elements</span></span>

|<span data-ttu-id="bf819-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bf819-113">**Element**</span></span>|<span data-ttu-id="bf819-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="bf819-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf819-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="bf819-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="bf819-116">Identifie la période interrogée pour les informations de disponibilité de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="bf819-116">Identifies the time span queried for the user availability information.</span></span>  <br/><br/> <span data-ttu-id="bf819-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="bf819-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="bf819-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="bf819-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="bf819-119">Identifie l’intervalle de temps interrogé pour obtenir des informations détaillées sur les heures de réunion suggérées.</span><span class="sxs-lookup"><span data-stu-id="bf819-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/><br/> <span data-ttu-id="bf819-120">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="bf819-120">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[<span data-ttu-id="bf819-121">Durée (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="bf819-121">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="bf819-122">Spécifie la durée pendant laquelle l’État absent (absent du bureau) est activé si l’élément [OofState](oofstate.md) est défini sur **Planifié**.</span><span class="sxs-lookup"><span data-stu-id="bf819-122">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="bf819-123">Voici les expressions XPath possibles pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="bf819-123">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="bf819-124">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="bf819-124">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="bf819-125">Représente une occurrence d’élément de calendrier unique.</span><span class="sxs-lookup"><span data-stu-id="bf819-125">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="bf819-126">Cette information est utilisée pour les demandes de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="bf819-126">This is used for Availability inquiries.</span></span> <span data-ttu-id="bf819-127">L’élément **StartTime** est requis dans l’élément **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="bf819-127">The **StartTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="bf819-128">L’élément **StartTime** de l’élément **CalendarEvent** est propre au type **CalendarEvent** , bien qu’il contienne les mêmes valeurs de facette que les éléments **StartTime** du type **Duration** .</span><span class="sxs-lookup"><span data-stu-id="bf819-128">The **StartTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type although it contains the same facet values that the **StartTime** elements in the **Duration** type contain.</span></span>  <br/><br/> <span data-ttu-id="bf819-129">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="bf819-129">The following is the XPath expression to this element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bf819-130">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="bf819-130">Text value</span></span>

<span data-ttu-id="bf819-131">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="bf819-131">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bf819-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="bf819-132">Remarks</span></span>

<span data-ttu-id="bf819-133">L’élément [EndTime](endtime.md) représente la fin de l’intervalle de temps.</span><span class="sxs-lookup"><span data-stu-id="bf819-133">The [EndTime](endtime.md) element represents the end of the time span.</span></span> 
  
<span data-ttu-id="bf819-134">Le schéma comprend de nombreux éléments [StartTime](starttime.md) .</span><span class="sxs-lookup"><span data-stu-id="bf819-134">The schema includes many [StartTime](starttime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bf819-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="bf819-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="bf819-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bf819-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf819-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bf819-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf819-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bf819-138">Schema Name</span></span>  <br/> |<span data-ttu-id="bf819-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bf819-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="bf819-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bf819-140">Validation File</span></span>  <br/> |<span data-ttu-id="bf819-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bf819-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf819-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bf819-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="bf819-143">False</span><span class="sxs-lookup"><span data-stu-id="bf819-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf819-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bf819-144">See also</span></span>

- [<span data-ttu-id="bf819-145">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="bf819-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="bf819-146">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="bf819-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

