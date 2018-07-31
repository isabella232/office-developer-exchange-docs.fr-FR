---
title: Condition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Condition
api_type:
- schema
ms.assetid: 0790a3f2-cb31-4036-a757-7821aa0722cb
description: L’élément Condition identifie la condition qui doit être remplie pour la partie de l’action de la règle doit être exécutée.
ms.openlocfilehash: d49f2984799b15c0499af59abecbb34abe15f7c3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353559"
---
# <a name="condition"></a><span data-ttu-id="bc7dc-103">Condition</span><span class="sxs-lookup"><span data-stu-id="bc7dc-103">Condition</span></span>

<span data-ttu-id="bc7dc-104">L’élément **Condition** identifie la condition qui doit être remplie pour la partie de l’action de la règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-104">The **Condition** element identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span> 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

```xml
<Condition> 
    <SenderDepartments/> 
</Condition>
```

```xml
<Condition> 
    <True/> 
</Condition>
```

```xml
<Condition> 
    <Recipients/> 
</Condition>
```

```xml
<Condition> 
    <And/> 
</Condition>
```

<span data-ttu-id="bc7dc-105">**ProtectionRuleConditionType**</span><span class="sxs-lookup"><span data-stu-id="bc7dc-105">**ProtectionRuleConditionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bc7dc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bc7dc-106">Attributes and elements</span></span>

<span data-ttu-id="bc7dc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc7dc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bc7dc-108">Attributes</span></span>

<span data-ttu-id="bc7dc-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc7dc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bc7dc-110">Child elements</span></span>

|<span data-ttu-id="bc7dc-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bc7dc-111">**Element**</span></span>|<span data-ttu-id="bc7dc-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="bc7dc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc7dc-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="bc7dc-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="bc7dc-114">Renvoie **la valeur true** si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|[<span data-ttu-id="bc7dc-115">And (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="bc7dc-115">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="bc7dc-116">Spécifie que tous les éléments enfants doivent correspondre pour prendre la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-116">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="bc7dc-117">Spécifie qu’il doit y avoir plusieurs conditions d’enfants de règle de protection.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-117">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
|[<span data-ttu-id="bc7dc-118">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="bc7dc-118">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="bc7dc-119">Spécifie que n’importe quel destinataire du message électronique correspond à un des destinataires spécifiés dans les éléments de [valeur (ProtectionRuleValueType)](value-protectionrulevaluetype.md) enfants.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-119">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="bc7dc-120">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="bc7dc-120">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="bc7dc-121">Spécifie que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de [valeur (ProtectionRuleValueType)](value-protectionrulevaluetype.md) enfants.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-121">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="bc7dc-122">True</span><span class="sxs-lookup"><span data-stu-id="bc7dc-122">True</span></span>](true.md) <br/> |<span data-ttu-id="bc7dc-123">Spécifie une condition qui correspond toujours.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-123">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc7dc-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bc7dc-124">Parent elements</span></span>

|<span data-ttu-id="bc7dc-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bc7dc-125">**Element**</span></span>|<span data-ttu-id="bc7dc-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="bc7dc-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc7dc-127">Règle</span><span class="sxs-lookup"><span data-stu-id="bc7dc-127">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="bc7dc-128">Contient une règle de protection unique.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-128">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc7dc-129">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="bc7dc-129">Text value</span></span>

<span data-ttu-id="bc7dc-130">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bc7dc-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="bc7dc-131">Remarks</span></span>

<span data-ttu-id="bc7dc-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc7dc-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc7dc-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bc7dc-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc7dc-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bc7dc-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bc7dc-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bc7dc-135">Schema Name</span></span>  <br/> |<span data-ttu-id="bc7dc-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bc7dc-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="bc7dc-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bc7dc-137">Validation File</span></span>  <br/> |<span data-ttu-id="bc7dc-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bc7dc-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bc7dc-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bc7dc-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc7dc-140">False</span><span class="sxs-lookup"><span data-stu-id="bc7dc-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc7dc-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bc7dc-141">See also</span></span>

- [<span data-ttu-id="bc7dc-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bc7dc-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

