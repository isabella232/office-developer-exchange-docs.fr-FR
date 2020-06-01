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
ms.openlocfilehash: 22ee9018df1e89a3783c4dfb56aaf065b2c8ea6c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466296"
---
# <a name="firstoccurrence"></a><span data-ttu-id="2fc14-103">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="2fc14-103">FirstOccurrence</span></span>

<span data-ttu-id="2fc14-104">L’élément **FirstOccurrence** représente la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="2fc14-104">The **FirstOccurrence** element represents the first occurrence of a recurring calendar item.</span></span> 
  
```xml
<FirstOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</FirstOccurrence>
```

 <span data-ttu-id="2fc14-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="2fc14-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2fc14-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2fc14-106">Attributes and elements</span></span>

<span data-ttu-id="2fc14-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2fc14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2fc14-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2fc14-108">Attributes</span></span>

<span data-ttu-id="2fc14-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2fc14-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2fc14-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2fc14-110">Child elements</span></span>

|<span data-ttu-id="2fc14-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2fc14-111">**Element**</span></span>|<span data-ttu-id="2fc14-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2fc14-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fc14-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="2fc14-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="2fc14-114">Contient l’identificateur unique et la clé de modification de la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="2fc14-114">Contains the unique identifier and change key of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2fc14-115">Démarrage</span><span class="sxs-lookup"><span data-stu-id="2fc14-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="2fc14-116">Représente l’heure de début de la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="2fc14-116">Represents the start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2fc14-117">Fin</span><span class="sxs-lookup"><span data-stu-id="2fc14-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2fc14-118">Représente l’heure de fin de la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="2fc14-118">Represents the end time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2fc14-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="2fc14-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="2fc14-120">Représente l’heure de début d’origine de la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="2fc14-120">Represents the original start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2fc14-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2fc14-121">Parent elements</span></span>

|<span data-ttu-id="2fc14-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2fc14-122">**Element**</span></span>|<span data-ttu-id="2fc14-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="2fc14-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fc14-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2fc14-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2fc14-125">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="2fc14-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2fc14-126">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="2fc14-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2fc14-127">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="2fc14-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2fc14-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="2fc14-128">Remarks</span></span>

<span data-ttu-id="2fc14-129">Cet élément est valide si [CalendarItemType](calendaritemtype.md) a la valeur RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="2fc14-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="2fc14-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2fc14-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2fc14-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2fc14-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2fc14-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2fc14-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2fc14-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2fc14-133">Schema name</span></span>  <br/> |<span data-ttu-id="2fc14-134">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2fc14-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="2fc14-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2fc14-135">Validation file</span></span>  <br/> |<span data-ttu-id="2fc14-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2fc14-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2fc14-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2fc14-137">Can be empty</span></span>  <br/> |<span data-ttu-id="2fc14-138">False</span><span class="sxs-lookup"><span data-stu-id="2fc14-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2fc14-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2fc14-139">See also</span></span>



- [<span data-ttu-id="2fc14-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2fc14-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="2fc14-141">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="2fc14-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

