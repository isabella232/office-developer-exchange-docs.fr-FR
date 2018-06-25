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
ms.openlocfilehash: 7dc85b5cd84af5ad00511a3df2b31ee3541e12b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829261"
---
# <a name="ruleoperationerrors"></a><span data-ttu-id="bd93b-103">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="bd93b-103">RuleOperationErrors</span></span>

<span data-ttu-id="bd93b-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **RuleOperationErrors** représente un tableau des erreurs de validation de règle sur chaque champ de règle qui comporte une erreur.</span><span class="sxs-lookup"><span data-stu-id="bd93b-104">The **RuleOperationErrors** element represents an array of rule validation errors on each rule field that has an error.</span></span> 
  
[<span data-ttu-id="bd93b-105">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="bd93b-105">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md)
  
[<span data-ttu-id="bd93b-106">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="bd93b-106">RuleOperationErrors</span></span>](ruleoperationerrors.md)
  
```XML
<RuleOperationErrors>
    <RuleOperationError>
</RuleOperationErrors>
```

 <span data-ttu-id="bd93b-107">**ArrayOfRuleOperationErrorsType**</span><span class="sxs-lookup"><span data-stu-id="bd93b-107">**ArrayOfRuleOperationErrorsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd93b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bd93b-108">Attributes and elements</span></span>

<span data-ttu-id="bd93b-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bd93b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd93b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="bd93b-110">Attributes</span></span>

<span data-ttu-id="bd93b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bd93b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd93b-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bd93b-112">Child elements</span></span>

|<span data-ttu-id="bd93b-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bd93b-113">**Element**</span></span>|<span data-ttu-id="bd93b-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="bd93b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd93b-115">RuleOperationError</span><span class="sxs-lookup"><span data-stu-id="bd93b-115">RuleOperationError</span></span>](ruleoperationerror.md) <br/> |<span data-ttu-id="bd93b-116">Représente une erreur d'opération de règle.</span><span class="sxs-lookup"><span data-stu-id="bd93b-116">Represents a rule operation error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd93b-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bd93b-117">Parent elements</span></span>

|<span data-ttu-id="bd93b-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bd93b-118">**Element**</span></span>|<span data-ttu-id="bd93b-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="bd93b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd93b-120">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="bd93b-120">UpdateInboxRulesResponse</span></span>](updateinboxrulesresponse.md) <br/> |<span data-ttu-id="bd93b-121">Définit une réponse à une demande de [UpdateInboxRules](updateinboxrules.md) .</span><span class="sxs-lookup"><span data-stu-id="bd93b-121">Defines a response to an [UpdateInboxRules](updateinboxrules.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bd93b-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bd93b-122">Text value</span></span>

<span data-ttu-id="bd93b-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bd93b-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bd93b-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="bd93b-124">Remarks</span></span>

<span data-ttu-id="bd93b-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd93b-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd93b-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bd93b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd93b-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bd93b-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bd93b-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bd93b-128">Schema name</span></span>  <br/> |<span data-ttu-id="bd93b-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="bd93b-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bd93b-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bd93b-130">Validation file</span></span>  <br/> |<span data-ttu-id="bd93b-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bd93b-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bd93b-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bd93b-132">Can be empty</span></span>  <br/> |<span data-ttu-id="bd93b-133">True</span><span class="sxs-lookup"><span data-stu-id="bd93b-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd93b-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bd93b-134">See also</span></span>



[<span data-ttu-id="bd93b-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="bd93b-135">UpdateInboxRules</span></span>](updateinboxrules.md)


- [<span data-ttu-id="bd93b-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bd93b-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

