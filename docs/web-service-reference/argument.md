---
title: Argument
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Argument
api_type:
- schema
ms.assetid: 15b0bfb8-2448-4ceb-aeac-965115e0fb72
description: L’élément argument spécifie les arguments de l’action.
ms.openlocfilehash: 41e3b1d891610669b0cc93f3daf6e8ee98c48396
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464755"
---
# <a name="argument"></a><span data-ttu-id="0ce7a-103">Argument</span><span class="sxs-lookup"><span data-stu-id="0ce7a-103">Argument</span></span>

<span data-ttu-id="0ce7a-104">L’élément **argument** spécifie les arguments de l’action.</span><span class="sxs-lookup"><span data-stu-id="0ce7a-104">The **Argument** element specifies arguments to the action.</span></span> 
  
```xml
<Argument Value=""/>
```

 <span data-ttu-id="0ce7a-105">**ProtectionRuleArgumentType**</span><span class="sxs-lookup"><span data-stu-id="0ce7a-105">**ProtectionRuleArgumentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ce7a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0ce7a-106">Attributes and elements</span></span>

<span data-ttu-id="0ce7a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0ce7a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ce7a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0ce7a-108">Attributes</span></span>

|<span data-ttu-id="0ce7a-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="0ce7a-109">**Attribute**</span></span>|<span data-ttu-id="0ce7a-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ce7a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0ce7a-111">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="0ce7a-111">**Value**</span></span> <br/> |<span data-ttu-id="0ce7a-112">Valeur de type String non vide qui représente la valeur d’un argument de la partie action d’une règle de protection.</span><span class="sxs-lookup"><span data-stu-id="0ce7a-112">A non-empty string value that represents the value of an argument to the action part of a protection rule.</span></span> <span data-ttu-id="0ce7a-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="0ce7a-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0ce7a-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0ce7a-114">Child elements</span></span>

<span data-ttu-id="0ce7a-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0ce7a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0ce7a-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0ce7a-116">Parent elements</span></span>

|<span data-ttu-id="0ce7a-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0ce7a-117">**Element**</span></span>|<span data-ttu-id="0ce7a-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="0ce7a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ce7a-119">Action (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="0ce7a-119">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="0ce7a-120">Identifie l’action qui doit être exécutée si la partie conditionnelle de la règle correspond.</span><span class="sxs-lookup"><span data-stu-id="0ce7a-120">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0ce7a-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0ce7a-121">Text value</span></span>

<span data-ttu-id="0ce7a-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0ce7a-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ce7a-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="0ce7a-123">Remarks</span></span>

<span data-ttu-id="0ce7a-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ce7a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ce7a-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0ce7a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ce7a-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0ce7a-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0ce7a-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0ce7a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="0ce7a-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0ce7a-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="0ce7a-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0ce7a-129">Validation File</span></span>  <br/> |<span data-ttu-id="0ce7a-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0ce7a-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0ce7a-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0ce7a-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ce7a-132">False</span><span class="sxs-lookup"><span data-stu-id="0ce7a-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ce7a-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0ce7a-133">See also</span></span>

- [<span data-ttu-id="0ce7a-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0ce7a-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

