---
title: StartDate (périodicité)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartDate
api_type:
- schema
ms.assetid: bd65ac06-b3ac-4c9b-9568-3e4dc94378e7
description: L’élément StartDate représente la date de début d’une tâche périodique ou d’un élément de calendrier.
ms.openlocfilehash: 6a38e63bbcf010ab6dca8f66440a2b0a559cf88d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829551"
---
# <a name="startdate-recurrence"></a><span data-ttu-id="05a86-103">StartDate (périodicité)</span><span class="sxs-lookup"><span data-stu-id="05a86-103">StartDate (Recurrence)</span></span>

<span data-ttu-id="05a86-104">L’élément **StartDate** représente la date de début d’une tâche périodique ou d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="05a86-104">The **StartDate** element represents the start date of a recurring task or calendar item.</span></span> 
  
```xml
<StartDate/>
```

<span data-ttu-id="05a86-105">**Date**</span><span class="sxs-lookup"><span data-stu-id="05a86-105">**Date**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="05a86-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="05a86-106">Attributes and elements</span></span>

<span data-ttu-id="05a86-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="05a86-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05a86-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="05a86-108">Attributes</span></span>

<span data-ttu-id="05a86-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05a86-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05a86-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="05a86-110">Child elements</span></span>

<span data-ttu-id="05a86-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05a86-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05a86-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="05a86-112">Parent elements</span></span>

|<span data-ttu-id="05a86-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="05a86-113">**Element**</span></span>|<span data-ttu-id="05a86-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="05a86-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05a86-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="05a86-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="05a86-116">Décrit la date de début et date de fin de périodicité d’un élément.</span><span class="sxs-lookup"><span data-stu-id="05a86-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="05a86-117">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="05a86-117">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="05a86-118">Indique la date de début d’une périodicité d’élément qui n’a pas une date de fin définie.</span><span class="sxs-lookup"><span data-stu-id="05a86-118">Describes the start date of an item recurrence pattern that does not have a defined end date.</span></span>  <br/> |
|[<span data-ttu-id="05a86-119">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="05a86-119">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="05a86-120">Décrit la date de début et le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="05a86-120">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05a86-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="05a86-121">Text value</span></span>

<span data-ttu-id="05a86-122">Une valeur de texte qui représente une date est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="05a86-122">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="05a86-123">La valeur ne peut pas être inférieure à avr 1, 1601 00:00:00.</span><span class="sxs-lookup"><span data-stu-id="05a86-123">The value cannot be less than Apr, 1, 1601 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="05a86-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="05a86-124">Remarks</span></span>

<span data-ttu-id="05a86-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="05a86-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05a86-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="05a86-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05a86-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="05a86-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05a86-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="05a86-128">Schema name</span></span>  <br/> |<span data-ttu-id="05a86-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="05a86-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="05a86-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="05a86-130">Validation file</span></span>  <br/> |<span data-ttu-id="05a86-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05a86-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05a86-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="05a86-132">Can be empty</span></span>  <br/> |<span data-ttu-id="05a86-133">False</span><span class="sxs-lookup"><span data-stu-id="05a86-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05a86-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05a86-134">See also</span></span>

- [<span data-ttu-id="05a86-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="05a86-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

