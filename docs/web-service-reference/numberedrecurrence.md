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
ms.openlocfilehash: 000674e5b0bad9deea5aa4ac78d41135a922c755
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465939"
---
# <a name="numberedrecurrence"></a><span data-ttu-id="f7138-103">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="f7138-103">NumberedRecurrence</span></span>

<span data-ttu-id="f7138-104">L’élément **NumberedRecurrence** décrit la date de début et le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="f7138-104">The **NumberedRecurrence** element describes the start date and the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberedRecurrence>
   <StartDate/>
   <NumberOfOccurrences/>
</NumberedRecurrence>
```

 <span data-ttu-id="f7138-105">**NumberedRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="f7138-105">**NumberedRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7138-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f7138-106">Attributes and elements</span></span>

<span data-ttu-id="f7138-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f7138-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7138-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f7138-108">Attributes</span></span>

<span data-ttu-id="f7138-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f7138-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7138-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f7138-110">Child elements</span></span>

|<span data-ttu-id="f7138-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7138-111">**Element**</span></span>|<span data-ttu-id="f7138-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7138-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7138-113">StartDate (périodicité)</span><span class="sxs-lookup"><span data-stu-id="f7138-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="f7138-114">Représente la date de début d’une tâche périodique ou d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="f7138-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f7138-115">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="f7138-115">NumberOfOccurrences</span></span>](numberofoccurrences.md) <br/> |<span data-ttu-id="f7138-116">Contient le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="f7138-116">Contains the number of occurrences of a recurring item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7138-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f7138-117">Parent elements</span></span>

|<span data-ttu-id="f7138-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7138-118">**Element**</span></span>|<span data-ttu-id="f7138-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7138-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7138-120">Récurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="f7138-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="f7138-121">Contient la périodicité des éléments de calendrier et des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="f7138-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="f7138-122">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="f7138-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="f7138-123">Contient des informations de récurrence pour les tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="f7138-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f7138-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="f7138-124">Remarks</span></span>

<span data-ttu-id="f7138-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f7138-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7138-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f7138-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7138-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f7138-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7138-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f7138-128">Schema name</span></span>  <br/> |<span data-ttu-id="f7138-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f7138-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7138-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f7138-130">Validation file</span></span>  <br/> |<span data-ttu-id="f7138-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f7138-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7138-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f7138-132">Can be empty</span></span>  <br/> |<span data-ttu-id="f7138-133">False</span><span class="sxs-lookup"><span data-stu-id="f7138-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7138-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f7138-134">See also</span></span>



- [<span data-ttu-id="f7138-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f7138-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

