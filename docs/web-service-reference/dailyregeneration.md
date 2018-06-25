---
title: DailyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DailyRegeneration
api_type:
- schema
ms.assetid: cafb57e4-c518-45e0-b565-2babd0dab1df
description: L’élément DailyRegeneration décrit la fréquence, en jours, dans laquelle une tâche est régénérée.
ms.openlocfilehash: 356f7fd2672b2ad87d17e597c52e9f12273ce3c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755788"
---
# <a name="dailyregeneration"></a><span data-ttu-id="7720b-103">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="7720b-103">DailyRegeneration</span></span>

<span data-ttu-id="7720b-104">L’élément **DailyRegeneration** décrit la fréquence, en jours, dans laquelle une tâche est régénérée.</span><span class="sxs-lookup"><span data-stu-id="7720b-104">The **DailyRegeneration** element describes the frequency, in days, in which a task is regenerated.</span></span> 
  
```xml
<DailyRegeneration>
   <Interval/>
</DailyRegeneration>
```

<span data-ttu-id="7720b-105">**DailyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="7720b-105">**DailyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7720b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7720b-106">Attributes and elements</span></span>

<span data-ttu-id="7720b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7720b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7720b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7720b-108">Attributes</span></span>

<span data-ttu-id="7720b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7720b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7720b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7720b-110">Child elements</span></span>

|<span data-ttu-id="7720b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7720b-111">**Element**</span></span>|<span data-ttu-id="7720b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7720b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7720b-113">Intervalle</span><span class="sxs-lookup"><span data-stu-id="7720b-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="7720b-114">Définit l’intervalle, en jours, entre deux éléments périodiques consécutives.</span><span class="sxs-lookup"><span data-stu-id="7720b-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="7720b-115">La valeur doit être compris entre 1 et 999.</span><span class="sxs-lookup"><span data-stu-id="7720b-115">The value must be in the range of 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7720b-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7720b-116">Parent elements</span></span>

|<span data-ttu-id="7720b-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7720b-117">**Element**</span></span>|<span data-ttu-id="7720b-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="7720b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7720b-119">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="7720b-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="7720b-120">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="7720b-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7720b-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="7720b-121">Remarks</span></span>

<span data-ttu-id="7720b-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7720b-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7720b-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7720b-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7720b-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7720b-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7720b-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7720b-125">Schema name</span></span>  <br/> |<span data-ttu-id="7720b-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7720b-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="7720b-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7720b-127">Validation file</span></span>  <br/> |<span data-ttu-id="7720b-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7720b-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7720b-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7720b-129">Can be empty</span></span>  <br/> |<span data-ttu-id="7720b-130">False</span><span class="sxs-lookup"><span data-stu-id="7720b-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7720b-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7720b-131">See also</span></span>

- [<span data-ttu-id="7720b-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7720b-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

