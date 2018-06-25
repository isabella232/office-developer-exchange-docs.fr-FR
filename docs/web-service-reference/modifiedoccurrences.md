---
title: ModifiedOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedOccurrences
api_type:
- schema
ms.assetid: 552932fc-b3b4-486e-8d73-32c0bb10bd68
description: L’élément ModifiedOccurrences contient un tableau d’occurrences d’élément calendrier périodiques qui ont été modifiés afin qu’ils soient différents de celui de l’élément maître de périodicité.
ms.openlocfilehash: 53f60740bcaa2de6713e1b6a3d2874153285645a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828472"
---
# <a name="modifiedoccurrences"></a><span data-ttu-id="2eca6-103">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="2eca6-103">ModifiedOccurrences</span></span>

<span data-ttu-id="2eca6-104">L’élément **ModifiedOccurrences** contient un tableau d’occurrences d’élément calendrier périodiques qui ont été modifiés afin qu’ils soient différents de celui de l’élément maître de périodicité.</span><span class="sxs-lookup"><span data-stu-id="2eca6-104">The **ModifiedOccurrences** element contains an array of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span> 
  
```xml
<ModifiedOccurrences>
   <Occurrence/>
</ModifiedOccurrences>
```

 <span data-ttu-id="2eca6-105">**NonEmptyArrayOfOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="2eca6-105">**NonEmptyArrayOfOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2eca6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2eca6-106">Attributes and elements</span></span>

<span data-ttu-id="2eca6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2eca6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2eca6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2eca6-108">Attributes</span></span>

<span data-ttu-id="2eca6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2eca6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2eca6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2eca6-110">Child elements</span></span>

|<span data-ttu-id="2eca6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2eca6-111">**Element**</span></span>|<span data-ttu-id="2eca6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2eca6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2eca6-113">Occurrence</span><span class="sxs-lookup"><span data-stu-id="2eca6-113">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="2eca6-114">Représente une seule occurrence de modification d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="2eca6-114">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2eca6-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2eca6-115">Parent elements</span></span>

|<span data-ttu-id="2eca6-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2eca6-116">**Element**</span></span>|<span data-ttu-id="2eca6-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="2eca6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2eca6-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2eca6-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2eca6-119">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="2eca6-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2eca6-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2eca6-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2eca6-121">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2eca6-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2eca6-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="2eca6-122">Remarks</span></span>

<span data-ttu-id="2eca6-123">Cet élément n’est valide que si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="2eca6-123">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="2eca6-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2eca6-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2eca6-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2eca6-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2eca6-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2eca6-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2eca6-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2eca6-127">Schema name</span></span>  <br/> |<span data-ttu-id="2eca6-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2eca6-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="2eca6-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2eca6-129">Validation file</span></span>  <br/> |<span data-ttu-id="2eca6-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2eca6-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2eca6-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2eca6-131">Can be empty</span></span>  <br/> |<span data-ttu-id="2eca6-132">False</span><span class="sxs-lookup"><span data-stu-id="2eca6-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2eca6-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2eca6-133">See also</span></span>



- [<span data-ttu-id="2eca6-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2eca6-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

