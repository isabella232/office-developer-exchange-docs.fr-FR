---
title: Erreur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Error
api_type:
- schema
ms.assetid: b1f54673-578a-496b-99f5-0fde2c669278
description: L’élément Error représente une seule erreur de validation sur une valeur de la propriété règle particulière, la valeur de propriété prédicat ou la valeur de la propriété action.
ms.openlocfilehash: adb2de56b7610aa92b5bf5b8d43ac22f35021b64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756205"
---
# <a name="error"></a><span data-ttu-id="016f1-103">Erreur</span><span class="sxs-lookup"><span data-stu-id="016f1-103">Error</span></span>

<span data-ttu-id="016f1-104">L’élément **Error** représente une seule erreur de validation sur une valeur de la propriété règle particulière, la valeur de propriété prédicat ou la valeur de la propriété action.</span><span class="sxs-lookup"><span data-stu-id="016f1-104">The **Error** element represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span> 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 <span data-ttu-id="016f1-105">**RuleValidationErrorType**</span><span class="sxs-lookup"><span data-stu-id="016f1-105">**RuleValidationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="016f1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="016f1-106">Attributes and elements</span></span>

<span data-ttu-id="016f1-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="016f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="016f1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="016f1-108">Attributes</span></span>

<span data-ttu-id="016f1-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="016f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="016f1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="016f1-110">Child elements</span></span>

|<span data-ttu-id="016f1-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="016f1-111">**Element**</span></span>|<span data-ttu-id="016f1-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="016f1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="016f1-113">FieldUri (règle)</span><span class="sxs-lookup"><span data-stu-id="016f1-113">FieldUri (Rule)</span></span>](fielduri-rule.md) <br/> |<span data-ttu-id="016f1-114">Spécifie l’URI pour le champ règle qui a provoqué l’erreur de validation.</span><span class="sxs-lookup"><span data-stu-id="016f1-114">Specifies the URI to the rule field that caused the validation error.</span></span>  <br/> |
|[<span data-ttu-id="016f1-115">Code d’erreur</span><span class="sxs-lookup"><span data-stu-id="016f1-115">ErrorCode</span></span>](errorcode.md) <br/> |<span data-ttu-id="016f1-116">Représente un code d’erreur de validation de règle qui décrit ce qui a échoué validation pour chaque action ou au prédicat de la règle.</span><span class="sxs-lookup"><span data-stu-id="016f1-116">Represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span>  <br/> |
|[<span data-ttu-id="016f1-117">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="016f1-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="016f1-118">Représente la raison de l’erreur de validation.</span><span class="sxs-lookup"><span data-stu-id="016f1-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="016f1-119">FieldValue</span><span class="sxs-lookup"><span data-stu-id="016f1-119">FieldValue</span></span>](fieldvalue.md) <br/> |<span data-ttu-id="016f1-120">Représente la valeur du champ qui a provoqué l’erreur de validation.</span><span class="sxs-lookup"><span data-stu-id="016f1-120">Represents the value of the field that caused the validation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="016f1-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="016f1-121">Parent elements</span></span>

|<span data-ttu-id="016f1-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="016f1-122">**Element**</span></span>|<span data-ttu-id="016f1-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="016f1-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="016f1-124">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="016f1-124">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="016f1-125">Représente un tableau règle des erreurs de validation sur chaque champ de règle qui comporte une erreur.</span><span class="sxs-lookup"><span data-stu-id="016f1-125">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="016f1-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="016f1-126">Text value</span></span>

<span data-ttu-id="016f1-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="016f1-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="016f1-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="016f1-128">Remarks</span></span>

<span data-ttu-id="016f1-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="016f1-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="016f1-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="016f1-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="016f1-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="016f1-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="016f1-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="016f1-132">Schema Name</span></span>  <br/> |<span data-ttu-id="016f1-133">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="016f1-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="016f1-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="016f1-134">Validation File</span></span>  <br/> |<span data-ttu-id="016f1-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="016f1-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="016f1-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="016f1-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="016f1-137">True</span><span class="sxs-lookup"><span data-stu-id="016f1-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="016f1-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="016f1-138">See also</span></span>



- [<span data-ttu-id="016f1-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="016f1-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

