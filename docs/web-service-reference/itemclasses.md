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
description: L’élément ItemClasses représente les classes d’éléments qui doivent être marquées sur les messages entrants pour que la condition ou l’exception s’applique.
ms.openlocfilehash: 56b99cad2abef0a9953e1793e5b633acca83a9eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460112"
---
# <a name="itemclasses"></a><span data-ttu-id="fdea1-103">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="fdea1-103">ItemClasses</span></span>

<span data-ttu-id="fdea1-104">L’élément **ItemClasses** représente les classes d’éléments qui doivent être marquées sur les messages entrants pour que la condition ou l’exception s’applique.</span><span class="sxs-lookup"><span data-stu-id="fdea1-104">The **ItemClasses** element represents the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span> 
  
```XML
<ItemClasses>
    <String/>
</ItemClasses>
```

 <span data-ttu-id="fdea1-105">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="fdea1-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fdea1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fdea1-106">Attributes and elements</span></span>

<span data-ttu-id="fdea1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fdea1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fdea1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fdea1-108">Attributes</span></span>

<span data-ttu-id="fdea1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fdea1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fdea1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fdea1-110">Child elements</span></span>

|<span data-ttu-id="fdea1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fdea1-111">**Element**</span></span>|<span data-ttu-id="fdea1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="fdea1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fdea1-113">String</span><span class="sxs-lookup"><span data-stu-id="fdea1-113">String</span></span>](string.md) <br/> |<span data-ttu-id="fdea1-114">Représente une classe d’élément unique.</span><span class="sxs-lookup"><span data-stu-id="fdea1-114">Represents a single item class.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fdea1-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fdea1-115">Parent elements</span></span>

|<span data-ttu-id="fdea1-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fdea1-116">**Element**</span></span>|<span data-ttu-id="fdea1-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="fdea1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fdea1-118">Conditions</span><span class="sxs-lookup"><span data-stu-id="fdea1-118">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="fdea1-119">Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="fdea1-119">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="fdea1-120">Exceptions</span><span class="sxs-lookup"><span data-stu-id="fdea1-120">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="fdea1-121">Représente les exceptions qui représentent toutes les conditions d'exception de règle disponibles pour une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="fdea1-121">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fdea1-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="fdea1-122">Text value</span></span>

<span data-ttu-id="fdea1-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fdea1-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fdea1-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="fdea1-124">Remarks</span></span>

<span data-ttu-id="fdea1-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fdea1-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fdea1-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fdea1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fdea1-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fdea1-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fdea1-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fdea1-128">Schema name</span></span>  <br/> |<span data-ttu-id="fdea1-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fdea1-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="fdea1-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fdea1-130">Validation file</span></span>  <br/> |<span data-ttu-id="fdea1-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fdea1-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fdea1-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fdea1-132">Can be empty</span></span>  <br/> |<span data-ttu-id="fdea1-133">False</span><span class="sxs-lookup"><span data-stu-id="fdea1-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fdea1-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fdea1-134">See also</span></span>



- [<span data-ttu-id="fdea1-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fdea1-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

