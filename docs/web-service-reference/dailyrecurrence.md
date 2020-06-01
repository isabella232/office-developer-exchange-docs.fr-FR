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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462170"
---
# <a name="dailyrecurrence"></a><span data-ttu-id="ded01-103">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="ded01-103">DailyRecurrence</span></span>

<span data-ttu-id="ded01-104">L’élément **DailyRecurrence** décrit la fréquence, en jours, à laquelle un élément de calendrier ou une tâche se répète.</span><span class="sxs-lookup"><span data-stu-id="ded01-104">The **DailyRecurrence** element describes the frequency, in days, in which a calendar item or a task recurs.</span></span> 
  
```xml
<DailyRecurrence>
   <Interval/>
</DailyRecurrence>
```

<span data-ttu-id="ded01-105">**DailyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="ded01-105">**DailyRecurrencePatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ded01-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ded01-106">Attributes and elements</span></span>

<span data-ttu-id="ded01-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ded01-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ded01-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ded01-108">Attributes</span></span>

<span data-ttu-id="ded01-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ded01-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ded01-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ded01-110">Child elements</span></span>

|<span data-ttu-id="ded01-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ded01-111">**Element**</span></span>|<span data-ttu-id="ded01-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ded01-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ded01-113">Interval</span><span class="sxs-lookup"><span data-stu-id="ded01-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="ded01-114">Définit l’intervalle, en jours, entre deux éléments périodiques consécutifs.</span><span class="sxs-lookup"><span data-stu-id="ded01-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="ded01-115">La valeur doit être comprise entre 1 et 999.</span><span class="sxs-lookup"><span data-stu-id="ded01-115">The value must be in the range from 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ded01-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ded01-116">Parent elements</span></span>

|<span data-ttu-id="ded01-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ded01-117">**Element**</span></span>|<span data-ttu-id="ded01-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="ded01-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ded01-119">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="ded01-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="ded01-120">Contient des informations de récurrence pour les tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="ded01-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="ded01-121">Récurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="ded01-121">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="ded01-122">Contient la périodicité des éléments de calendrier et des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="ded01-122">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ded01-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="ded01-123">Remarks</span></span>

<span data-ttu-id="ded01-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ded01-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ded01-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ded01-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ded01-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ded01-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ded01-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ded01-127">Schema name</span></span>  <br/> |<span data-ttu-id="ded01-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ded01-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="ded01-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ded01-129">Validation file</span></span>  <br/> |<span data-ttu-id="ded01-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ded01-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ded01-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ded01-131">Can be empty</span></span>  <br/> |<span data-ttu-id="ded01-132">False</span><span class="sxs-lookup"><span data-stu-id="ded01-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ded01-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ded01-133">See also</span></span>

- [<span data-ttu-id="ded01-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ded01-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

