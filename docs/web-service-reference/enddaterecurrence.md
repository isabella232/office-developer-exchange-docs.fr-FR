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
description: L’élément EndDateRecurrence décrit la date de début et date de fin de périodicité d’un élément.
ms.openlocfilehash: 73450bf69c6b122e806d85011975159e348ad740
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756176"
---
# <a name="enddaterecurrence"></a><span data-ttu-id="2b0e5-103">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="2b0e5-103">EndDateRecurrence</span></span>

<span data-ttu-id="2b0e5-104">L’élément **EndDateRecurrence** décrit la date de début et date de fin de périodicité d’un élément.</span><span class="sxs-lookup"><span data-stu-id="2b0e5-104">The **EndDateRecurrence** element describes the start date and the end date of an item recurrence pattern.</span></span> 
  
```xml
<EndDateRecurrence>
   <StartDate/>
   <EndDate/>
</EndDateRecurrence>
```

 <span data-ttu-id="2b0e5-105">**EndDateRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="2b0e5-105">**EndDateRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b0e5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2b0e5-106">Attributes and elements</span></span>

<span data-ttu-id="2b0e5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2b0e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b0e5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2b0e5-108">Attributes</span></span>

<span data-ttu-id="2b0e5-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2b0e5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b0e5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2b0e5-110">Child elements</span></span>

|<span data-ttu-id="2b0e5-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2b0e5-111">**Element**</span></span>|<span data-ttu-id="2b0e5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b0e5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b0e5-113">StartDate (périodicité)</span><span class="sxs-lookup"><span data-stu-id="2b0e5-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="2b0e5-114">Représente la date de début d’une tâche périodique ou d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="2b0e5-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2b0e5-115">EndDate (périodicité)</span><span class="sxs-lookup"><span data-stu-id="2b0e5-115">EndDate (Recurrence)</span></span>](enddate-recurrence.md) <br/> |<span data-ttu-id="2b0e5-116">Représente la date de fin d’une tâche périodique ou d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="2b0e5-116">Represents the end date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2b0e5-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2b0e5-117">Parent elements</span></span>

|<span data-ttu-id="2b0e5-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2b0e5-118">**Element**</span></span>|<span data-ttu-id="2b0e5-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="2b0e5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b0e5-120">Périodicité (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="2b0e5-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="2b0e5-121">Contient la périodicité pour les éléments de calendrier et les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="2b0e5-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="2b0e5-122">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="2b0e5-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="2b0e5-123">Contient la périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="2b0e5-123">Contains the recurrence pattern for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2b0e5-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="2b0e5-124">Remarks</span></span>

<span data-ttu-id="2b0e5-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2b0e5-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b0e5-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2b0e5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b0e5-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2b0e5-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b0e5-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2b0e5-128">Schema name</span></span>  <br/> |<span data-ttu-id="2b0e5-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2b0e5-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b0e5-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2b0e5-130">Validation file</span></span>  <br/> |<span data-ttu-id="2b0e5-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b0e5-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b0e5-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2b0e5-132">Can be empty</span></span>  <br/> |<span data-ttu-id="2b0e5-133">False</span><span class="sxs-lookup"><span data-stu-id="2b0e5-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b0e5-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2b0e5-134">See also</span></span>



- [<span data-ttu-id="2b0e5-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2b0e5-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

