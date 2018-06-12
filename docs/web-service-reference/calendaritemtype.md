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
ms.openlocfilehash: 3fe95c86ea24e6dfeb4740ead5e787bd63b5190d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755473"
---
# <a name="calendaritemtype"></a><span data-ttu-id="43f30-103">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="43f30-103">CalendarItemType</span></span>

<span data-ttu-id="43f30-104">L’élément **CalendarItemType** représente le type d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="43f30-104">The **CalendarItemType** element represents the type of a calendar item.</span></span> 
  
```xml
<CalendarItemType/>
```

 <span data-ttu-id="43f30-105">**CalendarItemTypeType**</span><span class="sxs-lookup"><span data-stu-id="43f30-105">**CalendarItemTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43f30-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="43f30-106">Attributes and elements</span></span>

<span data-ttu-id="43f30-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="43f30-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43f30-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="43f30-108">Attributes</span></span>

<span data-ttu-id="43f30-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="43f30-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43f30-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="43f30-110">Child elements</span></span>

<span data-ttu-id="43f30-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="43f30-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="43f30-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="43f30-112">Parent elements</span></span>

|<span data-ttu-id="43f30-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="43f30-113">**Element**</span></span>|<span data-ttu-id="43f30-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="43f30-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43f30-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="43f30-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="43f30-116">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="43f30-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="43f30-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="43f30-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="43f30-118">Représente un élément de calendrier Exchange.</span><span class="sxs-lookup"><span data-stu-id="43f30-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="43f30-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="43f30-119">Text value</span></span>

<span data-ttu-id="43f30-120">Une valeur de texte est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="43f30-120">A text value is required if this element is used.</span></span> <span data-ttu-id="43f30-121">Les valeurs possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="43f30-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="43f30-122">**Unique** L’élément n’est pas associé à un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="43f30-122">**Single** The item is not associated with a recurring calendar item.</span></span> 
    
- <span data-ttu-id="43f30-123">**Occurrence** L’élément est une occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="43f30-123">**Occurrence** The item is an occurrence of a recurring calendar item.</span></span> 
    
- <span data-ttu-id="43f30-124">**Exception** L’élément est une exception à un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="43f30-124">**Exception** The item is an exception to a recurring calendar item.</span></span> 
    
- <span data-ttu-id="43f30-125">**RecurringMaster** L’élément est maître pour un ensemble de rendez-vous périodiques.</span><span class="sxs-lookup"><span data-stu-id="43f30-125">**RecurringMaster** The item is master for a set of recurring calendar items.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="43f30-126">Note</span><span class="sxs-lookup"><span data-stu-id="43f30-126">Remarks</span></span>

<span data-ttu-id="43f30-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="43f30-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43f30-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="43f30-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43f30-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="43f30-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="43f30-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="43f30-130">Schema name</span></span>  <br/> |<span data-ttu-id="43f30-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="43f30-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="43f30-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="43f30-132">Validation file</span></span>  <br/> |<span data-ttu-id="43f30-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="43f30-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="43f30-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="43f30-134">Can be empty</span></span>  <br/> |<span data-ttu-id="43f30-135">False</span><span class="sxs-lookup"><span data-stu-id="43f30-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="43f30-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="43f30-136">See also</span></span>



- [<span data-ttu-id="43f30-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="43f30-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

