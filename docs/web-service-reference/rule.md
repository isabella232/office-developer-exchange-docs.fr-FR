---
title: Règle
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rule
api_type:
- schema
ms.assetid: c30f3851-bd56-4473-9106-dc85e9619486
description: L’élément de règle contient une règle de protection unique.
ms.openlocfilehash: 9abbb70381c214211172d2d5ba1ed43ee4797f17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829263"
---
# <a name="rule"></a><span data-ttu-id="bfabe-103">Règle</span><span class="sxs-lookup"><span data-stu-id="bfabe-103">Rule</span></span>

<span data-ttu-id="bfabe-104">L’élément de **règle** contient une règle de protection unique.</span><span class="sxs-lookup"><span data-stu-id="bfabe-104">The **Rule** element contains a single protection rule.</span></span> 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 <span data-ttu-id="bfabe-105">**ProtectionRuleType**</span><span class="sxs-lookup"><span data-stu-id="bfabe-105">**ProtectionRuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bfabe-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bfabe-106">Attributes and elements</span></span>

<span data-ttu-id="bfabe-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bfabe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bfabe-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bfabe-108">Attributes</span></span>

|<span data-ttu-id="bfabe-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="bfabe-109">**Attribute**</span></span>|<span data-ttu-id="bfabe-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="bfabe-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bfabe-111">**Name**</span><span class="sxs-lookup"><span data-stu-id="bfabe-111">**Name**</span></span> <br/> |<span data-ttu-id="bfabe-112">Identifie le nom de la règle.</span><span class="sxs-lookup"><span data-stu-id="bfabe-112">Identifies the name of the rule.</span></span> <span data-ttu-id="bfabe-113">Un attribut obligatoire de type chaîne avec une longueur minimale de 1.</span><span class="sxs-lookup"><span data-stu-id="bfabe-113">A required attribute of type string with a minimum length of 1.</span></span>  <br/> |
|<span data-ttu-id="bfabe-114">**UserOverridable**</span><span class="sxs-lookup"><span data-stu-id="bfabe-114">**UserOverridable**</span></span> <br/> |<span data-ttu-id="bfabe-115">Indique si la règle est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="bfabe-115">Specifies whether the rule is mandatory.</span></span> <span data-ttu-id="bfabe-116">Si la règle est obligatoire, cette valeur d’attribut doit avoir la **valeur false**.</span><span class="sxs-lookup"><span data-stu-id="bfabe-116">If the rule is mandatory, this attribute value must be **false**.</span></span> <span data-ttu-id="bfabe-117">Attribut de type Boolean obligatoire.</span><span class="sxs-lookup"><span data-stu-id="bfabe-117">A required attribute of type Boolean.</span></span>  <br/> |
|<span data-ttu-id="bfabe-118">**Priority**</span><span class="sxs-lookup"><span data-stu-id="bfabe-118">**Priority**</span></span> <br/> |<span data-ttu-id="bfabe-119">Spécifie la priorité de la règle.</span><span class="sxs-lookup"><span data-stu-id="bfabe-119">Specifies the rule priority.</span></span> <span data-ttu-id="bfabe-120">Un attribut obligatoire de type int avec une valeur minimale de 1.</span><span class="sxs-lookup"><span data-stu-id="bfabe-120">A required attribute of type int with a minimum value of 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bfabe-121">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bfabe-121">Child elements</span></span>

|<span data-ttu-id="bfabe-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bfabe-122">**Element**</span></span>|<span data-ttu-id="bfabe-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="bfabe-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfabe-124">Condition</span><span class="sxs-lookup"><span data-stu-id="bfabe-124">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="bfabe-125">Identifie la condition qui doit être remplie pour la partie de l’action de la règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="bfabe-125">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="bfabe-126">Action (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="bfabe-126">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="bfabe-127">Identifie l’action qui doit être exécutée si correspond à la partie de la condition de la règle.</span><span class="sxs-lookup"><span data-stu-id="bfabe-127">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bfabe-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bfabe-128">Parent elements</span></span>

|<span data-ttu-id="bfabe-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bfabe-129">**Element**</span></span>|<span data-ttu-id="bfabe-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="bfabe-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfabe-131">Règles</span><span class="sxs-lookup"><span data-stu-id="bfabe-131">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bfabe-132">Contient un tableau des règles de protection.</span><span class="sxs-lookup"><span data-stu-id="bfabe-132">Contains an array of protection rules.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bfabe-133">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bfabe-133">Text value</span></span>

<span data-ttu-id="bfabe-134">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bfabe-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bfabe-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="bfabe-135">Remarks</span></span>

<span data-ttu-id="bfabe-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bfabe-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bfabe-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bfabe-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bfabe-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bfabe-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bfabe-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bfabe-139">Schema Name</span></span>  <br/> |<span data-ttu-id="bfabe-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bfabe-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="bfabe-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bfabe-141">Validation File</span></span>  <br/> |<span data-ttu-id="bfabe-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bfabe-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bfabe-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bfabe-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="bfabe-144">False</span><span class="sxs-lookup"><span data-stu-id="bfabe-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bfabe-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bfabe-145">See also</span></span>



- [<span data-ttu-id="bfabe-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bfabe-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

