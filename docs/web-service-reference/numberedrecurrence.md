---
title: NumberedRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberedRecurrence
api_type:
- schema
ms.assetid: 53746909-ef21-4764-8715-a7769b943cca
description: L’élément NumberedRecurrence décrit la date de début et le nombre d’occurrences d’un élément périodique.
ms.openlocfilehash: 01fbf831fa7ff378221d4db3d873af730ac564d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828628"
---
# <a name="numberedrecurrence"></a><span data-ttu-id="05496-103">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="05496-103">NumberedRecurrence</span></span>

<span data-ttu-id="05496-104">L’élément **NumberedRecurrence** décrit la date de début et le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="05496-104">The **NumberedRecurrence** element describes the start date and the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberedRecurrence>
   <StartDate/>
   <NumberOfOccurrences/>
</NumberedRecurrence>
```

 <span data-ttu-id="05496-105">**NumberedRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="05496-105">**NumberedRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05496-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="05496-106">Attributes and elements</span></span>

<span data-ttu-id="05496-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="05496-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05496-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="05496-108">Attributes</span></span>

<span data-ttu-id="05496-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05496-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05496-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="05496-110">Child elements</span></span>

|<span data-ttu-id="05496-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="05496-111">**Element**</span></span>|<span data-ttu-id="05496-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="05496-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05496-113">StartDate (périodicité)</span><span class="sxs-lookup"><span data-stu-id="05496-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="05496-114">Représente la date de début d’une tâche périodique ou d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="05496-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="05496-115">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="05496-115">NumberOfOccurrences</span></span>](numberofoccurrences.md) <br/> |<span data-ttu-id="05496-116">Contient le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="05496-116">Contains the number of occurrences of a recurring item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="05496-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="05496-117">Parent elements</span></span>

|<span data-ttu-id="05496-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="05496-118">**Element**</span></span>|<span data-ttu-id="05496-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="05496-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05496-120">Périodicité (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="05496-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="05496-121">Contient la périodicité pour les éléments de calendrier et les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="05496-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="05496-122">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="05496-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="05496-123">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="05496-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="05496-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="05496-124">Remarks</span></span>

<span data-ttu-id="05496-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="05496-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05496-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="05496-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05496-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="05496-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05496-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="05496-128">Schema name</span></span>  <br/> |<span data-ttu-id="05496-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="05496-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="05496-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="05496-130">Validation file</span></span>  <br/> |<span data-ttu-id="05496-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05496-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05496-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="05496-132">Can be empty</span></span>  <br/> |<span data-ttu-id="05496-133">False</span><span class="sxs-lookup"><span data-stu-id="05496-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05496-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05496-134">See also</span></span>



- [<span data-ttu-id="05496-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="05496-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

