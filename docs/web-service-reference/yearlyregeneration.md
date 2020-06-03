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
description: L’élément YearlyRegeneration décrit la fréquence, exprimée en années, à laquelle une tâche est régénérée.
ms.openlocfilehash: 7a6796c433bc54d145d5a769e01f9bba46897735
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457878"
---
# <a name="yearlyregeneration"></a><span data-ttu-id="d26b9-103">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="d26b9-103">YearlyRegeneration</span></span>

<span data-ttu-id="d26b9-104">L’élément **YearlyRegeneration** décrit la fréquence, exprimée en années, à laquelle une tâche est régénérée.</span><span class="sxs-lookup"><span data-stu-id="d26b9-104">The **YearlyRegeneration** element describes the frequency, in years, in which a task is regenerated.</span></span> 
  
```xml
<YearlyRegeneratingPatternType>
   <Interval/>
</YearlyRegeneratingPatternType>
```

<span data-ttu-id="d26b9-105">**YearlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="d26b9-105">**YearlyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d26b9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d26b9-106">Attributes and elements</span></span>

<span data-ttu-id="d26b9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d26b9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d26b9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d26b9-108">Attributes</span></span>

<span data-ttu-id="d26b9-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d26b9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d26b9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d26b9-110">Child elements</span></span>

|<span data-ttu-id="d26b9-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d26b9-111">**Element**</span></span>|<span data-ttu-id="d26b9-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d26b9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d26b9-113">Interval</span><span class="sxs-lookup"><span data-stu-id="d26b9-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="d26b9-114">Définit l’intervalle, en années, pendant lequel une nouvelle tâche est régénérée après la fin de la tâche.</span><span class="sxs-lookup"><span data-stu-id="d26b9-114">Defines the interval, in years, during which a new task is regenerated after the completion of the task.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d26b9-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d26b9-115">Parent elements</span></span>

|<span data-ttu-id="d26b9-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d26b9-116">**Element**</span></span>|<span data-ttu-id="d26b9-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d26b9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d26b9-118">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d26b9-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="d26b9-119">Contient des informations de récurrence pour les tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="d26b9-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d26b9-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="d26b9-120">Remarks</span></span>

<span data-ttu-id="d26b9-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d26b9-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d26b9-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d26b9-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d26b9-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d26b9-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d26b9-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d26b9-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d26b9-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d26b9-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="d26b9-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d26b9-126">Validation File</span></span>  <br/> |<span data-ttu-id="d26b9-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d26b9-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d26b9-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d26b9-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="d26b9-129">False</span><span class="sxs-lookup"><span data-stu-id="d26b9-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d26b9-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d26b9-130">See also</span></span>

- [<span data-ttu-id="d26b9-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d26b9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

