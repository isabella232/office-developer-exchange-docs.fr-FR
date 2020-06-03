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
ms.openlocfilehash: e79616fd735cbf6410e85450bd75c1276923f171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458774"
---
# <a name="currentmeetingtime"></a><span data-ttu-id="86ccf-103">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="86ccf-103">CurrentMeetingTime</span></span>

<span data-ttu-id="86ccf-104">L’élément **CurrentMeetingTime** représente l’heure de début d’une réunion que vous souhaitez mettre à jour avec une heure de réunion proposée par un participant à la réunion.</span><span class="sxs-lookup"><span data-stu-id="86ccf-104">The **CurrentMeetingTime** element represents the start time of a meeting that you want to update with a meeting time proposed by a meeting attendee.</span></span> 
  
[<span data-ttu-id="86ccf-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="86ccf-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="86ccf-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="86ccf-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="86ccf-107">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="86ccf-107">CurrentMeetingTime</span></span>](currentmeetingtime.md)
  
```xml
<CurrentMeetingTime>...</CurrentMeetingTime>
```

 <span data-ttu-id="86ccf-108">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="86ccf-108">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86ccf-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="86ccf-109">Attributes and elements</span></span>

<span data-ttu-id="86ccf-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="86ccf-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86ccf-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="86ccf-111">Attributes</span></span>

<span data-ttu-id="86ccf-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="86ccf-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86ccf-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="86ccf-113">Child elements</span></span>

<span data-ttu-id="86ccf-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="86ccf-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="86ccf-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="86ccf-115">Parent elements</span></span>

|<span data-ttu-id="86ccf-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="86ccf-116">**Element**</span></span>|<span data-ttu-id="86ccf-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="86ccf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86ccf-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="86ccf-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="86ccf-119">Contient les options permettant d’obtenir des informations sur les suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="86ccf-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="86ccf-120">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="86ccf-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="86ccf-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="86ccf-121">Remarks</span></span>

<span data-ttu-id="86ccf-122">Cet élément n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="86ccf-122">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="86ccf-123">Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur exécutant MicrosoftExchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="86ccf-123">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="86ccf-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="86ccf-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86ccf-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="86ccf-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86ccf-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="86ccf-126">Schema Name</span></span>  <br/> |<span data-ttu-id="86ccf-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="86ccf-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="86ccf-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="86ccf-128">Validation File</span></span>  <br/> |<span data-ttu-id="86ccf-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="86ccf-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="86ccf-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="86ccf-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="86ccf-131">False</span><span class="sxs-lookup"><span data-stu-id="86ccf-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="86ccf-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="86ccf-132">See also</span></span>



[<span data-ttu-id="86ccf-133">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="86ccf-133">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="86ccf-134">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="86ccf-134">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

