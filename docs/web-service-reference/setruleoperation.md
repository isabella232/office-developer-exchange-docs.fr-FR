---
title: SetRuleOperation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetRuleOperation
api_type:
- schema
ms.assetid: 2106a85b-58fe-49be-b71d-4ca6aa66e060
description: L’élément SetRuleOperation représente une opération de mise à jour d’une règle existante.
ms.openlocfilehash: 9c956394d14c510e8dcc95110ef1874ea7010be0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829451"
---
# <a name="setruleoperation"></a><span data-ttu-id="cfc01-103">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="cfc01-103">SetRuleOperation</span></span>

<span data-ttu-id="cfc01-104">L’élément **SetRuleOperation** représente une opération de mise à jour d’une règle existante.</span><span class="sxs-lookup"><span data-stu-id="cfc01-104">The **SetRuleOperation** element represents an operation to update an existing rule.</span></span> 
  
[<span data-ttu-id="cfc01-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="cfc01-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="cfc01-106">Opérations</span><span class="sxs-lookup"><span data-stu-id="cfc01-106">Operations</span></span>](operations.md)
  
```XML
<SetRuleOperation>
    <Rule/>
</SetRuleOperation>
```

 <span data-ttu-id="cfc01-107">**SetRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="cfc01-107">**SetRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cfc01-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cfc01-108">Attributes and elements</span></span>

<span data-ttu-id="cfc01-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cfc01-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cfc01-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="cfc01-110">Attributes</span></span>

<span data-ttu-id="cfc01-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cfc01-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cfc01-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cfc01-112">Child elements</span></span>

|<span data-ttu-id="cfc01-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cfc01-113">**Element**</span></span>|<span data-ttu-id="cfc01-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="cfc01-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cfc01-115">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="cfc01-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="cfc01-116">Représente une règle de boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="cfc01-116">Represents a rule in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cfc01-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cfc01-117">Parent elements</span></span>

|<span data-ttu-id="cfc01-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cfc01-118">**Element**</span></span>|<span data-ttu-id="cfc01-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="cfc01-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cfc01-120">Opérations</span><span class="sxs-lookup"><span data-stu-id="cfc01-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="cfc01-121">Contient un tableau des opérations de règle qui peuvent être effectuées sur une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="cfc01-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cfc01-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="cfc01-122">Text value</span></span>

<span data-ttu-id="cfc01-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cfc01-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cfc01-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="cfc01-124">Remarks</span></span>

<span data-ttu-id="cfc01-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cfc01-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cfc01-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cfc01-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cfc01-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cfc01-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cfc01-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cfc01-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cfc01-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cfc01-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="cfc01-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cfc01-130">Validation File</span></span>  <br/> |<span data-ttu-id="cfc01-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cfc01-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cfc01-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cfc01-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cfc01-133">False</span><span class="sxs-lookup"><span data-stu-id="cfc01-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cfc01-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cfc01-134">See also</span></span>



[<span data-ttu-id="cfc01-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="cfc01-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="cfc01-136">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="cfc01-136">DeleteRuleOperation</span></span>](deleteruleoperation.md)
  
[<span data-ttu-id="cfc01-137">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="cfc01-137">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="cfc01-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cfc01-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

