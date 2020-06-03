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
description: L’élément StartDate représente la date de début d’une tâche ou d’un élément de calendrier périodique.
ms.openlocfilehash: 4514f126b1de31c64a2650b9e7cb6b7412a726c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457206"
---
# <a name="startdate-recurrence"></a><span data-ttu-id="90a67-103">StartDate (périodicité)</span><span class="sxs-lookup"><span data-stu-id="90a67-103">StartDate (Recurrence)</span></span>

<span data-ttu-id="90a67-104">L’élément **StartDate** représente la date de début d’une tâche ou d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="90a67-104">The **StartDate** element represents the start date of a recurring task or calendar item.</span></span> 
  
```xml
<StartDate/>
```

<span data-ttu-id="90a67-105">**Date**</span><span class="sxs-lookup"><span data-stu-id="90a67-105">**Date**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="90a67-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="90a67-106">Attributes and elements</span></span>

<span data-ttu-id="90a67-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="90a67-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90a67-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="90a67-108">Attributes</span></span>

<span data-ttu-id="90a67-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="90a67-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90a67-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="90a67-110">Child elements</span></span>

<span data-ttu-id="90a67-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="90a67-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="90a67-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="90a67-112">Parent elements</span></span>

|<span data-ttu-id="90a67-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="90a67-113">**Element**</span></span>|<span data-ttu-id="90a67-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="90a67-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90a67-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="90a67-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="90a67-116">Décrit la date de début et la date de fin d’une périodicité d’élément.</span><span class="sxs-lookup"><span data-stu-id="90a67-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="90a67-117">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="90a67-117">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="90a67-118">Décrit la date de début d’un critère de périodicité d’élément qui n’a pas de date de fin définie.</span><span class="sxs-lookup"><span data-stu-id="90a67-118">Describes the start date of an item recurrence pattern that does not have a defined end date.</span></span>  <br/> |
|[<span data-ttu-id="90a67-119">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="90a67-119">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="90a67-120">Décrit la date de début et le nombre d’occurrences d’un élément périodique.</span><span class="sxs-lookup"><span data-stu-id="90a67-120">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="90a67-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="90a67-121">Text value</span></span>

<span data-ttu-id="90a67-122">Une valeur de texte qui représente une date est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="90a67-122">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="90a67-123">La valeur ne peut pas être inférieure à la valeur Apr, 1, 1601 00:00:00.</span><span class="sxs-lookup"><span data-stu-id="90a67-123">The value cannot be less than Apr, 1, 1601 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="90a67-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="90a67-124">Remarks</span></span>

<span data-ttu-id="90a67-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="90a67-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90a67-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="90a67-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90a67-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="90a67-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90a67-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="90a67-128">Schema name</span></span>  <br/> |<span data-ttu-id="90a67-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="90a67-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="90a67-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="90a67-130">Validation file</span></span>  <br/> |<span data-ttu-id="90a67-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="90a67-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90a67-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="90a67-132">Can be empty</span></span>  <br/> |<span data-ttu-id="90a67-133">False</span><span class="sxs-lookup"><span data-stu-id="90a67-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90a67-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="90a67-134">See also</span></span>

- [<span data-ttu-id="90a67-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="90a67-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

