---
title: Action (ProtectionRuleActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: ca090dec-e2c5-49c8-a057-8d1f2409147f
description: L’élément action identifie l’action qui doit être exécutée si la partie condition de la règle correspond.
ms.openlocfilehash: 220a6fea16abb9ea823ae6239537b8c121702589
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527508"
---
# <a name="action-protectionruleactiontype"></a><span data-ttu-id="037e7-103">Action (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="037e7-103">Action (ProtectionRuleActionType)</span></span>

<span data-ttu-id="037e7-104">L’élément **action** identifie l’action qui doit être exécutée si la partie condition de la règle correspond.</span><span class="sxs-lookup"><span data-stu-id="037e7-104">The **Action** element identifies what action must be executed if the condition part of the rule matches.</span></span> 
  
```xml
<Action Name="">
   <Argument/>
</Action>

```

 <span data-ttu-id="037e7-105">**ProtectionRuleActionType**</span><span class="sxs-lookup"><span data-stu-id="037e7-105">**ProtectionRuleActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="037e7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="037e7-106">Attributes and elements</span></span>

<span data-ttu-id="037e7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="037e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="037e7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="037e7-108">Attributes</span></span>

|<span data-ttu-id="037e7-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="037e7-109">**Attribute**</span></span>|<span data-ttu-id="037e7-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="037e7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="037e7-111">**Nom**</span><span class="sxs-lookup"><span data-stu-id="037e7-111">**Name**</span></span> <br/> |<span data-ttu-id="037e7-112">Identifie le nom de l’action.</span><span class="sxs-lookup"><span data-stu-id="037e7-112">Identifies the name of the action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="037e7-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="037e7-113">Child elements</span></span>

|<span data-ttu-id="037e7-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="037e7-114">**Element**</span></span>|<span data-ttu-id="037e7-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="037e7-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="037e7-116">Argument</span><span class="sxs-lookup"><span data-stu-id="037e7-116">Argument</span></span>](argument.md) <br/> |<span data-ttu-id="037e7-117">Spécifie les arguments de l’action.</span><span class="sxs-lookup"><span data-stu-id="037e7-117">Specifies arguments to the action.</span></span> <span data-ttu-id="037e7-118">Cet élément ne se produira pas si l’action spécifiée ne nécessite pas que des arguments soient spécifiés.</span><span class="sxs-lookup"><span data-stu-id="037e7-118">This element will not occur if the specified action does not require arguments to be specified.</span></span> <span data-ttu-id="037e7-119">Cet élément peut apparaître une ou plusieurs fois si une action requiert un ou plusieurs arguments.</span><span class="sxs-lookup"><span data-stu-id="037e7-119">This element can occur one or more times if an action requires one or more arguments.</span></span> <span data-ttu-id="037e7-120">L’action **RightsProtectMessage** contient un seul argument.</span><span class="sxs-lookup"><span data-stu-id="037e7-120">The **RightsProtectMessage** action will contain a single argument.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="037e7-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="037e7-121">Parent elements</span></span>

|<span data-ttu-id="037e7-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="037e7-122">**Element**</span></span>|<span data-ttu-id="037e7-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="037e7-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="037e7-124">Règle</span><span class="sxs-lookup"><span data-stu-id="037e7-124">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="037e7-125">Contient une règle de protection unique.</span><span class="sxs-lookup"><span data-stu-id="037e7-125">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="037e7-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="037e7-126">Remarks</span></span>

<span data-ttu-id="037e7-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="037e7-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="037e7-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="037e7-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="037e7-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="037e7-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="037e7-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="037e7-130">Schema Name</span></span>  <br/> |<span data-ttu-id="037e7-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="037e7-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="037e7-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="037e7-132">Validation File</span></span>  <br/> |<span data-ttu-id="037e7-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="037e7-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="037e7-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="037e7-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="037e7-135">False</span><span class="sxs-lookup"><span data-stu-id="037e7-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="037e7-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="037e7-136">See also</span></span>

- [<span data-ttu-id="037e7-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="037e7-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

