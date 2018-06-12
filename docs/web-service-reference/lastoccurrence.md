---
title: LastOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LastOccurrence
api_type:
- schema
ms.assetid: c9ef0fcb-4265-4e60-9986-fff0f211d00b
description: L’élément LastOccurrence représente la dernière occurrence d’un élément de calendrier périodique.
ms.openlocfilehash: 2c8fdfc0005e86c9dda84a48ae1d3692b5134ca8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828209"
---
# <a name="lastoccurrence"></a><span data-ttu-id="ca880-103">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="ca880-103">LastOccurrence</span></span>

<span data-ttu-id="ca880-104">L’élément **LastOccurrence** représente la dernière occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="ca880-104">The **LastOccurrence** element represents the last occurrence of a recurring calendar item.</span></span> 
  
```xml
<LastOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</LastOccurrence>
```

 <span data-ttu-id="ca880-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="ca880-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca880-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ca880-106">Attributes and elements</span></span>

<span data-ttu-id="ca880-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ca880-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca880-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ca880-108">Attributes</span></span>

<span data-ttu-id="ca880-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ca880-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca880-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ca880-110">Child elements</span></span>

|<span data-ttu-id="ca880-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ca880-111">**Element**</span></span>|<span data-ttu-id="ca880-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ca880-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca880-113">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="ca880-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="ca880-114">Contient la clé unique identificateur et modification de la dernière occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="ca880-114">Contains the unique identifier and change key of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ca880-115">Début</span><span class="sxs-lookup"><span data-stu-id="ca880-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="ca880-116">Représente l’heure de début de la dernière occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="ca880-116">Represents the start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ca880-117">Fin</span><span class="sxs-lookup"><span data-stu-id="ca880-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ca880-118">Représente l’heure de fin de la dernière occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="ca880-118">Represents the end time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ca880-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="ca880-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="ca880-120">Représente l’heure de début d’origine de la dernière occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="ca880-120">Represents the original start time of the last occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ca880-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ca880-121">Parent elements</span></span>

|<span data-ttu-id="ca880-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ca880-122">**Element**</span></span>|<span data-ttu-id="ca880-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="ca880-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca880-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ca880-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ca880-125">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca880-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ca880-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ca880-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ca880-127">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca880-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ca880-128">Note</span><span class="sxs-lookup"><span data-stu-id="ca880-128">Remarks</span></span>

<span data-ttu-id="ca880-129">Cet élément n’est valide que si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="ca880-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="ca880-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ca880-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca880-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ca880-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca880-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ca880-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ca880-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ca880-133">Schema name</span></span>  <br/> |<span data-ttu-id="ca880-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ca880-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="ca880-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ca880-135">Validation file</span></span>  <br/> |<span data-ttu-id="ca880-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ca880-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ca880-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ca880-137">Can be empty</span></span>  <br/> |<span data-ttu-id="ca880-138">False</span><span class="sxs-lookup"><span data-stu-id="ca880-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca880-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ca880-139">See also</span></span>



- [<span data-ttu-id="ca880-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ca880-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="ca880-141">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ca880-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

