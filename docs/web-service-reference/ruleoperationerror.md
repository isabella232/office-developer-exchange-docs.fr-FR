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
ms.openlocfilehash: b5e0105a1fdb1564b3115a4c3a8411019f725483
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44464958"
---
# <a name="ruleoperationerror"></a><span data-ttu-id="8ed5e-103">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="8ed5e-103">RuleOperationError</span></span>

<span data-ttu-id="8ed5e-104">L’élément **RuleOperationError** représente une erreur d’opération de règle.</span><span class="sxs-lookup"><span data-stu-id="8ed5e-104">The **RuleOperationError** element represents a rule operation error.</span></span> 
  
```XML
<RuleOperationError>
    <OperationIndex/>
    <ValidationErrors/>
</RuleOperationError>
```

 <span data-ttu-id="8ed5e-105">**RuleOperationErrorType**</span><span class="sxs-lookup"><span data-stu-id="8ed5e-105">**RuleOperationErrorType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8ed5e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8ed5e-106">Attributes and elements</span></span>

<span data-ttu-id="8ed5e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8ed5e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ed5e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8ed5e-108">Attributes</span></span>

<span data-ttu-id="8ed5e-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8ed5e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ed5e-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8ed5e-110">Child elements</span></span>

|<span data-ttu-id="8ed5e-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8ed5e-111">**Element**</span></span>|<span data-ttu-id="8ed5e-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="8ed5e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ed5e-113">OperationIndex</span><span class="sxs-lookup"><span data-stu-id="8ed5e-113">OperationIndex</span></span>](operationindex.md) <br/> |<span data-ttu-id="8ed5e-114">Indique l’index de l’opération dans la demande qui a provoqué l’erreur d’opération de la règle.</span><span class="sxs-lookup"><span data-stu-id="8ed5e-114">Indicates the index of the operation in the request that caused the rule operation error.</span></span>  <br/> |
|[<span data-ttu-id="8ed5e-115">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="8ed5e-115">ValidationErrors</span></span>](validationerrors.md) <br/> |<span data-ttu-id="8ed5e-116">Représente un tableau des erreurs de validation de règle sur chaque champ de règle qui comporte une erreur.</span><span class="sxs-lookup"><span data-stu-id="8ed5e-116">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8ed5e-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8ed5e-117">Parent elements</span></span>

|<span data-ttu-id="8ed5e-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8ed5e-118">**Element**</span></span>|<span data-ttu-id="8ed5e-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="8ed5e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ed5e-120">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="8ed5e-120">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="8ed5e-121">Représente un tableau des erreurs de validation de règle sur chaque champ de règle qui comporte une erreur.</span><span class="sxs-lookup"><span data-stu-id="8ed5e-121">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ed5e-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8ed5e-122">Text value</span></span>

<span data-ttu-id="8ed5e-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8ed5e-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8ed5e-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="8ed5e-124">Remarks</span></span>

<span data-ttu-id="8ed5e-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8ed5e-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ed5e-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8ed5e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ed5e-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8ed5e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8ed5e-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8ed5e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="8ed5e-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="8ed5e-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8ed5e-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8ed5e-130">Validation File</span></span>  <br/> |<span data-ttu-id="8ed5e-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8ed5e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8ed5e-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8ed5e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="8ed5e-133">True</span><span class="sxs-lookup"><span data-stu-id="8ed5e-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ed5e-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8ed5e-134">See also</span></span>



- [<span data-ttu-id="8ed5e-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8ed5e-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

