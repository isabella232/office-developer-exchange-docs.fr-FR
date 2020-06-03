---
title: EndDate (récurrence)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDate
api_type:
- schema
ms.assetid: 16026595-26f8-4770-8a6d-0d3e4157effd
description: L’élément EndDate représente la date de fin d’une tâche périodique ou d’un élément de calendrier qui a le type de modèle EndDateRecurrence.
ms.openlocfilehash: 53d9b04faf1d8f740c858080b5fcbeadf577df0d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460161"
---
# <a name="enddate-recurrence"></a><span data-ttu-id="f4ec6-103">EndDate (récurrence)</span><span class="sxs-lookup"><span data-stu-id="f4ec6-103">EndDate (Recurrence)</span></span>

<span data-ttu-id="f4ec6-104">L’élément **EndDate** représente la date de fin d’une tâche périodique ou d’un élément de calendrier qui a le type de modèle EndDateRecurrence.</span><span class="sxs-lookup"><span data-stu-id="f4ec6-104">The **EndDate** element represents the end date of a recurring task or a calendar item that has the EndDateRecurrence pattern type.</span></span> 
  
```xml
<EndDate/>
```

 <span data-ttu-id="f4ec6-105">**date**</span><span class="sxs-lookup"><span data-stu-id="f4ec6-105">**date**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4ec6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f4ec6-106">Attributes and elements</span></span>

<span data-ttu-id="f4ec6-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f4ec6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4ec6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f4ec6-108">Attributes</span></span>

<span data-ttu-id="f4ec6-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f4ec6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4ec6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f4ec6-110">Child elements</span></span>

<span data-ttu-id="f4ec6-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f4ec6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4ec6-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f4ec6-112">Parent elements</span></span>

|<span data-ttu-id="f4ec6-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f4ec6-113">**Element**</span></span>|<span data-ttu-id="f4ec6-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f4ec6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4ec6-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="f4ec6-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="f4ec6-116">Décrit la date de début et la date de fin d’une périodicité d’élément.</span><span class="sxs-lookup"><span data-stu-id="f4ec6-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f4ec6-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f4ec6-117">Text value</span></span>

<span data-ttu-id="f4ec6-118">Une valeur de texte qui représente une date est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="f4ec6-118">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="f4ec6-119">La valeur ne peut pas être supérieure au 1er septembre 4500 00:00:00.</span><span class="sxs-lookup"><span data-stu-id="f4ec6-119">The value cannot be larger than September 1, 4500 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f4ec6-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="f4ec6-120">Remarks</span></span>

<span data-ttu-id="f4ec6-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f4ec6-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4ec6-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f4ec6-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4ec6-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f4ec6-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f4ec6-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f4ec6-124">Schema name</span></span>  <br/> |<span data-ttu-id="f4ec6-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f4ec6-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="f4ec6-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f4ec6-126">Validation file</span></span>  <br/> |<span data-ttu-id="f4ec6-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f4ec6-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f4ec6-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f4ec6-128">Can be empty</span></span>  <br/> |<span data-ttu-id="f4ec6-129">False</span><span class="sxs-lookup"><span data-stu-id="f4ec6-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4ec6-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f4ec6-130">See also</span></span>



- [<span data-ttu-id="f4ec6-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f4ec6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

