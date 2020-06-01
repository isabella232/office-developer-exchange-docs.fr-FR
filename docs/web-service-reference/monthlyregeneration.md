---
title: MonthlyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MonthlyRegeneration
api_type:
- schema
ms.assetid: 9a52ca97-a663-41fe-b61a-61d8c53833ca
description: L’élément MonthlyRegeneration décrit la fréquence, en mois, de la régénération de la tâche.
ms.openlocfilehash: c941bc2606790646d2797df27c854996901c0bc6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462737"
---
# <a name="monthlyregeneration"></a><span data-ttu-id="7cbf7-103">MonthlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="7cbf7-103">MonthlyRegeneration</span></span>

<span data-ttu-id="7cbf7-104">L’élément **MonthlyRegeneration** décrit la fréquence, en mois, de la régénération de la tâche.</span><span class="sxs-lookup"><span data-stu-id="7cbf7-104">The **MonthlyRegeneration** element describes the frequency, in months, of which task is regenerated.</span></span> 
  
```xml
<MonthlyRegeneration>
   <Interval/>
</MonthlyRegeneration>
```

 <span data-ttu-id="7cbf7-105">**MonthlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="7cbf7-105">**MonthlyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7cbf7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7cbf7-106">Attributes and elements</span></span>

<span data-ttu-id="7cbf7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7cbf7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cbf7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7cbf7-108">Attributes</span></span>

<span data-ttu-id="7cbf7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7cbf7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7cbf7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7cbf7-110">Child elements</span></span>

|<span data-ttu-id="7cbf7-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7cbf7-111">**Element**</span></span>|<span data-ttu-id="7cbf7-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7cbf7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cbf7-113">Interval</span><span class="sxs-lookup"><span data-stu-id="7cbf7-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="7cbf7-114">Définit l’intervalle, en mois, entre deux éléments périodiques consécutifs.</span><span class="sxs-lookup"><span data-stu-id="7cbf7-114">Defines the interval, in months, between two consecutive recurring items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7cbf7-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7cbf7-115">Parent elements</span></span>

|<span data-ttu-id="7cbf7-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7cbf7-116">**Element**</span></span>|<span data-ttu-id="7cbf7-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="7cbf7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cbf7-118">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="7cbf7-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="7cbf7-119">Contient des informations de récurrence pour les tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="7cbf7-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7cbf7-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="7cbf7-120">Remarks</span></span>

<span data-ttu-id="7cbf7-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="7cbf7-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7cbf7-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7cbf7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cbf7-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7cbf7-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7cbf7-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7cbf7-124">Schema name</span></span>  <br/> |<span data-ttu-id="7cbf7-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7cbf7-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7cbf7-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7cbf7-126">Validation file</span></span>  <br/> |<span data-ttu-id="7cbf7-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7cbf7-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7cbf7-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7cbf7-128">Can be empty</span></span>  <br/> |<span data-ttu-id="7cbf7-129">False</span><span class="sxs-lookup"><span data-stu-id="7cbf7-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cbf7-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7cbf7-130">See also</span></span>



- [<span data-ttu-id="7cbf7-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7cbf7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

