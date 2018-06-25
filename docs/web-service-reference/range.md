---
title: Plage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: L’élément de plage Spécifie une plage d’occurrences d’élément de calendrier pour un élément de calendrier périodique.
ms.openlocfilehash: 0264c541604808b46a50e292b8ff75f205796295
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828946"
---
# <a name="range"></a><span data-ttu-id="7f833-103">Plage</span><span class="sxs-lookup"><span data-stu-id="7f833-103">Range</span></span>

<span data-ttu-id="7f833-104">L’élément de **plage** spécifie une plage d’occurrences d’élément de calendrier pour un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="7f833-104">The **Range** element specifies a range of calendar item occurrences for a repeating calendar item.</span></span> 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 <span data-ttu-id="7f833-105">**OccurrencesRangeType**</span><span class="sxs-lookup"><span data-stu-id="7f833-105">**OccurrencesRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f833-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7f833-106">Attributes and elements</span></span>

<span data-ttu-id="7f833-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7f833-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f833-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7f833-108">Attributes</span></span>

|<span data-ttu-id="7f833-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="7f833-109">**Attribute**</span></span>|<span data-ttu-id="7f833-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="7f833-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7f833-111">**Début**</span><span class="sxs-lookup"><span data-stu-id="7f833-111">**Start**</span></span> <br/> |<span data-ttu-id="7f833-112">La valeur de texte de l’attribut **Démarrer** est la date de début de la plage d’éléments périodiques.</span><span class="sxs-lookup"><span data-stu-id="7f833-112">The text value of the **Start** attribute is the start date of the recurring item range.</span></span> <span data-ttu-id="7f833-113">Il s’agit d’une valeur **dateTime** .</span><span class="sxs-lookup"><span data-stu-id="7f833-113">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="7f833-114">**End**</span><span class="sxs-lookup"><span data-stu-id="7f833-114">**End**</span></span> <br/> |<span data-ttu-id="7f833-115">La valeur de texte de l’attribut de **fin** est la date de fin de la plage d’éléments périodiques.</span><span class="sxs-lookup"><span data-stu-id="7f833-115">The text value of the **End** attribute is the end date of the recurring item range.</span></span> <span data-ttu-id="7f833-116">Il s’agit d’une valeur **dateTime** .</span><span class="sxs-lookup"><span data-stu-id="7f833-116">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="7f833-117">**Count**</span><span class="sxs-lookup"><span data-stu-id="7f833-117">**Count**</span></span> <br/> |<span data-ttu-id="7f833-118">La valeur de texte de l’attribut de **nombre** est le nombre d’occurrences de l’élément périodique.</span><span class="sxs-lookup"><span data-stu-id="7f833-118">The text value of the **Count** attribute is the number of occurrences of the recurring item.</span></span> <span data-ttu-id="7f833-119">Il s’agit d’une valeur **entière** .</span><span class="sxs-lookup"><span data-stu-id="7f833-119">This is an **integer** value.</span></span>  <br/> |
|<span data-ttu-id="7f833-120">**CompareOriginalStartTime**</span><span class="sxs-lookup"><span data-stu-id="7f833-120">**CompareOriginalStartTime**</span></span> <br/> |<span data-ttu-id="7f833-121">La valeur de texte de **la valeur true** pour l’attribut **CompareOriginalStartTime** indique que le client doit comparer l’heure de début d’origine avec la nouvelle heure de début.</span><span class="sxs-lookup"><span data-stu-id="7f833-121">The text value of **true** for the **CompareOriginalStartTime** attribute indicates that the client should compare the original start time with the new start time.</span></span> <span data-ttu-id="7f833-122">La valeur **false** indique que le client n’a pas besoin comparer l’heure de début d’origine avec la nouvelle heure de début.</span><span class="sxs-lookup"><span data-stu-id="7f833-122">A value of **false** indicates that the client does not need to compare the original start time with the new start time.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7f833-123">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7f833-123">Child elements</span></span>

<span data-ttu-id="7f833-124">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7f833-124">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7f833-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7f833-125">Parent elements</span></span>

[<span data-ttu-id="7f833-126">Plages</span><span class="sxs-lookup"><span data-stu-id="7f833-126">Ranges</span></span>](ranges.md)
  
## <a name="remarks"></a><span data-ttu-id="7f833-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="7f833-127">Remarks</span></span>

<span data-ttu-id="7f833-128">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7f833-128">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7f833-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7f833-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f833-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7f833-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f833-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7f833-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7f833-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7f833-132">Schema name</span></span>  <br/> |<span data-ttu-id="7f833-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="7f833-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="7f833-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7f833-134">Validation file</span></span>  <br/> |<span data-ttu-id="7f833-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7f833-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7f833-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7f833-136">Can be empty</span></span>  <br/> ||
   

