---
title: Rule
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
description: L’élément rule contient une règle de protection unique.
ms.openlocfilehash: 6c18a2bd026893cd333bc7007203abf04a6f0be7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465000"
---
# <a name="rule"></a><span data-ttu-id="3af89-103">Rule</span><span class="sxs-lookup"><span data-stu-id="3af89-103">Rule</span></span>

<span data-ttu-id="3af89-104">L’élément **rule** contient une règle de protection unique.</span><span class="sxs-lookup"><span data-stu-id="3af89-104">The **Rule** element contains a single protection rule.</span></span> 
  
```XML
<Rule Name="" UserOverridable=="" Priority="">
   <Condition/>
   <Action/>
</Rule>
```

 <span data-ttu-id="3af89-105">**ProtectionRuleType**</span><span class="sxs-lookup"><span data-stu-id="3af89-105">**ProtectionRuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3af89-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3af89-106">Attributes and elements</span></span>

<span data-ttu-id="3af89-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3af89-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3af89-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3af89-108">Attributes</span></span>

|<span data-ttu-id="3af89-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="3af89-109">**Attribute**</span></span>|<span data-ttu-id="3af89-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="3af89-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3af89-111">**Nom**</span><span class="sxs-lookup"><span data-stu-id="3af89-111">**Name**</span></span> <br/> |<span data-ttu-id="3af89-112">Identifie le nom de la règle.</span><span class="sxs-lookup"><span data-stu-id="3af89-112">Identifies the name of the rule.</span></span> <span data-ttu-id="3af89-113">Attribut obligatoire de type String avec une longueur minimale de 1.</span><span class="sxs-lookup"><span data-stu-id="3af89-113">A required attribute of type string with a minimum length of 1.</span></span>  <br/> |
|<span data-ttu-id="3af89-114">**UserOverridable**</span><span class="sxs-lookup"><span data-stu-id="3af89-114">**UserOverridable**</span></span> <br/> |<span data-ttu-id="3af89-115">Indique si la règle est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="3af89-115">Specifies whether the rule is mandatory.</span></span> <span data-ttu-id="3af89-116">Si la règle est obligatoire, la valeur de cet attribut doit être **false**.</span><span class="sxs-lookup"><span data-stu-id="3af89-116">If the rule is mandatory, this attribute value must be **false**.</span></span> <span data-ttu-id="3af89-117">Attribut obligatoire de type Boolean.</span><span class="sxs-lookup"><span data-stu-id="3af89-117">A required attribute of type Boolean.</span></span>  <br/> |
|<span data-ttu-id="3af89-118">**Priorité**</span><span class="sxs-lookup"><span data-stu-id="3af89-118">**Priority**</span></span> <br/> |<span data-ttu-id="3af89-119">Spécifie la priorité de la règle.</span><span class="sxs-lookup"><span data-stu-id="3af89-119">Specifies the rule priority.</span></span> <span data-ttu-id="3af89-120">Attribut obligatoire de type int avec une valeur minimale de 1.</span><span class="sxs-lookup"><span data-stu-id="3af89-120">A required attribute of type int with a minimum value of 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3af89-121">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3af89-121">Child elements</span></span>

|<span data-ttu-id="3af89-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3af89-122">**Element**</span></span>|<span data-ttu-id="3af89-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="3af89-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3af89-124">Condition</span><span class="sxs-lookup"><span data-stu-id="3af89-124">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="3af89-125">Identifie la condition qui doit être remplie pour que la partie action de la règle soit exécutée.</span><span class="sxs-lookup"><span data-stu-id="3af89-125">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="3af89-126">Action (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="3af89-126">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="3af89-127">Identifie l’action qui doit être exécutée si la partie conditionnelle de la règle correspond.</span><span class="sxs-lookup"><span data-stu-id="3af89-127">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3af89-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3af89-128">Parent elements</span></span>

|<span data-ttu-id="3af89-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3af89-129">**Element**</span></span>|<span data-ttu-id="3af89-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="3af89-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3af89-131">Gestion</span><span class="sxs-lookup"><span data-stu-id="3af89-131">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3af89-132">Contient un tableau de règles de protection.</span><span class="sxs-lookup"><span data-stu-id="3af89-132">Contains an array of protection rules.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3af89-133">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3af89-133">Text value</span></span>

<span data-ttu-id="3af89-134">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3af89-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3af89-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="3af89-135">Remarks</span></span>

<span data-ttu-id="3af89-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3af89-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3af89-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3af89-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3af89-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3af89-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3af89-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3af89-139">Schema Name</span></span>  <br/> |<span data-ttu-id="3af89-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3af89-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="3af89-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3af89-141">Validation File</span></span>  <br/> |<span data-ttu-id="3af89-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3af89-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3af89-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3af89-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="3af89-144">False</span><span class="sxs-lookup"><span data-stu-id="3af89-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3af89-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3af89-145">See also</span></span>



- [<span data-ttu-id="3af89-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3af89-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

