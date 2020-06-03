---
title: RuleOperationErrors
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f15c7b9e-a670-4a11-bb62-2a298c91f142
description: L'élément RuleOperationErrors représente un tableau des erreurs de validation de règle sur chaque champ de règle qui comporte une erreur.
ms.openlocfilehash: d547155f3cbf9eedd0f9bfac7bf3768b3630b50e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464951"
---
# <a name="ruleoperationerrors"></a><span data-ttu-id="a5edb-103">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="a5edb-103">RuleOperationErrors</span></span>

<span data-ttu-id="a5edb-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **RuleOperationErrors** représente un tableau des erreurs de validation de règle sur chaque champ de règle qui comporte une erreur.</span><span class="sxs-lookup"><span data-stu-id="a5edb-104">The **RuleOperationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
[<span data-ttu-id="a5edb-105">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="a5edb-105">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
  
[<span data-ttu-id="a5edb-106">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="a5edb-106">RuleOperationErrors</span></span>](ruleoperationerrors.md)
  
```XML
<RuleOperationErrors>
    <RuleOperationError>
</RuleOperationErrors>
```

 <span data-ttu-id="a5edb-107">**ArrayOfRuleOperationErrorsType**</span><span class="sxs-lookup"><span data-stu-id="a5edb-107">**ArrayOfRuleOperationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5edb-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a5edb-108">Attributes and elements</span></span>

<span data-ttu-id="a5edb-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a5edb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5edb-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="a5edb-110">Attributes</span></span>

<span data-ttu-id="a5edb-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a5edb-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5edb-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a5edb-112">Child elements</span></span>

|<span data-ttu-id="a5edb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a5edb-113">**Element**</span></span>|<span data-ttu-id="a5edb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a5edb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5edb-115">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="a5edb-115">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="a5edb-116">Représente une erreur d'opération de règle.</span><span class="sxs-lookup"><span data-stu-id="a5edb-116">Represents a rule operation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a5edb-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a5edb-117">Parent elements</span></span>

|<span data-ttu-id="a5edb-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a5edb-118">**Element**</span></span>|<span data-ttu-id="a5edb-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="a5edb-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5edb-120">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="a5edb-120">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md) <br/> |<span data-ttu-id="a5edb-121">Définit une réponse à une demande de [UpdateInboxRules](updateinboxrules.md) .</span><span class="sxs-lookup"><span data-stu-id="a5edb-121">Defines a response to an [UpdateInboxRules](updateinboxrules.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a5edb-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a5edb-122">Text value</span></span>

<span data-ttu-id="a5edb-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a5edb-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a5edb-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="a5edb-124">Remarks</span></span>

<span data-ttu-id="a5edb-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5edb-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5edb-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a5edb-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5edb-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a5edb-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a5edb-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a5edb-128">Schema name</span></span>  <br/> |<span data-ttu-id="a5edb-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a5edb-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a5edb-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a5edb-130">Validation file</span></span>  <br/> |<span data-ttu-id="a5edb-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a5edb-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a5edb-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a5edb-132">Can be empty</span></span>  <br/> |<span data-ttu-id="a5edb-133">True</span><span class="sxs-lookup"><span data-stu-id="a5edb-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5edb-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a5edb-134">See also</span></span>



[<span data-ttu-id="a5edb-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="a5edb-135">UpdateInboxRules</span></span>](updateinboxrules.md)


- [<span data-ttu-id="a5edb-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a5edb-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

