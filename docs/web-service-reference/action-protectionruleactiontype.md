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
description: L’élément Action identifie l’action qui doit être exécutée si correspond à la partie de la condition de la règle.
ms.openlocfilehash: 8f699e698d3159c5ff2636da506542da3b218251
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756330"
---
# <a name="action-protectionruleactiontype"></a><span data-ttu-id="9f164-103">Action (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="9f164-103">Action (ProtectionRuleActionType)</span></span>

<span data-ttu-id="9f164-104">L’élément **Action** identifie l’action qui doit être exécutée si correspond à la partie de la condition de la règle.</span><span class="sxs-lookup"><span data-stu-id="9f164-104">The **Action** element identifies what action must be executed if the condition part of the rule matches.</span></span> 
  
```xml
<Action Name="">
   <Argument/>
</Action>

```

 <span data-ttu-id="9f164-105">**ProtectionRuleActionType**</span><span class="sxs-lookup"><span data-stu-id="9f164-105">**ProtectionRuleActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f164-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9f164-106">Attributes and elements</span></span>

<span data-ttu-id="9f164-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9f164-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f164-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9f164-108">Attributes</span></span>

|<span data-ttu-id="9f164-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="9f164-109">**Attribute**</span></span>|<span data-ttu-id="9f164-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f164-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9f164-111">**Name**</span><span class="sxs-lookup"><span data-stu-id="9f164-111">**Name**</span></span> <br/> |<span data-ttu-id="9f164-112">Identifie le nom de l’action.</span><span class="sxs-lookup"><span data-stu-id="9f164-112">Identifies the name of the action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9f164-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9f164-113">Child elements</span></span>

|<span data-ttu-id="9f164-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9f164-114">**Element**</span></span>|<span data-ttu-id="9f164-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f164-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f164-116">Argument</span><span class="sxs-lookup"><span data-stu-id="9f164-116">Argument</span></span>](argument.md) <br/> |<span data-ttu-id="9f164-117">Spécifie les arguments à l’action.</span><span class="sxs-lookup"><span data-stu-id="9f164-117">Specifies arguments to the action.</span></span> <span data-ttu-id="9f164-118">Cet élément ne se produit pas si l’action spécifiée ne nécessite pas de spécifier des arguments.</span><span class="sxs-lookup"><span data-stu-id="9f164-118">This element will not occur if the specified action does not require arguments to be specified.</span></span> <span data-ttu-id="9f164-119">Cet élément peut se produire une ou plusieurs fois si une action nécessite un ou plusieurs arguments.</span><span class="sxs-lookup"><span data-stu-id="9f164-119">This element can occur one or more times if an action requires one or more arguments.</span></span> <span data-ttu-id="9f164-120">L’action **RightsProtectMessage** contiendra un argument unique.</span><span class="sxs-lookup"><span data-stu-id="9f164-120">The **RightsProtectMessage** action will contain a single argument.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f164-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9f164-121">Parent elements</span></span>

|<span data-ttu-id="9f164-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9f164-122">**Element**</span></span>|<span data-ttu-id="9f164-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="9f164-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f164-124">Règle</span><span class="sxs-lookup"><span data-stu-id="9f164-124">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="9f164-125">Contient une règle de protection unique.</span><span class="sxs-lookup"><span data-stu-id="9f164-125">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f164-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="9f164-126">Remarks</span></span>

<span data-ttu-id="9f164-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f164-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f164-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9f164-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f164-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9f164-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f164-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9f164-130">Schema Name</span></span>  <br/> |<span data-ttu-id="9f164-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="9f164-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="9f164-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="9f164-132">Validation File</span></span>  <br/> |<span data-ttu-id="9f164-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9f164-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f164-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9f164-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f164-135">False</span><span class="sxs-lookup"><span data-stu-id="9f164-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f164-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9f164-136">See also</span></span>

- [<span data-ttu-id="9f164-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9f164-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

