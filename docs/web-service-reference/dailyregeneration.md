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
description: L’élément DailyRegeneration décrit la fréquence, en jours, de régénération d’une tâche.
ms.openlocfilehash: 518e4666031131f4a5fc80cc72c28a2110b468c5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462163"
---
# <a name="dailyregeneration"></a><span data-ttu-id="8c137-103">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="8c137-103">DailyRegeneration</span></span>

<span data-ttu-id="8c137-104">L’élément **DailyRegeneration** décrit la fréquence, en jours, de régénération d’une tâche.</span><span class="sxs-lookup"><span data-stu-id="8c137-104">The **DailyRegeneration** element describes the frequency, in days, in which a task is regenerated.</span></span> 
  
```xml
<DailyRegeneration>
   <Interval/>
</DailyRegeneration>
```

<span data-ttu-id="8c137-105">**DailyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="8c137-105">**DailyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8c137-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8c137-106">Attributes and elements</span></span>

<span data-ttu-id="8c137-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8c137-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c137-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8c137-108">Attributes</span></span>

<span data-ttu-id="8c137-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8c137-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8c137-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8c137-110">Child elements</span></span>

|<span data-ttu-id="8c137-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8c137-111">**Element**</span></span>|<span data-ttu-id="8c137-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8c137-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c137-113">Interval</span><span class="sxs-lookup"><span data-stu-id="8c137-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="8c137-114">Définit l’intervalle, en jours, entre deux éléments périodiques consécutifs.</span><span class="sxs-lookup"><span data-stu-id="8c137-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="8c137-115">La valeur doit être comprise entre 1 et 999.</span><span class="sxs-lookup"><span data-stu-id="8c137-115">The value must be in the range of 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8c137-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8c137-116">Parent elements</span></span>

|<span data-ttu-id="8c137-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8c137-117">**Element**</span></span>|<span data-ttu-id="8c137-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="8c137-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c137-119">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="8c137-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="8c137-120">Contient des informations de récurrence pour les tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="8c137-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8c137-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="8c137-121">Remarks</span></span>

<span data-ttu-id="8c137-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8c137-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8c137-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8c137-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8c137-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8c137-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8c137-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8c137-125">Schema name</span></span>  <br/> |<span data-ttu-id="8c137-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8c137-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="8c137-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8c137-127">Validation file</span></span>  <br/> |<span data-ttu-id="8c137-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8c137-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8c137-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8c137-129">Can be empty</span></span>  <br/> |<span data-ttu-id="8c137-130">False</span><span class="sxs-lookup"><span data-stu-id="8c137-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8c137-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8c137-131">See also</span></span>

- [<span data-ttu-id="8c137-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8c137-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

