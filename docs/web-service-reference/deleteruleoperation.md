---
title: DeleteRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteRuleOperation
api_type:
- schema
ms.assetid: c5e251af-f795-43cc-baaf-95d84475677c
description: L’élément DeleteRuleOperation contient une opération pour supprimer une règle de boîte de réception.
ms.openlocfilehash: 3410361e0b896fb0ef01c1873c9f8b0ac99afe58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755877"
---
# <a name="deleteruleoperation"></a><span data-ttu-id="04ca5-103">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="04ca5-103">DeleteRuleOperation</span></span>

<span data-ttu-id="04ca5-104">L’élément **DeleteRuleOperation** contient une opération pour supprimer une règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="04ca5-104">The **DeleteRuleOperation** element contains an operation to delete an existing Inbox rule.</span></span> 
  
- [<span data-ttu-id="04ca5-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="04ca5-105">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="04ca5-106">Opérations</span><span class="sxs-lookup"><span data-stu-id="04ca5-106">Operations</span></span>](operations.md)
  
```XML
<DeleteRuleOperation>
    <RuleId/>
</DeleteRuleOperation>
```

 <span data-ttu-id="04ca5-107">**DeleteRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="04ca5-107">**DeleteRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04ca5-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="04ca5-108">Attributes and elements</span></span>

<span data-ttu-id="04ca5-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="04ca5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04ca5-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="04ca5-110">Attributes</span></span>

<span data-ttu-id="04ca5-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="04ca5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04ca5-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="04ca5-112">Child elements</span></span>

|<span data-ttu-id="04ca5-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04ca5-113">**Element**</span></span>|<span data-ttu-id="04ca5-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="04ca5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04ca5-115">ID de la règle</span><span class="sxs-lookup"><span data-stu-id="04ca5-115">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="04ca5-116">Spécifie l’identificateur de la règle à supprimer.</span><span class="sxs-lookup"><span data-stu-id="04ca5-116">Specifies the identifier of the rule to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04ca5-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="04ca5-117">Parent elements</span></span>

|<span data-ttu-id="04ca5-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="04ca5-118">**Element**</span></span>|<span data-ttu-id="04ca5-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="04ca5-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04ca5-120">Opérations</span><span class="sxs-lookup"><span data-stu-id="04ca5-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="04ca5-121">Contient un tableau des opérations de règle qui peuvent être effectuées sur une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="04ca5-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04ca5-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="04ca5-122">Text value</span></span>

<span data-ttu-id="04ca5-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="04ca5-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04ca5-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="04ca5-124">Remarks</span></span>

<span data-ttu-id="04ca5-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="04ca5-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04ca5-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="04ca5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04ca5-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="04ca5-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04ca5-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="04ca5-128">Schema Name</span></span>  <br/> |<span data-ttu-id="04ca5-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="04ca5-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="04ca5-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="04ca5-130">Validation File</span></span>  <br/> |<span data-ttu-id="04ca5-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="04ca5-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04ca5-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="04ca5-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="04ca5-133">False</span><span class="sxs-lookup"><span data-stu-id="04ca5-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04ca5-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="04ca5-134">See also</span></span>

- [<span data-ttu-id="04ca5-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="04ca5-135">UpdateInboxRules</span></span>](updateinboxrules.md) 
- [<span data-ttu-id="04ca5-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="04ca5-136">SetRuleOperation</span></span>](setruleoperation.md) 
- [<span data-ttu-id="04ca5-137">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="04ca5-137">CreateRuleOperation</span></span>](createruleoperation.md)
- [<span data-ttu-id="04ca5-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="04ca5-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

