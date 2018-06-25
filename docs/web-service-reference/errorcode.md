---
title: Code d’erreur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0bb00cee-c66b-4f34-b99d-355458f5e83b
description: L’élément ErrorCode représente un code d’erreur de validation de règle qui décrit ce qui a échoué validation pour chaque action ou au prédicat de la règle.
ms.openlocfilehash: ed8e2fa72b0eb007925742e6d194f3a391b3f3cb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756210"
---
# <a name="errorcode"></a><span data-ttu-id="900ac-103">Code d’erreur</span><span class="sxs-lookup"><span data-stu-id="900ac-103">ErrorCode</span></span>

<span data-ttu-id="900ac-104">L’élément **ErrorCode** représente un code d’erreur de validation de règle qui décrit ce qui a échoué validation pour chaque action ou au prédicat de la règle.</span><span class="sxs-lookup"><span data-stu-id="900ac-104">The **ErrorCode** element represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span> 
  
```XML
<ErrorCode/>
```

 <span data-ttu-id="900ac-105">**RuleValidationErrorCodeType**</span><span class="sxs-lookup"><span data-stu-id="900ac-105">**RuleValidationErrorCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="900ac-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="900ac-106">Attributes and elements</span></span>

<span data-ttu-id="900ac-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="900ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="900ac-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="900ac-108">Attributes</span></span>

<span data-ttu-id="900ac-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="900ac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="900ac-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="900ac-110">Child elements</span></span>

<span data-ttu-id="900ac-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="900ac-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="900ac-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="900ac-112">Parent elements</span></span>

|<span data-ttu-id="900ac-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="900ac-113">**Element**</span></span>|<span data-ttu-id="900ac-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="900ac-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="900ac-115">Erreur</span><span class="sxs-lookup"><span data-stu-id="900ac-115">Error</span></span>](error.md) <br/> |<span data-ttu-id="900ac-116">Représente une seule erreur de validation sur une valeur de la propriété règle particulière, la valeur de propriété prédicat ou la valeur de la propriété action.</span><span class="sxs-lookup"><span data-stu-id="900ac-116">Represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="900ac-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="900ac-117">Text value</span></span>

<span data-ttu-id="900ac-118">La valeur de texte pour cet élément est limitée à une des chaînes suivantes :</span><span class="sxs-lookup"><span data-stu-id="900ac-118">The text value for this element is restricted to one of the following strings:</span></span>
  
- <span data-ttu-id="900ac-119">ADOperationFailure</span><span class="sxs-lookup"><span data-stu-id="900ac-119">ADOperationFailure</span></span>
    
- <span data-ttu-id="900ac-120">ConnectedAccountNotFound</span><span class="sxs-lookup"><span data-stu-id="900ac-120">ConnectedAccountNotFound</span></span>
    
- <span data-ttu-id="900ac-121">CreateWithRuleId</span><span class="sxs-lookup"><span data-stu-id="900ac-121">CreateWithRuleId</span></span>
    
- <span data-ttu-id="900ac-122">EmptyValueFound</span><span class="sxs-lookup"><span data-stu-id="900ac-122">EmptyValueFound</span></span>
    
- <span data-ttu-id="900ac-123">DuplicatedPriority</span><span class="sxs-lookup"><span data-stu-id="900ac-123">DuplicatedPriority</span></span>
    
- <span data-ttu-id="900ac-124">DuplicatedOperationOnTheSameRule</span><span class="sxs-lookup"><span data-stu-id="900ac-124">DuplicatedOperationOnTheSameRule</span></span>
    
- <span data-ttu-id="900ac-125">FolderDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="900ac-125">FolderDoesNotExist</span></span>
    
- <span data-ttu-id="900ac-126">InvalidAddress</span><span class="sxs-lookup"><span data-stu-id="900ac-126">InvalidAddress</span></span>
    
- <span data-ttu-id="900ac-127">InvalidDateRange</span><span class="sxs-lookup"><span data-stu-id="900ac-127">InvalidDateRange</span></span>
    
- <span data-ttu-id="900ac-128">InvalidFolderId</span><span class="sxs-lookup"><span data-stu-id="900ac-128">InvalidFolderId</span></span>
    
- <span data-ttu-id="900ac-129">InvalidSizeRange</span><span class="sxs-lookup"><span data-stu-id="900ac-129">InvalidSizeRange</span></span>
    
- <span data-ttu-id="900ac-130">InvalidValue</span><span class="sxs-lookup"><span data-stu-id="900ac-130">InvalidValue</span></span>
    
- <span data-ttu-id="900ac-131">MessageClassificationNotFound</span><span class="sxs-lookup"><span data-stu-id="900ac-131">MessageClassificationNotFound</span></span>
    
- <span data-ttu-id="900ac-132">MissingAction</span><span class="sxs-lookup"><span data-stu-id="900ac-132">MissingAction</span></span>
    
- <span data-ttu-id="900ac-133">MissingParameter</span><span class="sxs-lookup"><span data-stu-id="900ac-133">MissingParameter</span></span>
    
- <span data-ttu-id="900ac-134">MissingRangeValue</span><span class="sxs-lookup"><span data-stu-id="900ac-134">MissingRangeValue</span></span>
    
- <span data-ttu-id="900ac-135">NotSettable</span><span class="sxs-lookup"><span data-stu-id="900ac-135">NotSettable</span></span>
    
- <span data-ttu-id="900ac-136">RecipientDoesNotExist</span><span class="sxs-lookup"><span data-stu-id="900ac-136">RecipientDoesNotExist</span></span>
    
- <span data-ttu-id="900ac-137">RuleNotFound</span><span class="sxs-lookup"><span data-stu-id="900ac-137">RuleNotFound</span></span>
    
- <span data-ttu-id="900ac-138">SizeLessThanZero</span><span class="sxs-lookup"><span data-stu-id="900ac-138">SizeLessThanZero</span></span>
    
- <span data-ttu-id="900ac-139">StringValueTooBig</span><span class="sxs-lookup"><span data-stu-id="900ac-139">StringValueTooBig</span></span>
    
- <span data-ttu-id="900ac-140">UnsupportedAddress</span><span class="sxs-lookup"><span data-stu-id="900ac-140">UnsupportedAddress</span></span>
    
- <span data-ttu-id="900ac-141">UnexpectedError</span><span class="sxs-lookup"><span data-stu-id="900ac-141">UnexpectedError</span></span>
    
- <span data-ttu-id="900ac-142">UnsupportedRule</span><span class="sxs-lookup"><span data-stu-id="900ac-142">UnsupportedRule</span></span>
    
## <a name="remarks"></a><span data-ttu-id="900ac-143">Remarques</span><span class="sxs-lookup"><span data-stu-id="900ac-143">Remarks</span></span>

<span data-ttu-id="900ac-144">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="900ac-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="900ac-145">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="900ac-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="900ac-146">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="900ac-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="900ac-147">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="900ac-147">Schema Name</span></span>  <br/> |<span data-ttu-id="900ac-148">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="900ac-148">Messages schema</span></span>  <br/> |
|<span data-ttu-id="900ac-149">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="900ac-149">Validation File</span></span>  <br/> |<span data-ttu-id="900ac-150">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="900ac-150">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="900ac-151">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="900ac-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="900ac-152">False</span><span class="sxs-lookup"><span data-stu-id="900ac-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="900ac-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="900ac-153">See also</span></span>



- [<span data-ttu-id="900ac-154">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="900ac-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

