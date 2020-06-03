---
title: WeeklyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WeeklyRegeneration
api_type:
- schema
ms.assetid: f128fdaa-ca3d-4614-8e55-f25e76a67b6c
description: L’élément WeeklyRegeneration décrit la fréquence, en semaines, de régénération d’une tâche.
ms.openlocfilehash: dc333e051fd2213942e629a3f2764c72abfaeba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459748"
---
# <a name="weeklyregeneration"></a><span data-ttu-id="fc61f-103">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="fc61f-103">WeeklyRegeneration</span></span>

<span data-ttu-id="fc61f-104">L’élément **WeeklyRegeneration** décrit la fréquence, en semaines, de régénération d’une tâche.</span><span class="sxs-lookup"><span data-stu-id="fc61f-104">The **WeeklyRegeneration** element describes the frequency, in weeks, in which a task is regenerated.</span></span> 
  
```xml
<WeeklyRegeneration>
   <Interval/>
</WeeklyRegeneration>
```

 <span data-ttu-id="fc61f-105">**WeeklyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="fc61f-105">**WeeklyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc61f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fc61f-106">Attributes and elements</span></span>

<span data-ttu-id="fc61f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fc61f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc61f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fc61f-108">Attributes</span></span>

<span data-ttu-id="fc61f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fc61f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc61f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fc61f-110">Child elements</span></span>

|<span data-ttu-id="fc61f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fc61f-111">**Element**</span></span>|<span data-ttu-id="fc61f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="fc61f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc61f-113">Interval</span><span class="sxs-lookup"><span data-stu-id="fc61f-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="fc61f-114">Définit l’intervalle, en semaines, depuis la fin de la tâche, après lequel une nouvelle tâche est régénérée.</span><span class="sxs-lookup"><span data-stu-id="fc61f-114">Defines the interval, in weeks, since the task was completed, after which a new task is regenerated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc61f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fc61f-115">Parent elements</span></span>

|<span data-ttu-id="fc61f-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fc61f-116">**Element**</span></span>|<span data-ttu-id="fc61f-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="fc61f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc61f-118">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="fc61f-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="fc61f-119">Contient des informations de récurrence pour les tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="fc61f-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fc61f-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="fc61f-120">Remarks</span></span>

<span data-ttu-id="fc61f-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fc61f-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc61f-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fc61f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc61f-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fc61f-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc61f-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fc61f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="fc61f-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fc61f-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="fc61f-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fc61f-126">Validation File</span></span>  <br/> |<span data-ttu-id="fc61f-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fc61f-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc61f-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fc61f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc61f-129">False</span><span class="sxs-lookup"><span data-stu-id="fc61f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc61f-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fc61f-130">See also</span></span>



- [<span data-ttu-id="fc61f-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fc61f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

