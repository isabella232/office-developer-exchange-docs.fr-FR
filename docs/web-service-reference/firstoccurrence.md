---
title: FirstOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FirstOccurrence
api_type:
- schema
ms.assetid: d6748860-ce0d-4d2e-b7e4-9ed834f1e45a
description: L’élément FirstOccurrence représente la première occurrence d’un élément de calendrier périodique.
ms.openlocfilehash: e5244e74bdd5a4b8e22c6e63811db53b46fa353a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756432"
---
# <a name="firstoccurrence"></a><span data-ttu-id="75f01-103">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="75f01-103">FirstOccurrence</span></span>

<span data-ttu-id="75f01-104">L’élément **FirstOccurrence** représente la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="75f01-104">The **FirstOccurrence** element represents the first occurrence of a recurring calendar item.</span></span> 
  
```xml
<FirstOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</FirstOccurrence>
```

 <span data-ttu-id="75f01-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="75f01-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75f01-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="75f01-106">Attributes and elements</span></span>

<span data-ttu-id="75f01-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="75f01-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75f01-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="75f01-108">Attributes</span></span>

<span data-ttu-id="75f01-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="75f01-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75f01-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="75f01-110">Child elements</span></span>

|<span data-ttu-id="75f01-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="75f01-111">**Element**</span></span>|<span data-ttu-id="75f01-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="75f01-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75f01-113">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="75f01-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="75f01-114">Contient la clé unique identificateur et modification de la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="75f01-114">Contains the unique identifier and change key of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="75f01-115">Début</span><span class="sxs-lookup"><span data-stu-id="75f01-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="75f01-116">Représente l’heure de début de la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="75f01-116">Represents the start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="75f01-117">Fin</span><span class="sxs-lookup"><span data-stu-id="75f01-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="75f01-118">Représente l’heure de fin de la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="75f01-118">Represents the end time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="75f01-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="75f01-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="75f01-120">Représente l’heure de début d’origine de la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="75f01-120">Represents the original start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="75f01-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="75f01-121">Parent elements</span></span>

|<span data-ttu-id="75f01-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="75f01-122">**Element**</span></span>|<span data-ttu-id="75f01-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="75f01-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75f01-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="75f01-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="75f01-125">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="75f01-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="75f01-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="75f01-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="75f01-127">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="75f01-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="75f01-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="75f01-128">Remarks</span></span>

<span data-ttu-id="75f01-129">Cet élément n’est valide que si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="75f01-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="75f01-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="75f01-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75f01-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="75f01-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75f01-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="75f01-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="75f01-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="75f01-133">Schema name</span></span>  <br/> |<span data-ttu-id="75f01-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="75f01-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="75f01-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="75f01-135">Validation file</span></span>  <br/> |<span data-ttu-id="75f01-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="75f01-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="75f01-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="75f01-137">Can be empty</span></span>  <br/> |<span data-ttu-id="75f01-138">False</span><span class="sxs-lookup"><span data-stu-id="75f01-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75f01-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="75f01-139">See also</span></span>



- [<span data-ttu-id="75f01-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="75f01-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="75f01-141">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="75f01-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

