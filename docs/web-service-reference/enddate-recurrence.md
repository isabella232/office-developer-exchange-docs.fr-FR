---
title: EndDate (périodicité)
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
description: L’élément EndDate représente la date de fin d’une tâche périodique ou un élément de calendrier dont le type de motif EndDateRecurrence.
ms.openlocfilehash: b8570a069fc0a2d05044a9c85ab2d5c39d70ccdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756163"
---
# <a name="enddate-recurrence"></a><span data-ttu-id="d699a-103">EndDate (périodicité)</span><span class="sxs-lookup"><span data-stu-id="d699a-103">EndDate (Recurrence)</span></span>

<span data-ttu-id="d699a-104">L’élément **EndDate** représente la date de fin d’une tâche périodique ou un élément de calendrier dont le type de motif EndDateRecurrence.</span><span class="sxs-lookup"><span data-stu-id="d699a-104">The **EndDate** element represents the end date of a recurring task or a calendar item that has the EndDateRecurrence pattern type.</span></span> 
  
```xml
<EndDate/>
```

 <span data-ttu-id="d699a-105">**date**</span><span class="sxs-lookup"><span data-stu-id="d699a-105">**date**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d699a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d699a-106">Attributes and elements</span></span>

<span data-ttu-id="d699a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d699a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d699a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d699a-108">Attributes</span></span>

<span data-ttu-id="d699a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d699a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d699a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d699a-110">Child elements</span></span>

<span data-ttu-id="d699a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d699a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d699a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d699a-112">Parent elements</span></span>

|<span data-ttu-id="d699a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d699a-113">**Element**</span></span>|<span data-ttu-id="d699a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d699a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d699a-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="d699a-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="d699a-116">Décrit la date de début et date de fin de périodicité d’un élément.</span><span class="sxs-lookup"><span data-stu-id="d699a-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d699a-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d699a-117">Text value</span></span>

<span data-ttu-id="d699a-118">Une valeur de texte qui représente une date est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="d699a-118">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="d699a-119">La valeur ne peut pas dépasser 1 septembre, 4500 00:00:00.</span><span class="sxs-lookup"><span data-stu-id="d699a-119">The value cannot be larger than September 1, 4500 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d699a-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="d699a-120">Remarks</span></span>

<span data-ttu-id="d699a-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="d699a-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d699a-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d699a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d699a-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d699a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d699a-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d699a-124">Schema name</span></span>  <br/> |<span data-ttu-id="d699a-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d699a-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="d699a-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d699a-126">Validation file</span></span>  <br/> |<span data-ttu-id="d699a-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d699a-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d699a-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d699a-128">Can be empty</span></span>  <br/> |<span data-ttu-id="d699a-129">False</span><span class="sxs-lookup"><span data-stu-id="d699a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d699a-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d699a-130">See also</span></span>



- [<span data-ttu-id="d699a-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d699a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

