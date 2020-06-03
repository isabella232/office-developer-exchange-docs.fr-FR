---
title: DeletedOccurrenceStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a9c01c64-e76c-4adc-8b04-88af97bd0cc8
description: Le DeletedOccurrenceStateDefinition spécifie l’état d’une occurrence supprimée d’un élément de calendrier.
ms.openlocfilehash: ff8ad1d9c35d7bab3f6fe2cd1896bb16384c18e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458795"
---
# <a name="deletedoccurrencestatedefinition"></a><span data-ttu-id="3f793-103">DeletedOccurrenceStateDefinition</span><span class="sxs-lookup"><span data-stu-id="3f793-103">DeletedOccurrenceStateDefinition</span></span>

<span data-ttu-id="3f793-104">Le **DeletedOccurrenceStateDefinition** spécifie l’état d’une occurrence supprimée d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="3f793-104">The **DeletedOccurrenceStateDefinition** specifies the state for a deleted occurrence of a calendar item.</span></span> 
  
```XML
<DeletedOccurrenceStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeletedOccurrenceStateDefinition>
```

 <span data-ttu-id="3f793-105">**DeletedOccurrenceStateDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="3f793-105">**DeletedOccurrenceStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f793-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3f793-106">Attributes and elements</span></span>

<span data-ttu-id="3f793-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3f793-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f793-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3f793-108">Attributes</span></span>

<span data-ttu-id="3f793-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3f793-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f793-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3f793-110">Child elements</span></span>

|<span data-ttu-id="3f793-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3f793-111">**Element**</span></span>|<span data-ttu-id="3f793-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3f793-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f793-113">Occurrence (transition de fuseau horaire)</span><span class="sxs-lookup"><span data-stu-id="3f793-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="3f793-114">Spécifie la date de l’occurrence d’un élément de calendrier.</span><span class="sxs-lookup"><span data-stu-id="3f793-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3f793-115">IsOccurrencePresent</span><span class="sxs-lookup"><span data-stu-id="3f793-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="3f793-116">Spécifie une valeur de type Boolean qui indique si une occurrence de l’élément de calendrier est présente.</span><span class="sxs-lookup"><span data-stu-id="3f793-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3f793-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3f793-117">Parent elements</span></span>

|<span data-ttu-id="3f793-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3f793-118">**Element**</span></span>|<span data-ttu-id="3f793-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="3f793-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f793-120">StateDefinition</span><span class="sxs-lookup"><span data-stu-id="3f793-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="3f793-121">Spécifie une définition d’État.</span><span class="sxs-lookup"><span data-stu-id="3f793-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3f793-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="3f793-122">Remarks</span></span>

<span data-ttu-id="3f793-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3f793-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3f793-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f793-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f793-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3f793-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f793-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3f793-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3f793-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3f793-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3f793-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="3f793-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="3f793-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="3f793-129">Validation File</span></span>  <br/> |<span data-ttu-id="3f793-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="3f793-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3f793-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3f793-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3f793-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3f793-132">See also</span></span>

- [<span data-ttu-id="3f793-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3f793-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

