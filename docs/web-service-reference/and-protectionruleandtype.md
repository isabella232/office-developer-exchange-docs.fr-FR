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
description: L’élément and spécifie que tous les éléments enfants doivent correspondre pour avoir la valeur true.
ms.openlocfilehash: ba898ccd77518971afaf713d1c7c7955f46465d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464734"
---
# <a name="and-protectionruleandtype"></a><span data-ttu-id="6dba0-103">Et (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="6dba0-103">And (ProtectionRuleAndType)</span></span>

<span data-ttu-id="6dba0-104">L’élément **and** spécifie que tous les éléments enfants doivent correspondre pour avoir la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="6dba0-104">The **And** element specifies that all child elements must match to evaluate to **true**.</span></span>
  
```xml
<And>
   <AllInternal/>
   <And/>
   <RecipientIs/>
   <SenderDepartments/>
   <True/>
</And>
```

 <span data-ttu-id="6dba0-105">**ProtectionRuleAndType**</span><span class="sxs-lookup"><span data-stu-id="6dba0-105">**ProtectionRuleAndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6dba0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6dba0-106">Attributes and elements</span></span>

<span data-ttu-id="6dba0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6dba0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6dba0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6dba0-108">Attributes</span></span>

<span data-ttu-id="6dba0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6dba0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6dba0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6dba0-110">Child elements</span></span>

|<span data-ttu-id="6dba0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6dba0-111">**Element**</span></span>|<span data-ttu-id="6dba0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="6dba0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6dba0-113">AllInternal</span><span class="sxs-lookup"><span data-stu-id="6dba0-113">AllInternal</span></span>](allinternal.md) <br/> |<span data-ttu-id="6dba0-114">Renvoie la **valeur true** si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="6dba0-114">Evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span>  <br/> |
|<span data-ttu-id="6dba0-115">**And**</span><span class="sxs-lookup"><span data-stu-id="6dba0-115">**And**</span></span> <br/> |<span data-ttu-id="6dba0-116">Spécifie que tous les éléments enfants doivent correspondre pour avoir la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="6dba0-116">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
|[<span data-ttu-id="6dba0-117">Destinataireest</span><span class="sxs-lookup"><span data-stu-id="6dba0-117">RecipientIs</span></span>](recipientis.md) <br/> |<span data-ttu-id="6dba0-118">Spécifie que tout destinataire du message électronique correspond à l’un des destinataires spécifiés dans les éléments de [valeur enfant (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="6dba0-118">Specifies that any recipient of the e-mail message matches any of the specified recipients in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="6dba0-119">SenderDepartments</span><span class="sxs-lookup"><span data-stu-id="6dba0-119">SenderDepartments</span></span>](senderdepartments.md) <br/> |<span data-ttu-id="6dba0-120">Indique que le service de l’expéditeur correspond à l’un des services spécifiés dans les éléments de [valeur enfant (ProtectionRuleValueType)](value-protectionrulevaluetype.md) .</span><span class="sxs-lookup"><span data-stu-id="6dba0-120">Specifies that the department of the sender matches any of the specified departments in the child [Value (ProtectionRuleValueType)](value-protectionrulevaluetype.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="6dba0-121">True</span><span class="sxs-lookup"><span data-stu-id="6dba0-121">True</span></span>](true.md) <br/> |<span data-ttu-id="6dba0-122">Spécifie une condition qui correspond toujours à.</span><span class="sxs-lookup"><span data-stu-id="6dba0-122">Specifies a condition that always matches.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6dba0-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6dba0-123">Parent elements</span></span>

|<span data-ttu-id="6dba0-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6dba0-124">**Element**</span></span>|<span data-ttu-id="6dba0-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="6dba0-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6dba0-126">Condition</span><span class="sxs-lookup"><span data-stu-id="6dba0-126">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="6dba0-127">Identifie la condition qui doit être remplie pour que la partie action de la règle soit exécutée.</span><span class="sxs-lookup"><span data-stu-id="6dba0-127">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|<span data-ttu-id="6dba0-128">**And**</span><span class="sxs-lookup"><span data-stu-id="6dba0-128">**And**</span></span> <br/> |<span data-ttu-id="6dba0-129">Spécifie que tous les éléments enfants doivent correspondre pour avoir la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="6dba0-129">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6dba0-130">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6dba0-130">Text value</span></span>

<span data-ttu-id="6dba0-131">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6dba0-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6dba0-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="6dba0-132">Remarks</span></span>

<span data-ttu-id="6dba0-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dba0-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6dba0-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6dba0-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6dba0-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6dba0-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6dba0-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6dba0-136">Schema Name</span></span>  <br/> |<span data-ttu-id="6dba0-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6dba0-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="6dba0-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6dba0-138">Validation File</span></span>  <br/> |<span data-ttu-id="6dba0-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6dba0-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6dba0-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6dba0-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="6dba0-141">False</span><span class="sxs-lookup"><span data-stu-id="6dba0-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6dba0-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6dba0-142">See also</span></span>

- [<span data-ttu-id="6dba0-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6dba0-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

