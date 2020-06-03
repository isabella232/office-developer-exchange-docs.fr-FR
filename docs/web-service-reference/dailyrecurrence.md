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
description: L’élément DailyRecurrence décrit la fréquence, en jours, à laquelle un élément de calendrier ou une tâche se répète.
ms.openlocfilehash: d18a04ced19c87996c3a092f6668ab00c5a3f006
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462170"
---
# <a name="dailyrecurrence"></a><span data-ttu-id="04610-103">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="04610-103">DailyRecurrence</span></span>

<span data-ttu-id="04610-104">L’élément **DailyRecurrence** décrit la fréquence, en jours, à laquelle un élément de calendrier ou une tâche se répète.</span><span class="sxs-lookup"><span data-stu-id="04610-104">The **DailyRecurrence** element describes the frequency, in days, in which a calendar item or a task recurs.</span></span> 
  
```xml
<DailyRecurrence>
   <Interval/>
</DailyRecurrence>
```

<span data-ttu-id="04610-105">**DailyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="04610-105">**DailyRecurrencePatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="04610-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="04610-106">Attributes and elements</span></span>

<span data-ttu-id="04610-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="04610-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04610-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="04610-108">Attributes</span></span>

<span data-ttu-id="04610-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="04610-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04610-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="04610-110">Child elements</span></span>

|<span data-ttu-id="04610-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04610-111">**Element**</span></span>|<span data-ttu-id="04610-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="04610-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04610-113">Interval</span><span class="sxs-lookup"><span data-stu-id="04610-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="04610-114">Définit l’intervalle, en jours, entre deux éléments périodiques consécutifs.</span><span class="sxs-lookup"><span data-stu-id="04610-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="04610-115">La valeur doit être comprise entre 1 et 999.</span><span class="sxs-lookup"><span data-stu-id="04610-115">The value must be in the range from 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04610-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="04610-116">Parent elements</span></span>

|<span data-ttu-id="04610-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04610-117">**Element**</span></span>|<span data-ttu-id="04610-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="04610-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04610-119">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="04610-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="04610-120">Contient des informations de récurrence pour les tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="04610-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="04610-121">Récurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="04610-121">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="04610-122">Contient la périodicité des éléments de calendrier et des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="04610-122">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="04610-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="04610-123">Remarks</span></span>

<span data-ttu-id="04610-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="04610-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04610-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="04610-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04610-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="04610-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04610-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="04610-127">Schema name</span></span>  <br/> |<span data-ttu-id="04610-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="04610-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="04610-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="04610-129">Validation file</span></span>  <br/> |<span data-ttu-id="04610-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="04610-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04610-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="04610-131">Can be empty</span></span>  <br/> |<span data-ttu-id="04610-132">False</span><span class="sxs-lookup"><span data-stu-id="04610-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04610-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="04610-133">See also</span></span>

- [<span data-ttu-id="04610-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="04610-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

