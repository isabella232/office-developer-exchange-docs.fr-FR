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
description: L’élément Argument spécifie les arguments à l’action.
ms.openlocfilehash: ed4e46a8d9897516e9c96bf3930f7d488bc06714
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755322"
---
# <a name="argument"></a><span data-ttu-id="35972-103">Argument</span><span class="sxs-lookup"><span data-stu-id="35972-103">Argument</span></span>

<span data-ttu-id="35972-104">L’élément **Argument** spécifie les arguments à l’action.</span><span class="sxs-lookup"><span data-stu-id="35972-104">The **Argument** element specifies arguments to the action.</span></span> 
  
```xml
<Argument Value=""/>
```

 <span data-ttu-id="35972-105">**ProtectionRuleArgumentType**</span><span class="sxs-lookup"><span data-stu-id="35972-105">**ProtectionRuleArgumentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="35972-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="35972-106">Attributes and elements</span></span>

<span data-ttu-id="35972-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="35972-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35972-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="35972-108">Attributes</span></span>

|<span data-ttu-id="35972-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="35972-109">**Attribute**</span></span>|<span data-ttu-id="35972-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="35972-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="35972-111">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="35972-111">**Value**</span></span> <br/> |<span data-ttu-id="35972-112">Une valeur de chaîne non vide qui représente la valeur d’un argument à la partie de l’action d’une règle de protection.</span><span class="sxs-lookup"><span data-stu-id="35972-112">A non-empty string value that represents the value of an argument to the action part of a protection rule.</span></span> <span data-ttu-id="35972-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="35972-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="35972-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="35972-114">Child elements</span></span>

<span data-ttu-id="35972-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="35972-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="35972-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="35972-116">Parent elements</span></span>

|<span data-ttu-id="35972-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="35972-117">**Element**</span></span>|<span data-ttu-id="35972-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="35972-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35972-119">Action (ProtectionRuleActionType)</span><span class="sxs-lookup"><span data-stu-id="35972-119">Action (ProtectionRuleActionType)</span></span>](action-protectionruleactiontype.md) <br/> |<span data-ttu-id="35972-120">Identifie l’action qui doit être exécutée si correspond à la partie de la condition de la règle.</span><span class="sxs-lookup"><span data-stu-id="35972-120">Identifies what action must be executed if the condition part of the rule matches.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="35972-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="35972-121">Text value</span></span>

<span data-ttu-id="35972-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="35972-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="35972-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="35972-123">Remarks</span></span>

<span data-ttu-id="35972-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="35972-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35972-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="35972-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35972-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="35972-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="35972-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="35972-127">Schema Name</span></span>  <br/> |<span data-ttu-id="35972-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="35972-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="35972-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="35972-129">Validation File</span></span>  <br/> |<span data-ttu-id="35972-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="35972-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="35972-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="35972-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="35972-132">False</span><span class="sxs-lookup"><span data-stu-id="35972-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="35972-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="35972-133">See also</span></span>

- [<span data-ttu-id="35972-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="35972-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

