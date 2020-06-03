---
title: Règle (RuleType)
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
ms.assetid: 259a1f62-b235-4964-88bf-2d1f1c05a563
description: L’élément rule contient une seule règle et représente une règle dans la boîte aux lettres d’un utilisateur.
ms.openlocfilehash: cdbd21df235a62a9e201e1eaae1d82a8ac10cdd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465078"
---
# <a name="rule-ruletype"></a><span data-ttu-id="ac997-103">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="ac997-103">Rule (RuleType)</span></span>

<span data-ttu-id="ac997-104">L’élément **rule** contient une seule règle et représente une règle dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ac997-104">The **Rule** element contains a single rule and represents a rule in a user's mailbox.</span></span> 
  
```XML
<Rule>
    <RuleId>
    <DisplayName>
    <Priority>
    <IsEnabled>
    <IsNotSupported>
    <IsInError>
    <Conditions>
    <Exceptions>
    <Actions>
</Rule>
```

 <span data-ttu-id="ac997-105">**RuleType**</span><span class="sxs-lookup"><span data-stu-id="ac997-105">**RuleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac997-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ac997-106">Attributes and elements</span></span>

<span data-ttu-id="ac997-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ac997-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac997-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ac997-108">Attributes</span></span>

<span data-ttu-id="ac997-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ac997-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac997-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ac997-110">Child elements</span></span>

|<span data-ttu-id="ac997-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ac997-111">**Element**</span></span>|<span data-ttu-id="ac997-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ac997-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac997-113">RuleId</span><span class="sxs-lookup"><span data-stu-id="ac997-113">RuleId</span></span>](ruleid.md) <br/> |<span data-ttu-id="ac997-114">Spécifie l’identificateur de la règle.</span><span class="sxs-lookup"><span data-stu-id="ac997-114">Specifies the rule identifier.</span></span>  <br/> |
|[<span data-ttu-id="ac997-115">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="ac997-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="ac997-116">Contient le nom complet d’une règle.</span><span class="sxs-lookup"><span data-stu-id="ac997-116">Contains the display name of a rule.</span></span>  <br/> |
|[<span data-ttu-id="ac997-117">Priorité</span><span class="sxs-lookup"><span data-stu-id="ac997-117">Priority</span></span>](priority.md) <br/> |<span data-ttu-id="ac997-118">Indique l’ordre dans lequel une règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="ac997-118">Indicates the order in which a rule is to be run.</span></span>  <br/> |
|[<span data-ttu-id="ac997-119">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="ac997-119">IsEnabled</span></span>](isenabled.md) <br/> |<span data-ttu-id="ac997-120">Indique si la règle est activée.</span><span class="sxs-lookup"><span data-stu-id="ac997-120">Indicates whether the rule is enabled.</span></span>  <br/> |
|[<span data-ttu-id="ac997-121">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="ac997-121">IsNotSupported</span></span>](isnotsupported.md) <br/> |<span data-ttu-id="ac997-122">Indique si la règle ne peut pas être modifiée avec les API avec code managé.</span><span class="sxs-lookup"><span data-stu-id="ac997-122">Indicates whether the rule cannot be modified with the managed code APIs.</span></span>  <br/> |
|[<span data-ttu-id="ac997-123">IsInError</span><span class="sxs-lookup"><span data-stu-id="ac997-123">IsInError</span></span>](isinerror.md) <br/> |<span data-ttu-id="ac997-124">Indique si la règle se trouve dans une condition d’erreur.</span><span class="sxs-lookup"><span data-stu-id="ac997-124">Indicates whether the rule is in an error condition.</span></span>  <br/> |
|[<span data-ttu-id="ac997-125">Conditions</span><span class="sxs-lookup"><span data-stu-id="ac997-125">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="ac997-126">Identifie les conditions qui, lorsqu’elles sont remplies, déclencheront les actions de règle pour une règle.</span><span class="sxs-lookup"><span data-stu-id="ac997-126">Identifies the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="ac997-127">Exceptions</span><span class="sxs-lookup"><span data-stu-id="ac997-127">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="ac997-128">Identifie les exceptions qui représentent toutes les conditions d’exception de règle disponibles pour la règle de boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="ac997-128">Identifies the exceptions that represent all the available rule exception conditions for the inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="ac997-129">Actions</span><span class="sxs-lookup"><span data-stu-id="ac997-129">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="ac997-130">Représente les actions à effectuer sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="ac997-130">Represents the actions to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ac997-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ac997-131">Parent elements</span></span>

|<span data-ttu-id="ac997-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ac997-132">**Element**</span></span>|<span data-ttu-id="ac997-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="ac997-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac997-134">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="ac997-134">CreateRuleOperation</span></span>](createruleoperation.md) <br/> |<span data-ttu-id="ac997-135">Représente une opération de création d’une règle.</span><span class="sxs-lookup"><span data-stu-id="ac997-135">Represents an operation to create a new rule.</span></span>  <br/> |
|[<span data-ttu-id="ac997-136">InboxRules</span><span class="sxs-lookup"><span data-stu-id="ac997-136">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="ac997-137">Représente un tableau de règles dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ac997-137">Represents an array of rules in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ac997-138">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="ac997-138">SetRuleOperation</span></span>](setruleoperation.md) <br/> |<span data-ttu-id="ac997-139">Représente une opération de mise à jour d’une règle existante.</span><span class="sxs-lookup"><span data-stu-id="ac997-139">Represents an operation to update an existing rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ac997-140">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ac997-140">Text value</span></span>

<span data-ttu-id="ac997-141">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ac997-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ac997-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="ac997-142">Remarks</span></span>

<span data-ttu-id="ac997-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac997-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac997-144">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ac997-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac997-145">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ac997-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ac997-146">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ac997-146">Schema Name</span></span>  <br/> |<span data-ttu-id="ac997-147">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ac997-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="ac997-148">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ac997-148">Validation File</span></span>  <br/> |<span data-ttu-id="ac997-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ac997-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ac997-150">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ac997-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="ac997-151">True</span><span class="sxs-lookup"><span data-stu-id="ac997-151">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac997-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ac997-152">See also</span></span>



[<span data-ttu-id="ac997-153">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="ac997-153">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="ac997-154">SetRuleOperation</span><span class="sxs-lookup"><span data-stu-id="ac997-154">SetRuleOperation</span></span>](setruleoperation.md)
  
[<span data-ttu-id="ac997-155">CreateRuleOperation</span><span class="sxs-lookup"><span data-stu-id="ac997-155">CreateRuleOperation</span></span>](createruleoperation.md)


- [<span data-ttu-id="ac997-156">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ac997-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

