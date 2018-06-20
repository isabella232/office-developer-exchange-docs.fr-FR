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
ms.openlocfilehash: ed605946f99aa63416337cd0e731c931176a8ed4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755531"
---
# <a name="condition"></a><span data-ttu-id="315f2-103">Condition</span><span class="sxs-lookup"><span data-stu-id="315f2-103">Condition</span></span>

<span data-ttu-id="315f2-104">L’élément **Condition** identifie la condition qui doit être remplie pour la partie de l’action de la règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="315f2-104">The **Condition** element identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span> 
  
```xml
<Condition>
   <AllInternal/>
</Condition>
```

 <span data-ttu-id="315f2-105">**ProtectionRuleConditionType**</span><span class="sxs-lookup"><span data-stu-id="315f2-105">**ProtectionRuleConditionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="315f2-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="315f2-106">Attributes and elements</span></span>

<span data-ttu-id="315f2-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="315f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="315f2-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="315f2-108">Attributes</span></span>

<span data-ttu-id="315f2-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="315f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="315f2-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="315f2-110">Child elements</span></span>

|<span data-ttu-id="315f2-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="315f2-111">**Element**</span></span>|<span data-ttu-id="315f2-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="315f2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="315f2-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="315f2-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="315f2-114">Renvoie **la valeur true** si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="315f2-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|[<span data-ttu-id="315f2-115">Et (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="315f2-115">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="315f2-116">Spécifie que tous les éléments enfants doivent correspondre pour prendre la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="315f2-116">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="315f2-117">Spécifie qu’il doit y avoir plusieurs conditions d’enfants de règle de protection.</span><span class="sxs-lookup"><span data-stu-id="315f2-117">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
|[<span data-ttu-id="315f2-118">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="315f2-118">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="315f2-119">Spécifie que n’importe quel destinataire du message électronique correspond à un des destinataires spécifiés dans les éléments de [valeur (ProtectionRuleValueType)](value-protectionrulevaluetype.md) enfants.</span><span class="sxs-lookup"><span data-stu-id="315f2-119">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="315f2-120">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="315f2-120">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="315f2-121">Spécifie que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de [valeur (ProtectionRuleValueType)](value-protectionrulevaluetype.md) enfants.</span><span class="sxs-lookup"><span data-stu-id="315f2-121">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="315f2-122">True</span><span class="sxs-lookup"><span data-stu-id="315f2-122">True</span></span>](true.md) <br/> |<span data-ttu-id="315f2-123">Spécifie une condition qui correspond toujours.</span><span class="sxs-lookup"><span data-stu-id="315f2-123">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="315f2-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="315f2-124">Parent elements</span></span>

|<span data-ttu-id="315f2-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="315f2-125">**Element**</span></span>|<span data-ttu-id="315f2-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="315f2-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="315f2-127">Règle</span><span class="sxs-lookup"><span data-stu-id="315f2-127">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="315f2-128">Contient une règle de protection unique.</span><span class="sxs-lookup"><span data-stu-id="315f2-128">Contains a single protection rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="315f2-129">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="315f2-129">Text value</span></span>

<span data-ttu-id="315f2-130">Aucun.</span><span class="sxs-lookup"><span data-stu-id="315f2-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="315f2-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="315f2-131">Remarks</span></span>

<span data-ttu-id="315f2-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="315f2-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="315f2-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="315f2-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="315f2-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="315f2-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="315f2-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="315f2-135">Schema Name</span></span>  <br/> |<span data-ttu-id="315f2-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="315f2-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="315f2-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="315f2-137">Validation File</span></span>  <br/> |<span data-ttu-id="315f2-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="315f2-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="315f2-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="315f2-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="315f2-140">False</span><span class="sxs-lookup"><span data-stu-id="315f2-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="315f2-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="315f2-141">See also</span></span>



- [<span data-ttu-id="315f2-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="315f2-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

