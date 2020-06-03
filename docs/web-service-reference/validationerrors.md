---
title: ValidationErrors
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ValidationErrors
api_type:
- schema
ms.assetid: 009526aa-22e7-4f5c-be88-079175aa9122
description: L'élément ValidationErrors représente un tableau des erreurs de validation de règle sur chaque champ de règle qui comporte une erreur.
ms.openlocfilehash: 0861425b04e03a3e2e54a47a5027d0a11264392d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530274"
---
# <a name="validationerrors"></a><span data-ttu-id="ebfaa-103">ValidationErrors</span><span class="sxs-lookup"><span data-stu-id="ebfaa-103">ValidationErrors</span></span>

<span data-ttu-id="ebfaa-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **ValidationErrors** représente un tableau des erreurs de validation de règle sur chaque champ de règle qui comporte une erreur.</span><span class="sxs-lookup"><span data-stu-id="ebfaa-104">The **ValidationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
```XML
<VaidationErrors>
   <Error/>
</ValidationErrors>
```

 <span data-ttu-id="ebfaa-105">**ArrayOfRuleValidationErrorsType**</span><span class="sxs-lookup"><span data-stu-id="ebfaa-105">**ArrayOfRuleValidationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ebfaa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ebfaa-106">Attributes and elements</span></span>

<span data-ttu-id="ebfaa-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ebfaa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ebfaa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ebfaa-108">Attributes</span></span>

<span data-ttu-id="ebfaa-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ebfaa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ebfaa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ebfaa-110">Child elements</span></span>

|<span data-ttu-id="ebfaa-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ebfaa-111">**Element**</span></span>|<span data-ttu-id="ebfaa-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ebfaa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ebfaa-113">Erreur</span><span class="sxs-lookup"><span data-stu-id="ebfaa-113">Error</span></span>](error.md) <br/> |<span data-ttu-id="ebfaa-114">Représente une seule erreur de validation sur une valeur de la propriété règle particulière, valeur de la propriété prédicat ou valeur de la propriété action</span><span class="sxs-lookup"><span data-stu-id="ebfaa-114">Represents a single validation error on a particular rule property value, predicate property value, or action property value</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ebfaa-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ebfaa-115">Parent elements</span></span>

|<span data-ttu-id="ebfaa-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ebfaa-116">**Element**</span></span>|<span data-ttu-id="ebfaa-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ebfaa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ebfaa-118">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="ebfaa-118">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="ebfaa-119">Représente une erreur d'opération de règle.</span><span class="sxs-lookup"><span data-stu-id="ebfaa-119">Represents a rule operation error.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ebfaa-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ebfaa-120">Text value</span></span>

<span data-ttu-id="ebfaa-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ebfaa-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ebfaa-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="ebfaa-122">Remarks</span></span>

<span data-ttu-id="ebfaa-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ebfaa-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ebfaa-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ebfaa-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ebfaa-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ebfaa-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ebfaa-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ebfaa-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ebfaa-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ebfaa-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ebfaa-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ebfaa-128">Validation File</span></span>  <br/> |<span data-ttu-id="ebfaa-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ebfaa-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ebfaa-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ebfaa-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ebfaa-131">True</span><span class="sxs-lookup"><span data-stu-id="ebfaa-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ebfaa-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ebfaa-132">See also</span></span>



- [<span data-ttu-id="ebfaa-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ebfaa-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

