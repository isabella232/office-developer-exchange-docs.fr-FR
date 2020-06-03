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
description: L’élément NoEndRecurrence décrit la date de début d’un critère de récurrence d’élément qui n’a pas de date de fin définie.
ms.openlocfilehash: 31a3bd6ae2d7ce94debbeebc4fd4f536447433a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466793"
---
# <a name="noendrecurrence"></a><span data-ttu-id="0dea1-103">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="0dea1-103">NoEndRecurrence</span></span>

<span data-ttu-id="0dea1-104">L’élément **NoEndRecurrence** décrit la date de début d’un critère de récurrence d’élément qui n’a pas de date de fin définie.</span><span class="sxs-lookup"><span data-stu-id="0dea1-104">The **NoEndRecurrence** element describes the start date of an item recurrence pattern that does not have a defined end date.</span></span> 
  
```xml
<NoEndRecurrence>
   <StartDate/>
</NoEndRecurrence>
```

 <span data-ttu-id="0dea1-105">**NoEndRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="0dea1-105">**NoEndRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0dea1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0dea1-106">Attributes and elements</span></span>

<span data-ttu-id="0dea1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0dea1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0dea1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0dea1-108">Attributes</span></span>

<span data-ttu-id="0dea1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0dea1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0dea1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0dea1-110">Child elements</span></span>

|<span data-ttu-id="0dea1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0dea1-111">**Element**</span></span>|<span data-ttu-id="0dea1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0dea1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0dea1-113">StartDate (périodicité)</span><span class="sxs-lookup"><span data-stu-id="0dea1-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="0dea1-114">Représente la date de début d’une tâche périodique ou d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="0dea1-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0dea1-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0dea1-115">Parent elements</span></span>

|<span data-ttu-id="0dea1-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0dea1-116">**Element**</span></span>|<span data-ttu-id="0dea1-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="0dea1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0dea1-118">Récurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="0dea1-118">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="0dea1-119">Contient la périodicité des éléments de calendrier et des demandes de réunion.</span><span class="sxs-lookup"><span data-stu-id="0dea1-119">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="0dea1-120">Périodicité (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="0dea1-120">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="0dea1-121">Contient des informations de récurrence pour les tâches périodiques.</span><span class="sxs-lookup"><span data-stu-id="0dea1-121">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0dea1-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="0dea1-122">Remarks</span></span>

<span data-ttu-id="0dea1-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0dea1-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0dea1-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0dea1-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0dea1-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0dea1-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0dea1-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0dea1-126">Schema name</span></span>  <br/> |<span data-ttu-id="0dea1-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0dea1-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="0dea1-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0dea1-128">Validation file</span></span>  <br/> |<span data-ttu-id="0dea1-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0dea1-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0dea1-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0dea1-130">Can be empty</span></span>  <br/> |<span data-ttu-id="0dea1-131">False</span><span class="sxs-lookup"><span data-stu-id="0dea1-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0dea1-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0dea1-132">See also</span></span>



- [<span data-ttu-id="0dea1-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0dea1-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

