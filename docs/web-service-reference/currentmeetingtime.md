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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458774"
---
# <a name="currentmeetingtime"></a><span data-ttu-id="eba07-103">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="eba07-103">CurrentMeetingTime</span></span>

<span data-ttu-id="eba07-104">L’élément **CurrentMeetingTime** représente l’heure de début d’une réunion que vous souhaitez mettre à jour avec une heure de réunion proposée par un participant à la réunion.</span><span class="sxs-lookup"><span data-stu-id="eba07-104">The **CurrentMeetingTime** element represents the start time of a meeting that you want to update with a meeting time proposed by a meeting attendee.</span></span> 
  
[<span data-ttu-id="eba07-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="eba07-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="eba07-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="eba07-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="eba07-107">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="eba07-107">CurrentMeetingTime</span></span>](currentmeetingtime.md)
  
```xml
<CurrentMeetingTime>...</CurrentMeetingTime>
```

 <span data-ttu-id="eba07-108">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="eba07-108">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eba07-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="eba07-109">Attributes and elements</span></span>

<span data-ttu-id="eba07-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="eba07-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eba07-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="eba07-111">Attributes</span></span>

<span data-ttu-id="eba07-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="eba07-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eba07-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="eba07-113">Child elements</span></span>

<span data-ttu-id="eba07-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="eba07-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eba07-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="eba07-115">Parent elements</span></span>

|<span data-ttu-id="eba07-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eba07-116">**Element**</span></span>|<span data-ttu-id="eba07-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="eba07-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eba07-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="eba07-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="eba07-119">Contient les options permettant d’obtenir des informations sur les suggestions de réunion.</span><span class="sxs-lookup"><span data-stu-id="eba07-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="eba07-120">Voici le XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="eba07-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eba07-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="eba07-121">Remarks</span></span>

<span data-ttu-id="eba07-122">Cet élément n’est pas obligatoire.</span><span class="sxs-lookup"><span data-stu-id="eba07-122">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="eba07-123">Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur exécutant MicrosoftExchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="eba07-123">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="eba07-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="eba07-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eba07-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="eba07-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eba07-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="eba07-126">Schema Name</span></span>  <br/> |<span data-ttu-id="eba07-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="eba07-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="eba07-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="eba07-128">Validation File</span></span>  <br/> |<span data-ttu-id="eba07-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eba07-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eba07-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="eba07-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="eba07-131">False</span><span class="sxs-lookup"><span data-stu-id="eba07-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eba07-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="eba07-132">See also</span></span>



[<span data-ttu-id="eba07-133">Opération GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="eba07-133">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="eba07-134">Obtention de la disponibilité des utilisateurs</span><span class="sxs-lookup"><span data-stu-id="eba07-134">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

