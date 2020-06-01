---
title: ErrorCode
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: L’élément ErrorCode représente un code d’erreur de validation de règle qui décrit ce qui a échoué lors de chaque prédicat ou action de règle.
ms.openlocfilehash: 6432aeee786d74a9afcb346cb66765f9001257de
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460077"
---
# <a name="errorcode"></a><span data-ttu-id="fe1c2-103">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="fe1c2-103">ErrorCode</span></span>

<span data-ttu-id="fe1c2-104">L’élément **ErrorCode** représente un code d’erreur de validation de règle qui décrit ce qui a échoué lors de chaque prédicat ou action de règle.</span><span class="sxs-lookup"><span data-stu-id="fe1c2-104">The **ErrorCode** element represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="fe1c2-105">**RuleValidationErrorCodeType**</span><span class="sxs-lookup"><span data-stu-id="fe1c2-105">**RuleValidationErrorCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fe1c2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fe1c2-106">Attributes and elements</span></span>

<span data-ttu-id="fe1c2-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fe1c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fe1c2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fe1c2-108">Attributes</span></span>

<span data-ttu-id="fe1c2-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fe1c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fe1c2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fe1c2-110">Child elements</span></span>

<span data-ttu-id="fe1c2-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fe1c2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fe1c2-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fe1c2-112">Parent elements</span></span>

|<span data-ttu-id="fe1c2-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fe1c2-113">**Element**</span></span>|<span data-ttu-id="fe1c2-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="fe1c2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fe1c2-115">Erreur</span><span class="sxs-lookup"><span data-stu-id="fe1c2-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="fe1c2-116">Représente une seule erreur de validation sur une valeur de propriété de règle, une valeur de propriété de prédicat ou une valeur de propriété d’action particulière.</span><span class="sxs-lookup"><span data-stu-id="fe1c2-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fe1c2-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="fe1c2-117">Text value</span></span>

<span data-ttu-id="fe1c2-118">La valeur de texte de cet élément est restreinte à l’une des chaînes suivantes :</span><span class="sxs-lookup"><span data-stu-id="fe1c2-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="fe1c2-119">ADOperationFailure</span><span class="sxs-lookup"><span data-stu-id="fe1c2-119">ADOperationFailure</span></span>
    
- <span data-ttu-id="fe1c2-120">ConnectedAccountNotFound</span><span class="sxs-lookup"><span data-stu-id="fe1c2-120">ConnectedAccountNotFound</span></span>
    
- <span data-ttu-id="fe1c2-121">CreateWithRuleId</span><span class="sxs-lookup"><span data-stu-id="fe1c2-121">CreateWithRuleId</span></span>
    
- <span data-ttu-id="fe1c2-122">EmptyValueFound</span><span class="sxs-lookup"><span data-stu-id="fe1c2-122">EmptyValueFound</span></span>
    
- <span data-ttu-id="fe1c2-123">DuplicatedPriority</span><span class="sxs-lookup"><span data-stu-id="fe1c2-123">DuplicatedPriority</span></span>
    
- <span data-ttu-id="fe1c2-124">DuplicatedOperationOnTheSameRule</span><span class="sxs-lookup"><span data-stu-id="fe1c2-124">DuplicatedOperationOnTheSameRule</span></span>
    
- <span data-ttu-id="fe1c2-125">FolderDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="fe1c2-125">FolderDoesNotExist</span></span>
    
- <span data-ttu-id="fe1c2-126">InvalidAddress</span><span class="sxs-lookup"><span data-stu-id="fe1c2-126">InvalidAddress</span></span>
    
- <span data-ttu-id="fe1c2-127">InvalidDateRange</span><span class="sxs-lookup"><span data-stu-id="fe1c2-127">InvalidDateRange</span></span>
    
- <span data-ttu-id="fe1c2-128">InvalidFolderId</span><span class="sxs-lookup"><span data-stu-id="fe1c2-128">InvalidFolderId</span></span>
    
- <span data-ttu-id="fe1c2-129">InvalidSizeRange</span><span class="sxs-lookup"><span data-stu-id="fe1c2-129">InvalidSizeRange</span></span>
    
- <span data-ttu-id="fe1c2-130">InvalidValue</span><span class="sxs-lookup"><span data-stu-id="fe1c2-130">InvalidValue</span></span>
    
- <span data-ttu-id="fe1c2-131">MessageClassificationNotFound</span><span class="sxs-lookup"><span data-stu-id="fe1c2-131">MessageClassificationNotFound</span></span>
    
- <span data-ttu-id="fe1c2-132">MissingAction</span><span class="sxs-lookup"><span data-stu-id="fe1c2-132">MissingAction</span></span>
    
- <span data-ttu-id="fe1c2-133">MissingParameter</span><span class="sxs-lookup"><span data-stu-id="fe1c2-133">MissingParameter</span></span>
    
- <span data-ttu-id="fe1c2-134">MissingRangeValue</span><span class="sxs-lookup"><span data-stu-id="fe1c2-134">MissingRangeValue</span></span>
    
- <span data-ttu-id="fe1c2-135">NotSettable</span><span class="sxs-lookup"><span data-stu-id="fe1c2-135">NotSettable</span></span>
    
- <span data-ttu-id="fe1c2-136">RecipientDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="fe1c2-136">RecipientDoesNotExist</span></span>
    
- <span data-ttu-id="fe1c2-137">RuleNotFound</span><span class="sxs-lookup"><span data-stu-id="fe1c2-137">RuleNotFound</span></span>
    
- <span data-ttu-id="fe1c2-138">SizeLessThanZero</span><span class="sxs-lookup"><span data-stu-id="fe1c2-138">SizeLessThanZero</span></span>
    
- <span data-ttu-id="fe1c2-139">StringValueTooBig</span><span class="sxs-lookup"><span data-stu-id="fe1c2-139">StringValueTooBig</span></span>
    
- <span data-ttu-id="fe1c2-140">UnsupportedAddress</span><span class="sxs-lookup"><span data-stu-id="fe1c2-140">UnsupportedAddress</span></span>
    
- <span data-ttu-id="fe1c2-141">UnexpectedError</span><span class="sxs-lookup"><span data-stu-id="fe1c2-141">UnexpectedError</span></span>
    
- <span data-ttu-id="fe1c2-142">UnsupportedRule</span><span class="sxs-lookup"><span data-stu-id="fe1c2-142">UnsupportedRule</span></span>
    
## <a name="remarks"></a><span data-ttu-id="fe1c2-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="fe1c2-143">Remarks</span></span>

<span data-ttu-id="fe1c2-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe1c2-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fe1c2-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fe1c2-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fe1c2-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fe1c2-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fe1c2-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fe1c2-147">Schema Name</span></span>  <br/> |<span data-ttu-id="fe1c2-148">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="fe1c2-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fe1c2-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fe1c2-149">Validation File</span></span>  <br/> |<span data-ttu-id="fe1c2-150">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fe1c2-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fe1c2-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fe1c2-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="fe1c2-152">False</span><span class="sxs-lookup"><span data-stu-id="fe1c2-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fe1c2-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fe1c2-153">See also</span></span>



- [<span data-ttu-id="fe1c2-154">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fe1c2-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

