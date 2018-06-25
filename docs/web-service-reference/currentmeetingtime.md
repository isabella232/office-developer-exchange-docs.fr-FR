---
title: CurrentMeetingTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CurrentMeetingTime
api_type:
- schema
ms.assetid: 1ff68154-24b5-465a-a31c-3d3bab0d491e
description: L’élément CurrentMeetingTime représente l’heure de début d’une réunion que vous souhaitez mettre à jour avec une heure de réunion proposée par un participant à la réunion.
ms.openlocfilehash: 88adbe566270d759986e9b55afd4827c0513ca43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755766"
---
# <a name="currentmeetingtime"></a><span data-ttu-id="8b6d4-103">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="8b6d4-103">CurrentMeetingTime</span></span>

<span data-ttu-id="8b6d4-104">L’élément **CurrentMeetingTime** représente l’heure de début d’une réunion que vous souhaitez mettre à jour avec une heure de réunion proposée par un participant à la réunion.</span><span class="sxs-lookup"><span data-stu-id="8b6d4-104">The **CurrentMeetingTime** element represents the start time of a meeting that you want to update with a meeting time proposed by a meeting attendee.</span></span> 
  
[<span data-ttu-id="8b6d4-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="8b6d4-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="8b6d4-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="8b6d4-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="8b6d4-107">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="8b6d4-107">CurrentMeetingTime</span></span>](currentmeetingtime.md)
  
```xml
<CurrentMeetingTime>...</CurrentMeetingTime>
```

 <span data-ttu-id="8b6d4-108">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="8b6d4-108">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b6d4-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8b6d4-109">Attributes and elements</span></span>

<span data-ttu-id="8b6d4-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8b6d4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b6d4-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="8b6d4-111">Attributes</span></span>

<span data-ttu-id="8b6d4-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8b6d4-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b6d4-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8b6d4-113">Child elements</span></span>

<span data-ttu-id="8b6d4-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8b6d4-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8b6d4-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8b6d4-115">Parent elements</span></span>

|<span data-ttu-id="8b6d4-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8b6d4-116">**Element**</span></span>|<span data-ttu-id="8b6d4-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="8b6d4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b6d4-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="8b6d4-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="8b6d4-119">Contient les options permettant d’obtenir des informations de suggestion de réunion.</span><span class="sxs-lookup"><span data-stu-id="8b6d4-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="8b6d4-120">Vous trouverez ci-dessous le XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="8b6d4-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8b6d4-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="8b6d4-121">Remarks</span></span>

<span data-ttu-id="8b6d4-122">Cet élément n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="8b6d4-122">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="8b6d4-123">Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="8b6d4-123">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8b6d4-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8b6d4-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b6d4-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8b6d4-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b6d4-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8b6d4-126">Schema Name</span></span>  <br/> |<span data-ttu-id="8b6d4-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8b6d4-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b6d4-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8b6d4-128">Validation File</span></span>  <br/> |<span data-ttu-id="8b6d4-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8b6d4-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b6d4-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8b6d4-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="8b6d4-131">False</span><span class="sxs-lookup"><span data-stu-id="8b6d4-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b6d4-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8b6d4-132">See also</span></span>



[<span data-ttu-id="8b6d4-133">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="8b6d4-133">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="8b6d4-134">Obtention de disponibilité de l’utilisateur</span><span class="sxs-lookup"><span data-stu-id="8b6d4-134">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

