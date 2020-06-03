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
description: L’élément condition identifie la condition qui doit être remplie pour que la partie action de la règle s’exécute.
ms.openlocfilehash: 2aea11197f072a4dbe21292bb47075d6f273d31b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463222"
---
# <a name="condition"></a><span data-ttu-id="893c5-103">Condition</span><span class="sxs-lookup"><span data-stu-id="893c5-103">Condition</span></span>

<span data-ttu-id="893c5-104">L’élément **condition** identifie la condition qui doit être remplie pour que la partie action de la règle s’exécute.</span><span class="sxs-lookup"><span data-stu-id="893c5-104">The **Condition** element identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span> 
  
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

<span data-ttu-id="893c5-105">**ProtectionRuleConditionType**</span><span class="sxs-lookup"><span data-stu-id="893c5-105">**ProtectionRuleConditionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="893c5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="893c5-106">Attributes and elements</span></span>

<span data-ttu-id="893c5-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="893c5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="893c5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="893c5-108">Attributes</span></span>

<span data-ttu-id="893c5-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="893c5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="893c5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="893c5-110">Child elements</span></span>

|<span data-ttu-id="893c5-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="893c5-111">**Element**</span></span>|<span data-ttu-id="893c5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="893c5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="893c5-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="893c5-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="893c5-114">Renvoie la **valeur true** si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="893c5-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|[<span data-ttu-id="893c5-115">Et (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="893c5-115">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="893c5-116">Spécifie que tous les éléments enfants doivent correspondre pour avoir la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="893c5-116">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="893c5-117">Spécifie qu’il doit y avoir plus d’une condition de règle de protection enfant.</span><span class="sxs-lookup"><span data-stu-id="893c5-117">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
|[<span data-ttu-id="893c5-118">Destinataireest</span><span class="sxs-lookup"><span data-stu-id="893c5-118">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="893c5-119">Spécifie que tout destinataire du message électronique correspond à l’un des destinataires spécifiés dans les éléments de [valeur enfant (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="893c5-119">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="893c5-120">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="893c5-120">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="893c5-121">Indique que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de [valeur enfant (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="893c5-121">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="893c5-122">True</span><span class="sxs-lookup"><span data-stu-id="893c5-122">True</span></span>](true.md) <br/> |<span data-ttu-id="893c5-123">Spécifie une condition qui correspond toujours à.</span><span class="sxs-lookup"><span data-stu-id="893c5-123">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="893c5-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="893c5-124">Parent elements</span></span>

|<span data-ttu-id="893c5-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="893c5-125">**Element**</span></span>|<span data-ttu-id="893c5-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="893c5-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="893c5-127">Règle</span><span class="sxs-lookup"><span data-stu-id="893c5-127">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="893c5-128">Contient une règle de protection unique.</span><span class="sxs-lookup"><span data-stu-id="893c5-128">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="893c5-129">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="893c5-129">Text value</span></span>

<span data-ttu-id="893c5-130">Aucun.</span><span class="sxs-lookup"><span data-stu-id="893c5-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="893c5-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="893c5-131">Remarks</span></span>

<span data-ttu-id="893c5-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="893c5-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="893c5-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="893c5-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="893c5-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="893c5-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="893c5-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="893c5-135">Schema Name</span></span>  <br/> |<span data-ttu-id="893c5-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="893c5-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="893c5-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="893c5-137">Validation File</span></span>  <br/> |<span data-ttu-id="893c5-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="893c5-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="893c5-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="893c5-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="893c5-140">False</span><span class="sxs-lookup"><span data-stu-id="893c5-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="893c5-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="893c5-141">See also</span></span>

- [<span data-ttu-id="893c5-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="893c5-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

