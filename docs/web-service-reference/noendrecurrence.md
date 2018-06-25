---
title: NoEndRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NoEndRecurrence
api_type:
- schema
ms.assetid: ab2ebd9c-388e-45f1-abf9-56e293ef123b
description: L’élément NoEndRecurrence indique la date de début d’une périodicité d’élément qui n’a pas une date de fin définie.
ms.openlocfilehash: fc3eae170f5c07e31d7a80b45836efd07d74e543
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828537"
---
# <a name="noendrecurrence"></a><span data-ttu-id="dc164-103">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="dc164-103">NoEndRecurrence</span></span>

<span data-ttu-id="dc164-104">L’élément **NoEndRecurrence** indique la date de début d’une périodicité d’élément qui n’a pas une date de fin définie.</span><span class="sxs-lookup"><span data-stu-id="dc164-104">The **NoEndRecurrence** element describes the start date of an item recurrence pattern that does not have a defined end date.</span></span> 
  
```xml
<NoEndRecurrence>
   <StartDate/>
</NoEndRecurrence>
```

 <span data-ttu-id="dc164-105">**NoEndRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="dc164-105">**NoEndRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc164-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dc164-106">Attributes and elements</span></span>

<span data-ttu-id="dc164-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dc164-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc164-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="dc164-108">Attributes</span></span>

<span data-ttu-id="dc164-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dc164-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc164-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dc164-110">Child elements</span></span>

|<span data-ttu-id="dc164-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dc164-111">**Element**</span></span>|<span data-ttu-id="dc164-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="dc164-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc164-113">StartDate (périodicité)</span><span class="sxs-lookup"><span data-stu-id="dc164-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="dc164-114">Représente la date de début d’une tâche périodique ou d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="dc164-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc164-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dc164-115">Parent elements</span></span>

|<span data-ttu-id="dc164-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dc164-116">**Element**</span></span>|<span data-ttu-id="dc164-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="dc164-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc164-118">Périodicité (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="dc164-118">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="dc164-119">Contient la périodicité pour les éléments de calendrier et les demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="dc164-119">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="dc164-120">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="dc164-120">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="dc164-121">Contient des informations de périodicité pour les tâches répétitives.</span><span class="sxs-lookup"><span data-stu-id="dc164-121">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dc164-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="dc164-122">Remarks</span></span>

<span data-ttu-id="dc164-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="dc164-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc164-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dc164-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc164-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dc164-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dc164-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dc164-126">Schema name</span></span>  <br/> |<span data-ttu-id="dc164-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="dc164-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="dc164-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dc164-128">Validation file</span></span>  <br/> |<span data-ttu-id="dc164-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dc164-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dc164-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dc164-130">Can be empty</span></span>  <br/> |<span data-ttu-id="dc164-131">False</span><span class="sxs-lookup"><span data-stu-id="dc164-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc164-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dc164-132">See also</span></span>



- [<span data-ttu-id="dc164-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dc164-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

