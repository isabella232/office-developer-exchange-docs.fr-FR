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
description: L’élément error représente une erreur de validation unique sur une valeur de propriété de règle, une valeur de propriété de prédicat ou une valeur de propriété d’action particulière.
ms.openlocfilehash: 9c28f63aa79446d89152868c81c85ffa7b3a8b39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460679"
---
# <a name="error"></a><span data-ttu-id="988ba-103">Erreur</span><span class="sxs-lookup"><span data-stu-id="988ba-103">Error</span></span>

<span data-ttu-id="988ba-104">L’élément **Error** représente une erreur de validation unique sur une valeur de propriété de règle, une valeur de propriété de prédicat ou une valeur de propriété d’action particulière.</span><span class="sxs-lookup"><span data-stu-id="988ba-104">The **Error** element represents a single validation error on a particular rule property value, predicate property value, or action property value.</span></span> 
  
```XML
<Error>
   <FieldUri/>
   <ErrorCode/>
   <ErrorMessage/>
   <FieldValue/>
</Error>
```

 <span data-ttu-id="988ba-105">**RuleValidationErrorType**</span><span class="sxs-lookup"><span data-stu-id="988ba-105">**RuleValidationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="988ba-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="988ba-106">Attributes and elements</span></span>

<span data-ttu-id="988ba-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="988ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="988ba-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="988ba-108">Attributes</span></span>

<span data-ttu-id="988ba-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="988ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="988ba-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="988ba-110">Child elements</span></span>

|<span data-ttu-id="988ba-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="988ba-111">**Element**</span></span>|<span data-ttu-id="988ba-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="988ba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="988ba-113">FieldUri (règle)</span><span class="sxs-lookup"><span data-stu-id="988ba-113">FieldUri (Rule)</span></span>](fielduri-rule.md) <br/> |<span data-ttu-id="988ba-114">Spécifie l’URI du champ de règle à l’origine de l’erreur de validation.</span><span class="sxs-lookup"><span data-stu-id="988ba-114">Specifies the URI to the rule field that caused the validation error.</span></span>  <br/> |
|[<span data-ttu-id="988ba-115">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="988ba-115">ErrorCode</span></span>](errorcode.md) <br/> |<span data-ttu-id="988ba-116">Représente un code d’erreur de validation de règle qui décrit l’échec de validation pour chaque prédicat ou action de règle.</span><span class="sxs-lookup"><span data-stu-id="988ba-116">Represents a rule validation error code that describes what failed validation for each rule predicate or action.</span></span>  <br/> |
|[<span data-ttu-id="988ba-117">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="988ba-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="988ba-118">Représente la raison de l’erreur de validation.</span><span class="sxs-lookup"><span data-stu-id="988ba-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="988ba-119">FieldValue</span><span class="sxs-lookup"><span data-stu-id="988ba-119">FieldValue</span></span>](fieldvalue.md) <br/> |<span data-ttu-id="988ba-120">Représente la valeur du champ à l’origine de l’erreur de validation.</span><span class="sxs-lookup"><span data-stu-id="988ba-120">Represents the value of the field that caused the validation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="988ba-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="988ba-121">Parent elements</span></span>

|<span data-ttu-id="988ba-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="988ba-122">**Element**</span></span>|<span data-ttu-id="988ba-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="988ba-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="988ba-124">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="988ba-124">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="988ba-125">Représente un tableau des erreurs de validation de règle sur chaque champ de règle qui comporte une erreur.</span><span class="sxs-lookup"><span data-stu-id="988ba-125">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="988ba-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="988ba-126">Text value</span></span>

<span data-ttu-id="988ba-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="988ba-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="988ba-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="988ba-128">Remarks</span></span>

<span data-ttu-id="988ba-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="988ba-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="988ba-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="988ba-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="988ba-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="988ba-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="988ba-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="988ba-132">Schema Name</span></span>  <br/> |<span data-ttu-id="988ba-133">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="988ba-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="988ba-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="988ba-134">Validation File</span></span>  <br/> |<span data-ttu-id="988ba-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="988ba-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="988ba-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="988ba-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="988ba-137">True</span><span class="sxs-lookup"><span data-stu-id="988ba-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="988ba-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="988ba-138">See also</span></span>



- [<span data-ttu-id="988ba-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="988ba-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

