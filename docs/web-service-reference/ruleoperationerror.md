---
title: RuleOperationError
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RuleOperationError
api_type:
- schema
ms.assetid: b447e610-d37c-40d3-9158-aa108a9f248e
description: L’élément RuleOperationError représente une erreur d’opération de règle.
ms.openlocfilehash: ff42addea0f55b13794e2c910d4d865ad0b17bc3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829265"
---
# <a name="ruleoperationerror"></a><span data-ttu-id="73cd4-103">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="73cd4-103">RuleOperationError</span></span>

<span data-ttu-id="73cd4-104">L’élément **RuleOperationError** représente une erreur d’opération de règle.</span><span class="sxs-lookup"><span data-stu-id="73cd4-104">The **RuleOperationError** element represents a rule operation error.</span></span> 
  
```XML
<RuleOperationError>
    <OperationIndex/>
    <ValidationErrors/>
</RuleOperationError>
```

 <span data-ttu-id="73cd4-105">**RuleOperationErrorType**</span><span class="sxs-lookup"><span data-stu-id="73cd4-105">**RuleOperationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73cd4-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="73cd4-106">Attributes and elements</span></span>

<span data-ttu-id="73cd4-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="73cd4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73cd4-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="73cd4-108">Attributes</span></span>

<span data-ttu-id="73cd4-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="73cd4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73cd4-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="73cd4-110">Child elements</span></span>

|<span data-ttu-id="73cd4-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="73cd4-111">**Element**</span></span>|<span data-ttu-id="73cd4-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="73cd4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73cd4-113">OperationIndex</span><span class="sxs-lookup"><span data-stu-id="73cd4-113">OperationIndex</span></span>](operationindex.md) <br/> |<span data-ttu-id="73cd4-114">Indique l’index de l’opération dans la demande qui a provoqué l’erreur de règle de l’opération.</span><span class="sxs-lookup"><span data-stu-id="73cd4-114">Indicates the index of the operation in the request that caused the rule operation error.</span></span>  <br/> |
|[<span data-ttu-id="73cd4-115">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="73cd4-115">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="73cd4-116">Représente un tableau règle des erreurs de validation sur chaque champ de règle qui comporte une erreur.</span><span class="sxs-lookup"><span data-stu-id="73cd4-116">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="73cd4-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="73cd4-117">Parent elements</span></span>

|<span data-ttu-id="73cd4-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="73cd4-118">**Element**</span></span>|<span data-ttu-id="73cd4-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="73cd4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73cd4-120">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="73cd4-120">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="73cd4-121">Représente un tableau règle des erreurs de validation sur chaque champ de règle qui comporte une erreur.</span><span class="sxs-lookup"><span data-stu-id="73cd4-121">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="73cd4-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="73cd4-122">Text value</span></span>

<span data-ttu-id="73cd4-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="73cd4-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="73cd4-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="73cd4-124">Remarks</span></span>

<span data-ttu-id="73cd4-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="73cd4-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73cd4-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="73cd4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73cd4-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="73cd4-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="73cd4-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="73cd4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="73cd4-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="73cd4-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="73cd4-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="73cd4-130">Validation File</span></span>  <br/> |<span data-ttu-id="73cd4-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="73cd4-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="73cd4-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="73cd4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="73cd4-133">True</span><span class="sxs-lookup"><span data-stu-id="73cd4-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73cd4-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="73cd4-134">See also</span></span>



- [<span data-ttu-id="73cd4-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="73cd4-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

