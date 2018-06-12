---
title: WithinDateRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WithinDateRange
api_type:
- schema
ms.assetid: 226aeb15-016f-45ca-992a-c137ba09ca08
description: L’élément WithinDateRange spécifie la plage de dates dans laquelle les messages entrants ont reçue dans l’ordre de l’exception ou la condition à appliquer.
ms.openlocfilehash: d85ef91c581008c2aafb06b1900c4514aebacd65
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839049"
---
# <a name="withindaterange"></a><span data-ttu-id="7529b-103">WithinDateRange</span><span class="sxs-lookup"><span data-stu-id="7529b-103">WithinDateRange</span></span>

<span data-ttu-id="7529b-104">L’élément **WithinDateRange** spécifie la plage de dates dans laquelle les messages entrants ont reçue dans l’ordre de l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="7529b-104">The **WithinDateRange** element specifies the date range within which incoming messages have to have been received in order for the condition or exception to apply.</span></span> 
  
```XML
<WithinDateRange>
     <StartDateTime/>
     <EndDateTime/>
</WithinDateRange>
```

 <span data-ttu-id="7529b-105">**RulePredicateDateRangeType**</span><span class="sxs-lookup"><span data-stu-id="7529b-105">**RulePredicateDateRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7529b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7529b-106">Attributes and elements</span></span>

<span data-ttu-id="7529b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7529b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7529b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7529b-108">Attributes</span></span>

<span data-ttu-id="7529b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7529b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7529b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7529b-110">Child elements</span></span>

|<span data-ttu-id="7529b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7529b-111">**Element**</span></span>|<span data-ttu-id="7529b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="7529b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7529b-113">StartDateTime</span><span class="sxs-lookup"><span data-stu-id="7529b-113">StartDateTime</span></span>](startdatetime.md) <br/> |<span data-ttu-id="7529b-114">Spécifie la règle de période et indique que la condition de règle est remplie après cette valeur.</span><span class="sxs-lookup"><span data-stu-id="7529b-114">Specifies the rule time period and indicates that the rule condition is met after this value.</span></span>  <br/> |
|[<span data-ttu-id="7529b-115">EndDateTime</span><span class="sxs-lookup"><span data-stu-id="7529b-115">EndDateTime</span></span>](enddatetime.md) <br/> |<span data-ttu-id="7529b-116">Spécifie la règle de période et indique que la condition de règle est remplie avant cette valeur.</span><span class="sxs-lookup"><span data-stu-id="7529b-116">Specifies the rule time period and indicates that the rule condition is met before this value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7529b-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7529b-117">Parent elements</span></span>

|<span data-ttu-id="7529b-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7529b-118">**Element**</span></span>|<span data-ttu-id="7529b-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="7529b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7529b-120">Conditions</span><span class="sxs-lookup"><span data-stu-id="7529b-120">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="7529b-121">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="7529b-121">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="7529b-122">Exceptions</span><span class="sxs-lookup"><span data-stu-id="7529b-122">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="7529b-123">Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="7529b-123">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7529b-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7529b-124">Text value</span></span>

<span data-ttu-id="7529b-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7529b-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7529b-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="7529b-126">Remarks</span></span>

<span data-ttu-id="7529b-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7529b-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7529b-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7529b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7529b-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7529b-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7529b-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7529b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="7529b-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7529b-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7529b-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7529b-132">Validation File</span></span>  <br/> |<span data-ttu-id="7529b-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7529b-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7529b-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7529b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="7529b-135">True</span><span class="sxs-lookup"><span data-stu-id="7529b-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7529b-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7529b-136">See also</span></span>



- [<span data-ttu-id="7529b-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7529b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

