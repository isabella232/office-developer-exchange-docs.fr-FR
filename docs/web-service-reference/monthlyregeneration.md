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
description: L’élément MonthlyRegeneration décrit la fréquence, en mois, dont la tâche est régénérée.
ms.openlocfilehash: 3de8ab5a6a2134ad5c596bf2bcb073d881c89746
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828488"
---
# <a name="monthlyregeneration"></a><span data-ttu-id="4b0a2-103">MonthlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="4b0a2-103">MonthlyRegeneration</span></span>

<span data-ttu-id="4b0a2-104">L’élément **MonthlyRegeneration** décrit la fréquence, en mois, dont la tâche est régénérée.</span><span class="sxs-lookup"><span data-stu-id="4b0a2-104">The **MonthlyRegeneration** element describes the frequency, in months, of which task is regenerated.</span></span> 
  
```xml
<MonthlyRegeneration>
   <Interval/>
</MonthlyRegeneration>
```

 <span data-ttu-id="4b0a2-105">**MonthlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="4b0a2-105">**MonthlyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b0a2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4b0a2-106">Attributes and elements</span></span>

<span data-ttu-id="4b0a2-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4b0a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b0a2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4b0a2-108">Attributes</span></span>

<span data-ttu-id="4b0a2-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4b0a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b0a2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4b0a2-110">Child elements</span></span>

|<span data-ttu-id="4b0a2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b0a2-111">**Element**</span></span>|<span data-ttu-id="4b0a2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b0a2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b0a2-113">Intervalle</span><span class="sxs-lookup"><span data-stu-id="4b0a2-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="4b0a2-114">Définit l’intervalle, en mois, entre les deux éléments périodiques consécutives.</span><span class="sxs-lookup"><span data-stu-id="4b0a2-114">Defines the interval, in months, between two consecutive recurring items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b0a2-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4b0a2-115">Parent elements</span></span>

|<span data-ttu-id="4b0a2-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b0a2-116">**Element**</span></span>|<span data-ttu-id="4b0a2-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b0a2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b0a2-118">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="4b0a2-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="4b0a2-119">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="4b0a2-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4b0a2-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="4b0a2-120">Remarks</span></span>

<span data-ttu-id="4b0a2-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4b0a2-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b0a2-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4b0a2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b0a2-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4b0a2-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4b0a2-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4b0a2-124">Schema name</span></span>  <br/> |<span data-ttu-id="4b0a2-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4b0a2-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="4b0a2-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4b0a2-126">Validation file</span></span>  <br/> |<span data-ttu-id="4b0a2-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4b0a2-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4b0a2-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4b0a2-128">Can be empty</span></span>  <br/> |<span data-ttu-id="4b0a2-129">False</span><span class="sxs-lookup"><span data-stu-id="4b0a2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b0a2-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4b0a2-130">See also</span></span>



- [<span data-ttu-id="4b0a2-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4b0a2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

