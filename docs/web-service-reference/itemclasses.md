---
title: ItemClasses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemClasses
api_type:
- schema
ms.assetid: f95430cc-2860-47c1-af2d-8c4156c9b281
description: L’élément ItemClasses représente les classes d’élément qui doivent être marqués sur les messages entrants afin que l’exception ou la condition à appliquer.
ms.openlocfilehash: 70a4823f9017ba8c6f894394d5907f1adeb80167
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828148"
---
# <a name="itemclasses"></a><span data-ttu-id="1000b-103">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="1000b-103">ItemClasses</span></span>

<span data-ttu-id="1000b-104">L’élément **ItemClasses** représente les classes d’élément qui doivent être marqués sur les messages entrants afin que l’exception ou la condition à appliquer.</span><span class="sxs-lookup"><span data-stu-id="1000b-104">The **ItemClasses** element represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="1000b-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="1000b-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1000b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1000b-106">Attributes and elements</span></span>

<span data-ttu-id="1000b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1000b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1000b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1000b-108">Attributes</span></span>

<span data-ttu-id="1000b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1000b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1000b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1000b-110">Child elements</span></span>

|<span data-ttu-id="1000b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1000b-111">**Element**</span></span>|<span data-ttu-id="1000b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1000b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1000b-113">String</span><span class="sxs-lookup"><span data-stu-id="1000b-113">String</span></span>](string.md) <br/> |<span data-ttu-id="1000b-114">Représente une classe d’élément unique.</span><span class="sxs-lookup"><span data-stu-id="1000b-114">Represents a single item class.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1000b-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1000b-115">Parent elements</span></span>

|<span data-ttu-id="1000b-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1000b-116">**Element**</span></span>|<span data-ttu-id="1000b-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="1000b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1000b-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="1000b-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="1000b-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="1000b-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="1000b-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="1000b-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="1000b-121">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="1000b-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1000b-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1000b-122">Text value</span></span>

<span data-ttu-id="1000b-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1000b-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1000b-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="1000b-124">Remarks</span></span>

<span data-ttu-id="1000b-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1000b-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1000b-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1000b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1000b-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1000b-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1000b-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1000b-128">Schema name</span></span>  <br/> |<span data-ttu-id="1000b-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1000b-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="1000b-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1000b-130">Validation file</span></span>  <br/> |<span data-ttu-id="1000b-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1000b-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1000b-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1000b-132">Can be empty</span></span>  <br/> |<span data-ttu-id="1000b-133">False</span><span class="sxs-lookup"><span data-stu-id="1000b-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1000b-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1000b-134">See also</span></span>



- [<span data-ttu-id="1000b-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1000b-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

