---
title: SenderDepartments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderDepartments
api_type:
- schema
ms.assetid: b016cdde-d597-40ac-87c4-63ca68bd539d
description: L’élément SenderDepartments indique que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de valeur (ProtectionRuleValueType) enfants.
ms.openlocfilehash: d40e6299bd46ede559cc2cce3bcc9d1611e96bd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829331"
---
# <a name="senderdepartments"></a><span data-ttu-id="f7b49-103">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="f7b49-103">SenderDepartments</span></span>

<span data-ttu-id="f7b49-104">L’élément **SenderDepartments** indique que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de [valeur (ProtectionRuleValueType)](value-protectionrulevaluetype.md) enfants.</span><span class="sxs-lookup"><span data-stu-id="f7b49-104">The **SenderDepartments** element specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span> 
  
```XML
<SenderDepartments>
   <Value/>
</SenderDepartments>
```

 <span data-ttu-id="f7b49-105">**ProtectionRuleSenderDepartmentsType**</span><span class="sxs-lookup"><span data-stu-id="f7b49-105">**ProtectionRuleSenderDepartmentsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7b49-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f7b49-106">Attributes and elements</span></span>

<span data-ttu-id="f7b49-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f7b49-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7b49-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f7b49-108">Attributes</span></span>

<span data-ttu-id="f7b49-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f7b49-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7b49-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f7b49-110">Child elements</span></span>

|<span data-ttu-id="f7b49-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7b49-111">**Element**</span></span>|<span data-ttu-id="f7b49-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7b49-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7b49-113">Valeur (ProtectionRuleValueType)</span><span class="sxs-lookup"><span data-stu-id="f7b49-113">Value (ProtectionRuleValueType)</span></span>](value-protectionrulevaluetype.md) <br/> |<span data-ttu-id="f7b49-114">Identifie un service unique de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="f7b49-114">Identifies a single sender department.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7b49-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f7b49-115">Parent elements</span></span>

|<span data-ttu-id="f7b49-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f7b49-116">**Element**</span></span>|<span data-ttu-id="f7b49-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="f7b49-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7b49-118">Condition</span><span class="sxs-lookup"><span data-stu-id="f7b49-118">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="f7b49-119">Identifie la condition qui doit être remplie pour la partie de l’action de la règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="f7b49-119">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="f7b49-120">Et (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="f7b49-120">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="f7b49-121">Spécifie que tous les éléments enfants doivent correspondre pour prendre la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="f7b49-121">Specifies that all child elements must match to evaluate to **true**.</span></span> <span data-ttu-id="f7b49-122">Spécifie qu’il doit y avoir plusieurs conditions d’enfants de règle de protection.</span><span class="sxs-lookup"><span data-stu-id="f7b49-122">Specifies that there must be more than one protection rule child condition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f7b49-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="f7b49-123">Remarks</span></span>

<span data-ttu-id="f7b49-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7b49-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7b49-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f7b49-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7b49-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f7b49-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7b49-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f7b49-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f7b49-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f7b49-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7b49-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f7b49-129">Validation File</span></span>  <br/> |<span data-ttu-id="f7b49-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f7b49-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7b49-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f7b49-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7b49-132">False</span><span class="sxs-lookup"><span data-stu-id="f7b49-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7b49-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f7b49-133">See also</span></span>



- [<span data-ttu-id="f7b49-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f7b49-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

