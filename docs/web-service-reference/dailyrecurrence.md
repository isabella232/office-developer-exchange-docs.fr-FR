---
title: DailyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DailyRecurrence
api_type:
- schema
ms.assetid: 0aaf265d-b723-49c6-8e9c-9ba60141e9ab
description: L’élément DailyRecurrence décrit la fréquence, en jours, dans laquelle un élément de calendrier ou d’une tâche est périodique.
ms.openlocfilehash: d02c1f7425372d60c10b40527dc5f0d65f923b45
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755784"
---
# <a name="dailyrecurrence"></a><span data-ttu-id="7fb22-103">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="7fb22-103">DailyRecurrence</span></span>

<span data-ttu-id="7fb22-104">L’élément **DailyRecurrence** décrit la fréquence, en jours, dans laquelle un élément de calendrier ou d’une tâche est périodique.</span><span class="sxs-lookup"><span data-stu-id="7fb22-104">The **DailyRecurrence** element describes the frequency, in days, in which a calendar item or a task recurs.</span></span> 
  
```xml
<DailyRecurrence>
   <Interval/>
</DailyRecurrence>
```

<span data-ttu-id="7fb22-105">**DailyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="7fb22-105">**DailyRecurrencePatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7fb22-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7fb22-106">Attributes and elements</span></span>

<span data-ttu-id="7fb22-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7fb22-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7fb22-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7fb22-108">Attributes</span></span>

<span data-ttu-id="7fb22-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7fb22-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7fb22-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7fb22-110">Child elements</span></span>

|<span data-ttu-id="7fb22-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7fb22-111">**Element**</span></span>|<span data-ttu-id="7fb22-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7fb22-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7fb22-113">Intervalle</span><span class="sxs-lookup"><span data-stu-id="7fb22-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="7fb22-114">Définit l’intervalle, en jours, entre deux éléments périodiques consécutives.</span><span class="sxs-lookup"><span data-stu-id="7fb22-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="7fb22-115">La valeur doit être compris entre 1 et 999.</span><span class="sxs-lookup"><span data-stu-id="7fb22-115">The value must be in the range from 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7fb22-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7fb22-116">Parent elements</span></span>

|<span data-ttu-id="7fb22-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7fb22-117">**Element**</span></span>|<span data-ttu-id="7fb22-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="7fb22-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7fb22-119">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="7fb22-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="7fb22-120">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="7fb22-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="7fb22-121">Périodicité (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="7fb22-121">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="7fb22-122">Contient la périodicité pour les éléments de calendrier et les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="7fb22-122">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7fb22-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="7fb22-123">Remarks</span></span>

<span data-ttu-id="7fb22-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7fb22-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7fb22-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7fb22-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7fb22-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7fb22-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7fb22-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7fb22-127">Schema name</span></span>  <br/> |<span data-ttu-id="7fb22-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7fb22-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="7fb22-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7fb22-129">Validation file</span></span>  <br/> |<span data-ttu-id="7fb22-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7fb22-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7fb22-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7fb22-131">Can be empty</span></span>  <br/> |<span data-ttu-id="7fb22-132">False</span><span class="sxs-lookup"><span data-stu-id="7fb22-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7fb22-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7fb22-133">See also</span></span>

- [<span data-ttu-id="7fb22-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7fb22-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

