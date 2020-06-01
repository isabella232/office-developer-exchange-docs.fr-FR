---
title: TimeZoneDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: L’élément TimeZoneDefinition spécifie les points et les transitions qui définissent un fuseau horaire.
ms.openlocfilehash: 58d34556686bfc77244b5829798eada51a1df843
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466065"
---
# <a name="timezonedefinition"></a><span data-ttu-id="bfb0b-103">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="bfb0b-103">TimeZoneDefinition</span></span>

<span data-ttu-id="bfb0b-104">L’élément **TimeZoneDefinition** spécifie les points et les transitions qui définissent un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bfb0b-104">The **TimeZoneDefinition** element specifies the periods and transitions that define a time zone.</span></span> 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 <span data-ttu-id="bfb0b-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="bfb0b-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bfb0b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bfb0b-106">Attributes and elements</span></span>

<span data-ttu-id="bfb0b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bfb0b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bfb0b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bfb0b-108">Attributes</span></span>

|<span data-ttu-id="bfb0b-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bfb0b-109">**Attribute**</span></span>|<span data-ttu-id="bfb0b-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="bfb0b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bfb0b-111">ID</span><span class="sxs-lookup"><span data-stu-id="bfb0b-111">Id</span></span>  <br/> |<span data-ttu-id="bfb0b-112">Représente l’identificateur unique du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bfb0b-112">Represents the unique identifier of the time zone.</span></span>  <br/> |
|<span data-ttu-id="bfb0b-113">Nom</span><span class="sxs-lookup"><span data-stu-id="bfb0b-113">Name</span></span>  <br/> |<span data-ttu-id="bfb0b-114">Représente le nom descriptif du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bfb0b-114">Represents the descriptive name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bfb0b-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bfb0b-115">Child elements</span></span>

|<span data-ttu-id="bfb0b-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bfb0b-116">**Element**</span></span>|<span data-ttu-id="bfb0b-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="bfb0b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfb0b-118">Periods</span><span class="sxs-lookup"><span data-stu-id="bfb0b-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="bfb0b-119">Représente un tableau d’éléments [period](period.md) qui définissent le décalage temporel à différentes étapes du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bfb0b-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="bfb0b-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="bfb0b-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="bfb0b-121">Représente un tableau d’éléments [TransitionsGroup](transitionsgroup.md) qui spécifient des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bfb0b-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="bfb0b-122">Transitions</span><span class="sxs-lookup"><span data-stu-id="bfb0b-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="bfb0b-123">Représente un tableau de transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bfb0b-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bfb0b-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bfb0b-124">Parent elements</span></span>

|<span data-ttu-id="bfb0b-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bfb0b-125">**Element**</span></span>|<span data-ttu-id="bfb0b-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="bfb0b-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfb0b-127">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="bfb0b-127">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="bfb0b-128">Représente un tableau de définitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="bfb0b-128">Represents an array of time zone definitions.</span></span>  <br/> |
|[<span data-ttu-id="bfb0b-129">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="bfb0b-129">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="bfb0b-130">Représente la définition de fuseau horaire par défaut qui doit être utilisée pour la portée des propriétés DateTime des objets créés, mis à jour et récupérés à l’aide des services Web Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="bfb0b-130">Represents the default time zone definition that is to be used for scoping the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bfb0b-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="bfb0b-131">Remarks</span></span>

<span data-ttu-id="bfb0b-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bfb0b-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bfb0b-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bfb0b-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bfb0b-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bfb0b-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bfb0b-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bfb0b-135">Schema Name</span></span>  <br/> |<span data-ttu-id="bfb0b-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bfb0b-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="bfb0b-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bfb0b-137">Validation File</span></span>  <br/> |<span data-ttu-id="bfb0b-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bfb0b-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bfb0b-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bfb0b-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="bfb0b-140">False</span><span class="sxs-lookup"><span data-stu-id="bfb0b-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bfb0b-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bfb0b-141">See also</span></span>



- [<span data-ttu-id="bfb0b-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bfb0b-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

