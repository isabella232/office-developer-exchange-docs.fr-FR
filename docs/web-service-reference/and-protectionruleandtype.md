---
title: Et (ProtectionRuleAndType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 7fafd1c8-cd29-43a0-b383-f6595f934f48
description: L’élément et spécifie que tous les éléments enfants doivent correspondre pour renvoyer la valeur true.
ms.openlocfilehash: 9e0128ee3fa2b6ffdc5975946694475afec53c25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755205"
---
# <a name="and-protectionruleandtype"></a><span data-ttu-id="79474-103">Et (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="79474-103">And (ProtectionRuleAndType)</span></span>

<span data-ttu-id="79474-104">L’élément **et** Spécifie que tous les éléments enfants doivent correspondre pour prendre la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="79474-104">The **And** element specifies that all child elements must match to evaluate to **true**.</span></span>
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 <span data-ttu-id="79474-105">**ProtectionRuleAndType**</span><span class="sxs-lookup"><span data-stu-id="79474-105">**ProtectionRuleAndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79474-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="79474-106">Attributes and elements</span></span>

<span data-ttu-id="79474-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="79474-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79474-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="79474-108">Attributes</span></span>

<span data-ttu-id="79474-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79474-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79474-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="79474-110">Child elements</span></span>

|<span data-ttu-id="79474-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="79474-111">**Element**</span></span>|<span data-ttu-id="79474-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="79474-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79474-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="79474-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="79474-114">Renvoie **la valeur true** si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="79474-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|<span data-ttu-id="79474-115">**And**</span><span class="sxs-lookup"><span data-stu-id="79474-115">**And**</span></span> <br/> |<span data-ttu-id="79474-116">Spécifie que tous les éléments enfants doivent correspondre pour prendre la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="79474-116">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
|[<span data-ttu-id="79474-117">RecipientIs</span><span class="sxs-lookup"><span data-stu-id="79474-117">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="79474-118">Spécifie que n’importe quel destinataire du message électronique correspond à un des destinataires spécifiés dans les éléments de [valeur (ProtectionRuleValueType)](value-protectionrulevaluetype.md) enfants.</span><span class="sxs-lookup"><span data-stu-id="79474-118">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="79474-119">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="79474-119">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="79474-120">Spécifie que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de [valeur (ProtectionRuleValueType)](value-protectionrulevaluetype.md) enfants.</span><span class="sxs-lookup"><span data-stu-id="79474-120">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="79474-121">True</span><span class="sxs-lookup"><span data-stu-id="79474-121">True</span></span>](true.md) <br/> |<span data-ttu-id="79474-122">Spécifie une condition qui correspond toujours.</span><span class="sxs-lookup"><span data-stu-id="79474-122">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="79474-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="79474-123">Parent elements</span></span>

|<span data-ttu-id="79474-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="79474-124">**Element**</span></span>|<span data-ttu-id="79474-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="79474-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79474-126">Condition</span><span class="sxs-lookup"><span data-stu-id="79474-126">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="79474-127">Identifie la condition qui doit être remplie pour la partie de l’action de la règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="79474-127">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|<span data-ttu-id="79474-128">**And**</span><span class="sxs-lookup"><span data-stu-id="79474-128">**And**</span></span> <br/> |<span data-ttu-id="79474-129">Spécifie que tous les éléments enfants doivent correspondre pour prendre la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="79474-129">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79474-130">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="79474-130">Text value</span></span>

<span data-ttu-id="79474-131">Aucun.</span><span class="sxs-lookup"><span data-stu-id="79474-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="79474-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="79474-132">Remarks</span></span>

<span data-ttu-id="79474-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="79474-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79474-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="79474-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79474-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="79474-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79474-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="79474-136">Schema Name</span></span>  <br/> |<span data-ttu-id="79474-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="79474-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="79474-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="79474-138">Validation File</span></span>  <br/> |<span data-ttu-id="79474-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="79474-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79474-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="79474-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="79474-141">False</span><span class="sxs-lookup"><span data-stu-id="79474-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79474-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="79474-142">See also</span></span>

- [<span data-ttu-id="79474-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="79474-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

