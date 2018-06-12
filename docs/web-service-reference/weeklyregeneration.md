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
description: L’élément WeeklyRegeneration décrit la fréquence, en semaines, dans lequel une tâche est régénérée.
ms.openlocfilehash: 36cd3cc5c180f2b2cf53708e7787d0595f518def
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839047"
---
# <a name="weeklyregeneration"></a><span data-ttu-id="592c2-103">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="592c2-103">WeeklyRegeneration</span></span>

<span data-ttu-id="592c2-104">L’élément **WeeklyRegeneration** décrit la fréquence, en semaines, dans lequel une tâche est régénérée.</span><span class="sxs-lookup"><span data-stu-id="592c2-104">The **WeeklyRegeneration** element describes the frequency, in weeks, in which a task is regenerated.</span></span> 
  
```xml
<WeeklyRegeneration>
   <Interval/>
</WeeklyRegeneration>
```

 <span data-ttu-id="592c2-105">**WeeklyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="592c2-105">**WeeklyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="592c2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="592c2-106">Attributes and elements</span></span>

<span data-ttu-id="592c2-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="592c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="592c2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="592c2-108">Attributes</span></span>

<span data-ttu-id="592c2-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="592c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="592c2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="592c2-110">Child elements</span></span>

|<span data-ttu-id="592c2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="592c2-111">**Element**</span></span>|<span data-ttu-id="592c2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="592c2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="592c2-113">Intervalle</span><span class="sxs-lookup"><span data-stu-id="592c2-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="592c2-114">Définit l’intervalle, en semaines, dans la mesure où la tâche est terminée, après lequel une tâche est régénérée.</span><span class="sxs-lookup"><span data-stu-id="592c2-114">Defines the interval, in weeks, since the task was completed, after which a new task is regenerated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="592c2-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="592c2-115">Parent elements</span></span>

|<span data-ttu-id="592c2-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="592c2-116">**Element**</span></span>|<span data-ttu-id="592c2-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="592c2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="592c2-118">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="592c2-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="592c2-119">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="592c2-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="592c2-120">Note</span><span class="sxs-lookup"><span data-stu-id="592c2-120">Remarks</span></span>

<span data-ttu-id="592c2-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="592c2-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="592c2-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="592c2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="592c2-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="592c2-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="592c2-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="592c2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="592c2-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="592c2-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="592c2-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="592c2-126">Validation File</span></span>  <br/> |<span data-ttu-id="592c2-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="592c2-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="592c2-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="592c2-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="592c2-129">False</span><span class="sxs-lookup"><span data-stu-id="592c2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="592c2-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="592c2-130">See also</span></span>



- [<span data-ttu-id="592c2-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="592c2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

