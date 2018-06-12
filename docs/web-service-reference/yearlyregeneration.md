---
title: YearlyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- YearlyRegeneration
api_type:
- schema
ms.assetid: 23538bca-738e-4319-944e-f459ff8a7eba
description: L’élément YearlyRegeneration décrit la fréquence, en années, dans lequel une tâche est régénérée.
ms.openlocfilehash: d034be1ff70e92fd5e96118b9fd1eb3033737f6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839073"
---
# <a name="yearlyregeneration"></a><span data-ttu-id="034dd-103">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="034dd-103">YearlyRegeneration</span></span>

<span data-ttu-id="034dd-104">L’élément **YearlyRegeneration** décrit la fréquence, en années, dans lequel une tâche est régénérée.</span><span class="sxs-lookup"><span data-stu-id="034dd-104">The **YearlyRegeneration** element describes the frequency, in years, in which a task is regenerated.</span></span> 
  
```xml
<YearlyRegeneratingPatternType>
   <Interval/>
</YearlyRegeneratingPatternType>
```

<span data-ttu-id="034dd-105">**YearlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="034dd-105">**YearlyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="034dd-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="034dd-106">Attributes and elements</span></span>

<span data-ttu-id="034dd-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="034dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="034dd-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="034dd-108">Attributes</span></span>

<span data-ttu-id="034dd-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="034dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="034dd-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="034dd-110">Child elements</span></span>

|<span data-ttu-id="034dd-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="034dd-111">**Element**</span></span>|<span data-ttu-id="034dd-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="034dd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="034dd-113">Intervalle</span><span class="sxs-lookup"><span data-stu-id="034dd-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="034dd-114">Définit l’intervalle, en années, pendant laquelle une nouvelle tâche est régénérée après la fin de la tâche.</span><span class="sxs-lookup"><span data-stu-id="034dd-114">Defines the interval, in years, during which a new task is regenerated after the completion of the task.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="034dd-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="034dd-115">Parent elements</span></span>

|<span data-ttu-id="034dd-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="034dd-116">**Element**</span></span>|<span data-ttu-id="034dd-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="034dd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="034dd-118">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="034dd-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="034dd-119">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="034dd-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="034dd-120">Note</span><span class="sxs-lookup"><span data-stu-id="034dd-120">Remarks</span></span>

<span data-ttu-id="034dd-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="034dd-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="034dd-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="034dd-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="034dd-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="034dd-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="034dd-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="034dd-124">Schema Name</span></span>  <br/> |<span data-ttu-id="034dd-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="034dd-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="034dd-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="034dd-126">Validation File</span></span>  <br/> |<span data-ttu-id="034dd-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="034dd-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="034dd-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="034dd-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="034dd-129">False</span><span class="sxs-lookup"><span data-stu-id="034dd-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="034dd-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="034dd-130">See also</span></span>

- [<span data-ttu-id="034dd-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="034dd-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

