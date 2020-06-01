---
title: EndDateRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDateRecurrence
api_type:
- schema
ms.assetid: a5ee2504-db84-49ee-870c-cca9269f2e26
description: L’élément EndDateRecurrence décrit la date de début et la date de fin d’une périodicité d’élément.
ms.openlocfilehash: e8ae72012e5bcac8d8b2a06b6d3a9b3a7caf30d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460147"
---
# <a name="enddaterecurrence"></a><span data-ttu-id="997f5-103">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="997f5-103">EndDateRecurrence</span></span>

<span data-ttu-id="997f5-104">L’élément **EndDateRecurrence** décrit la date de début et la date de fin d’une périodicité d’élément.</span><span class="sxs-lookup"><span data-stu-id="997f5-104">The **EndDateRecurrence** element describes the start date and the end date of an item recurrence pattern.</span></span> 
  
```xml
<EndDateRecurrence>
   <StartDate/>
   <EndDate/>
</EndDateRecurrence>
```

 <span data-ttu-id="997f5-105">**EndDateRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="997f5-105">**EndDateRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="997f5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="997f5-106">Attributes and elements</span></span>

<span data-ttu-id="997f5-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="997f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="997f5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="997f5-108">Attributes</span></span>

<span data-ttu-id="997f5-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="997f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="997f5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="997f5-110">Child elements</span></span>

|<span data-ttu-id="997f5-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="997f5-111">**Element**</span></span>|<span data-ttu-id="997f5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="997f5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="997f5-113">StartDate (périodicité)</span><span class="sxs-lookup"><span data-stu-id="997f5-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="997f5-114">Représente la date de début d’une tâche périodique ou d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="997f5-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="997f5-115">EndDate (récurrence)</span><span class="sxs-lookup"><span data-stu-id="997f5-115">EndDate (Recurrence)</span></span>](enddate-recurrence.md) <br/> |<span data-ttu-id="997f5-116">Représente la date de fin d’une tâche périodique ou d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="997f5-116">Represents the end date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="997f5-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="997f5-117">Parent elements</span></span>

|<span data-ttu-id="997f5-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="997f5-118">**Element**</span></span>|<span data-ttu-id="997f5-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="997f5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="997f5-120">Récurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="997f5-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="997f5-121">Contient la périodicité des éléments de calendrier et des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="997f5-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="997f5-122">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="997f5-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="997f5-123">Contient la périodicité des tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="997f5-123">Contains the recurrence pattern for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="997f5-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="997f5-124">Remarks</span></span>

<span data-ttu-id="997f5-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="997f5-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="997f5-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="997f5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="997f5-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="997f5-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="997f5-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="997f5-128">Schema name</span></span>  <br/> |<span data-ttu-id="997f5-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="997f5-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="997f5-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="997f5-130">Validation file</span></span>  <br/> |<span data-ttu-id="997f5-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="997f5-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="997f5-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="997f5-132">Can be empty</span></span>  <br/> |<span data-ttu-id="997f5-133">False</span><span class="sxs-lookup"><span data-stu-id="997f5-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="997f5-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="997f5-134">See also</span></span>



- [<span data-ttu-id="997f5-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="997f5-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

