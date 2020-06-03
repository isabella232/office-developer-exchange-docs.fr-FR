---
title: CalendarItemType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarItemType
api_type:
- schema
ms.assetid: 1feb0788-adf7-4a7c-830c-005214ad930f
description: L’élément CalendarItemType représente le type d’un élément de calendrier.
ms.openlocfilehash: 05e93b6db3ae574c03f6e43c5ebec2288edec3e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527193"
---
# <a name="calendaritemtype"></a><span data-ttu-id="d3a58-103">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="d3a58-103">CalendarItemType</span></span>

<span data-ttu-id="d3a58-104">L’élément **CalendarItemType** représente le type d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="d3a58-104">The **CalendarItemType** element represents the type of a calendar item.</span></span> 
  
```xml
<CalendarItemType/>
```

 <span data-ttu-id="d3a58-105">**CalendarItemTypeType**</span><span class="sxs-lookup"><span data-stu-id="d3a58-105">**CalendarItemTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3a58-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d3a58-106">Attributes and elements</span></span>

<span data-ttu-id="d3a58-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d3a58-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3a58-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d3a58-108">Attributes</span></span>

<span data-ttu-id="d3a58-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d3a58-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3a58-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d3a58-110">Child elements</span></span>

<span data-ttu-id="d3a58-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d3a58-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d3a58-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d3a58-112">Parent elements</span></span>

|<span data-ttu-id="d3a58-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d3a58-113">**Element**</span></span>|<span data-ttu-id="d3a58-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d3a58-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3a58-115">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="d3a58-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d3a58-116">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3a58-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d3a58-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d3a58-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d3a58-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3a58-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3a58-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="d3a58-119">Text value</span></span>

<span data-ttu-id="d3a58-120">Une valeur de texte est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="d3a58-120">A text value is required if this element is used.</span></span> <span data-ttu-id="d3a58-121">Les valeurs possibles pour cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="d3a58-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="d3a58-122">**Unique** L’élément n’est pas associé à un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="d3a58-122">**Single** The item is not associated with a recurring calendar item.</span></span> 
    
- <span data-ttu-id="d3a58-123">**Occurrence** L’élément est une occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="d3a58-123">**Occurrence** The item is an occurrence of a recurring calendar item.</span></span> 
    
- <span data-ttu-id="d3a58-124">**Exception** L’élément est une exception à un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="d3a58-124">**Exception** The item is an exception to a recurring calendar item.</span></span> 
    
- <span data-ttu-id="d3a58-125">**RecurringMaster** L’élément est une forme de base pour un ensemble d’éléments de calendrier périodiques.</span><span class="sxs-lookup"><span data-stu-id="d3a58-125">**RecurringMaster** The item is master for a set of recurring calendar items.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="d3a58-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="d3a58-126">Remarks</span></span>

<span data-ttu-id="d3a58-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d3a58-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3a58-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d3a58-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3a58-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d3a58-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3a58-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d3a58-130">Schema name</span></span>  <br/> |<span data-ttu-id="d3a58-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d3a58-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3a58-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d3a58-132">Validation file</span></span>  <br/> |<span data-ttu-id="d3a58-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d3a58-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3a58-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d3a58-134">Can be empty</span></span>  <br/> |<span data-ttu-id="d3a58-135">False</span><span class="sxs-lookup"><span data-stu-id="d3a58-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3a58-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d3a58-136">See also</span></span>



- [<span data-ttu-id="d3a58-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d3a58-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

