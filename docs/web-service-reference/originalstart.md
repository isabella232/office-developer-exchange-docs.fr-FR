---
title: OriginalStart
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OriginalStart
api_type:
- schema
ms.assetid: 4599dd34-15ee-4d57-b886-732081b50784
description: L’élément OriginalStart représente l’heure de début d’origine d’un élément de calendrier.
ms.openlocfilehash: 5346a65c432b8e96cb95e412e3e88fbc40ce36e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462366"
---
# <a name="originalstart"></a><span data-ttu-id="05109-103">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="05109-103">OriginalStart</span></span>

<span data-ttu-id="05109-104">L’élément **OriginalStart** représente l’heure de début d’origine d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="05109-104">The **OriginalStart** element represents the original start time of a calendar item.</span></span> 
  
```xml
<OriginalStart/>
```

 <span data-ttu-id="05109-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="05109-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05109-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="05109-106">Attributes and elements</span></span>

<span data-ttu-id="05109-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="05109-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05109-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="05109-108">Attributes</span></span>

<span data-ttu-id="05109-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="05109-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05109-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="05109-110">Child elements</span></span>

<span data-ttu-id="05109-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05109-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05109-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="05109-112">Parent elements</span></span>

|<span data-ttu-id="05109-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="05109-113">**Element**</span></span>|<span data-ttu-id="05109-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="05109-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05109-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="05109-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="05109-116">Représente un élément de calendrier dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="05109-116">Represents a calendar item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="05109-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="05109-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="05109-118">Représente la première occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="05109-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="05109-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="05109-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="05109-120">Représente la dernière occurrence d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="05109-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="05109-121">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="05109-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="05109-122">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="05109-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="05109-123">Réunions</span><span class="sxs-lookup"><span data-stu-id="05109-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="05109-124">Représente une occurrence modifiée unique d’un élément de calendrier périodique.</span><span class="sxs-lookup"><span data-stu-id="05109-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05109-125">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="05109-125">Text value</span></span>

<span data-ttu-id="05109-126">Une valeur de texte qui représente une date et une heure est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="05109-126">A text value that represents a date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="05109-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="05109-127">Remarks</span></span>

<span data-ttu-id="05109-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="05109-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05109-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="05109-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05109-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="05109-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05109-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="05109-131">Schema Name</span></span>  <br/> |<span data-ttu-id="05109-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="05109-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="05109-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="05109-133">Validation File</span></span>  <br/> |<span data-ttu-id="05109-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05109-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05109-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="05109-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="05109-136">False</span><span class="sxs-lookup"><span data-stu-id="05109-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05109-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05109-137">See also</span></span>



- [<span data-ttu-id="05109-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="05109-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

