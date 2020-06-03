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
description: L’élément CreateRuleOperation représente une opération de création d’une nouvelle règle de boîte de réception.
ms.openlocfilehash: df857544e6d5840a3f738740114195e4c4bb5798
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460770"
---
# <a name="createruleoperation"></a><span data-ttu-id="298a3-103">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="298a3-103">CreateRuleOperation</span></span>

<span data-ttu-id="298a3-104">L’élément **CreateRuleOperation** représente une opération de création d’une nouvelle règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="298a3-104">The **CreateRuleOperation** element represents an operation to create a new Inbox rule.</span></span> 
  
[<span data-ttu-id="298a3-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="298a3-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="298a3-106">Operations</span><span class="sxs-lookup"><span data-stu-id="298a3-106">Operations</span></span>](operations.md)
  
```xml
<CreateRuleOperation>
    <Rule/>
</CreateRuleOperation>
```

 <span data-ttu-id="298a3-107">**CreateRuleOperationType**</span><span class="sxs-lookup"><span data-stu-id="298a3-107">**CreateRuleOperationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="298a3-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="298a3-108">Attributes and elements</span></span>

<span data-ttu-id="298a3-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="298a3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="298a3-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="298a3-110">Attributes</span></span>

<span data-ttu-id="298a3-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="298a3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="298a3-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="298a3-112">Child elements</span></span>

|<span data-ttu-id="298a3-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="298a3-113">**Element**</span></span>|<span data-ttu-id="298a3-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="298a3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="298a3-115">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="298a3-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="298a3-116">Représente une règle à créer dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="298a3-116">Represents a rule to be created in a user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="298a3-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="298a3-117">Parent elements</span></span>

|<span data-ttu-id="298a3-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="298a3-118">**Element**</span></span>|<span data-ttu-id="298a3-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="298a3-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="298a3-120">Operations</span><span class="sxs-lookup"><span data-stu-id="298a3-120">Operations</span></span>](operations.md) <br/> |<span data-ttu-id="298a3-121">Contient les opérations qui peuvent être effectuées sur une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="298a3-121">Contains the operations that can be performed on an Inbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="298a3-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="298a3-122">Text value</span></span>

<span data-ttu-id="298a3-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="298a3-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="298a3-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="298a3-124">Remarks</span></span>

<span data-ttu-id="298a3-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="298a3-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="298a3-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="298a3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="298a3-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="298a3-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="298a3-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="298a3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="298a3-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="298a3-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="298a3-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="298a3-130">Validation File</span></span>  <br/> |<span data-ttu-id="298a3-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="298a3-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="298a3-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="298a3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="298a3-133">False</span><span class="sxs-lookup"><span data-stu-id="298a3-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="298a3-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="298a3-134">See also</span></span>



[<span data-ttu-id="298a3-135">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="298a3-135">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="298a3-136">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="298a3-136">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="298a3-137">DeleteRuleOperation</span><span class="sxs-lookup"><span data-stu-id="298a3-137">DeleteRuleOperation</span></span>](deleteruleoperation.md)


- [<span data-ttu-id="298a3-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="298a3-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

