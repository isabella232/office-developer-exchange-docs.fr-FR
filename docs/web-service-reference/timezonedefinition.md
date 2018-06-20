---
title: Définition de fuseau horaire
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
description: L’élément de la définition de fuseau horaire spécifie les périodes et les transitions qui définissent un fuseau horaire.
ms.openlocfilehash: ffd5ed0c862af794e4aff2387f508849b1d5fd5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838736"
---
# <a name="timezonedefinition"></a><span data-ttu-id="08bb5-103">Définition de fuseau horaire</span><span class="sxs-lookup"><span data-stu-id="08bb5-103">TimeZoneDefinition</span></span>

<span data-ttu-id="08bb5-104">L’élément de la **définition de fuseau horaire** spécifie les périodes et les transitions qui définissent un fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="08bb5-104">The **TimeZoneDefinition** element specifies the periods and transitions that define a time zone.</span></span> 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 <span data-ttu-id="08bb5-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="08bb5-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08bb5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="08bb5-106">Attributes and elements</span></span>

<span data-ttu-id="08bb5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="08bb5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08bb5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="08bb5-108">Attributes</span></span>

|<span data-ttu-id="08bb5-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="08bb5-109">**Attribute**</span></span>|<span data-ttu-id="08bb5-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="08bb5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="08bb5-111">ID</span><span class="sxs-lookup"><span data-stu-id="08bb5-111">Id</span></span>  <br/> |<span data-ttu-id="08bb5-112">Identificateur unique du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="08bb5-112">Represents the unique identifier of the time zone.</span></span>  <br/> |
|<span data-ttu-id="08bb5-113">Nom</span><span class="sxs-lookup"><span data-stu-id="08bb5-113">Name</span></span>  <br/> |<span data-ttu-id="08bb5-114">Représente le nom descriptif du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="08bb5-114">Represents the descriptive name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="08bb5-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="08bb5-115">Child elements</span></span>

|<span data-ttu-id="08bb5-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="08bb5-116">**Element**</span></span>|<span data-ttu-id="08bb5-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="08bb5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08bb5-118">Périodes</span><span class="sxs-lookup"><span data-stu-id="08bb5-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="08bb5-119">Représente un tableau d’éléments de [période](period.md) qui définissent le décalage de temps à différents stades du fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="08bb5-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="08bb5-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="08bb5-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="08bb5-121">Représente un tableau d’éléments [TransitionsGroup](transitionsgroup.md) qui spécifient les transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="08bb5-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="08bb5-122">Transitions</span><span class="sxs-lookup"><span data-stu-id="08bb5-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="08bb5-123">Représente un tableau des transitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="08bb5-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08bb5-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="08bb5-124">Parent elements</span></span>

|<span data-ttu-id="08bb5-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="08bb5-125">**Element**</span></span>|<span data-ttu-id="08bb5-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="08bb5-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08bb5-127">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="08bb5-127">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="08bb5-128">Représente un tableau des définitions de fuseau horaire.</span><span class="sxs-lookup"><span data-stu-id="08bb5-128">Represents an array of time zone definitions.</span></span>  <br/> |
|[<span data-ttu-id="08bb5-129">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="08bb5-129">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="08bb5-130">Représente la définition de fuseau horaire par défaut qui doit être utilisé pour les propriétés DateTime des objets qui sont créés, mis à jour et récupérés à l’aide d’Exchange Web Services (EWS) de portée.</span><span class="sxs-lookup"><span data-stu-id="08bb5-130">Represents the default time zone definition that is to be used for scoping the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="08bb5-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="08bb5-131">Remarks</span></span>

<span data-ttu-id="08bb5-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="08bb5-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08bb5-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="08bb5-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08bb5-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="08bb5-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08bb5-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="08bb5-135">Schema Name</span></span>  <br/> |<span data-ttu-id="08bb5-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="08bb5-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="08bb5-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="08bb5-137">Validation File</span></span>  <br/> |<span data-ttu-id="08bb5-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="08bb5-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08bb5-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="08bb5-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="08bb5-140">False</span><span class="sxs-lookup"><span data-stu-id="08bb5-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08bb5-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="08bb5-141">See also</span></span>



- [<span data-ttu-id="08bb5-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="08bb5-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

