---
title: CreateRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateRuleOperation
api_type:
- schema
ms.assetid: e9f70726-db08-4089-839e-a41007d0a473
description: L’élément CreateRuleOperation représente une opération pour créer une nouvelle règle de boîte de réception.
ms.openlocfilehash: c531f222ffe886e6ef53a99609cfa27e84fd6107
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755738"
---
# <a name="createruleoperation"></a><span data-ttu-id="6adc4-103">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="6adc4-103">CreateRuleOperation</span></span>

<span data-ttu-id="6adc4-104">L’élément **CreateRuleOperation** représente une opération pour créer une nouvelle règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="6adc4-104">The **CreateRuleOperation** element represents an operation to create a new Inbox rule.</span></span> 
  
[<span data-ttu-id="6adc4-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="6adc4-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="6adc4-106">Opérations</span><span class="sxs-lookup"><span data-stu-id="6adc4-106">Operations</span></span>](operations.md)
  
```xml
<CreateRuleOperation>
    <Rule/>
</CreateRuleOperation>
```

 <span data-ttu-id="6adc4-107">**CreateRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="6adc4-107">**CreateRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6adc4-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6adc4-108">Attributes and elements</span></span>

<span data-ttu-id="6adc4-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6adc4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6adc4-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="6adc4-110">Attributes</span></span>

<span data-ttu-id="6adc4-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6adc4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6adc4-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6adc4-112">Child elements</span></span>

|<span data-ttu-id="6adc4-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6adc4-113">**Element**</span></span>|<span data-ttu-id="6adc4-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="6adc4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6adc4-115">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="6adc4-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="6adc4-116">Représente une règle à créer dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6adc4-116">Represents a rule to be created in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6adc4-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6adc4-117">Parent elements</span></span>

|<span data-ttu-id="6adc4-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6adc4-118">**Element**</span></span>|<span data-ttu-id="6adc4-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="6adc4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6adc4-120">Opérations</span><span class="sxs-lookup"><span data-stu-id="6adc4-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="6adc4-121">Contient les opérations qui peuvent être effectuées sur une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="6adc4-121">Contains the operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6adc4-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6adc4-122">Text value</span></span>

<span data-ttu-id="6adc4-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6adc4-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6adc4-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="6adc4-124">Remarks</span></span>

<span data-ttu-id="6adc4-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6adc4-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6adc4-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6adc4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6adc4-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6adc4-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6adc4-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6adc4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6adc4-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6adc4-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="6adc4-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6adc4-130">Validation File</span></span>  <br/> |<span data-ttu-id="6adc4-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6adc4-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6adc4-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6adc4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="6adc4-133">False</span><span class="sxs-lookup"><span data-stu-id="6adc4-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6adc4-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6adc4-134">See also</span></span>



[<span data-ttu-id="6adc4-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="6adc4-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="6adc4-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="6adc4-136">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="6adc4-137">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="6adc4-137">DeleteRuleOperation</span></span>](deleteruleoperation.md)


- [<span data-ttu-id="6adc4-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6adc4-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

