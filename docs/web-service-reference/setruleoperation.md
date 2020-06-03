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
ms.openlocfilehash: 96fba2f229003b8c729c36614e69655852a3aa8c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526332"
---
# <a name="setruleoperation"></a><span data-ttu-id="d8e4d-103">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="d8e4d-103">SetRuleOperation</span></span>

<span data-ttu-id="d8e4d-104">L’élément **SetRuleOperation** représente une opération de mise à jour d’une règle existante.</span><span class="sxs-lookup"><span data-stu-id="d8e4d-104">The **SetRuleOperation** element represents an operation to update an existing rule.</span></span> 
  
[<span data-ttu-id="d8e4d-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="d8e4d-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="d8e4d-106">Operations</span><span class="sxs-lookup"><span data-stu-id="d8e4d-106">Operations</span></span>](operations.md)
  
```XML
<SetRuleOperation>
    <Rule/>
</SetRuleOperation>
```

 <span data-ttu-id="d8e4d-107">**SetRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="d8e4d-107">**SetRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8e4d-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d8e4d-108">Attributes and elements</span></span>

<span data-ttu-id="d8e4d-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d8e4d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8e4d-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d8e4d-110">Attributes</span></span>

<span data-ttu-id="d8e4d-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d8e4d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8e4d-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d8e4d-112">Child elements</span></span>

|<span data-ttu-id="d8e4d-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d8e4d-113">**Element**</span></span>|<span data-ttu-id="d8e4d-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d8e4d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8e4d-115">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="d8e4d-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="d8e4d-116">Représente une règle dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d8e4d-116">Represents a rule in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8e4d-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d8e4d-117">Parent elements</span></span>

|<span data-ttu-id="d8e4d-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d8e4d-118">**Element**</span></span>|<span data-ttu-id="d8e4d-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="d8e4d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8e4d-120">Opérations</span><span class="sxs-lookup"><span data-stu-id="d8e4d-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="d8e4d-121">Contient un tableau des opérations de règle qui peuvent être effectuées sur une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="d8e4d-121">Contains an array of rule operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d8e4d-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d8e4d-122">Text value</span></span>

<span data-ttu-id="d8e4d-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d8e4d-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d8e4d-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="d8e4d-124">Remarks</span></span>

<span data-ttu-id="d8e4d-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8e4d-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8e4d-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d8e4d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8e4d-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d8e4d-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8e4d-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d8e4d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d8e4d-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d8e4d-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8e4d-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d8e4d-130">Validation File</span></span>  <br/> |<span data-ttu-id="d8e4d-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d8e4d-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8e4d-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d8e4d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8e4d-133">False</span><span class="sxs-lookup"><span data-stu-id="d8e4d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8e4d-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d8e4d-134">See also</span></span>



[<span data-ttu-id="d8e4d-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="d8e4d-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="d8e4d-136">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="d8e4d-136">DeleteRuleOperation</span></span>](deleteruleoperation.md)
  
[<span data-ttu-id="d8e4d-137">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="d8e4d-137">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="d8e4d-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d8e4d-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

