---
title: AllInternal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllInternal
api_type:
- schema
ms.assetid: b7e5072f-5d9f-4ee0-b58b-4d75d878ea1c
description: L’élément AllInternal donne la valeur true si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.
ms.openlocfilehash: 0ffd4178e711e3117497eed682e3fd3e0594989b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755194"
---
# <a name="allinternal"></a><span data-ttu-id="4a0cc-103">AllInternal</span><span class="sxs-lookup"><span data-stu-id="4a0cc-103">AllInternal</span></span>

<span data-ttu-id="4a0cc-104">L’élément **AllInternal** renvoie **la valeur true** si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="4a0cc-104">The **AllInternal** element evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span> 
  
```xml
<AllInternal/>
```

 <span data-ttu-id="4a0cc-105">**ProtectionRuleAllInternalType**</span><span class="sxs-lookup"><span data-stu-id="4a0cc-105">**ProtectionRuleAllInternalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a0cc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4a0cc-106">Attributes and elements</span></span>

<span data-ttu-id="4a0cc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4a0cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a0cc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4a0cc-108">Attributes</span></span>

<span data-ttu-id="4a0cc-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4a0cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a0cc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4a0cc-110">Child elements</span></span>

<span data-ttu-id="4a0cc-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4a0cc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4a0cc-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4a0cc-112">Parent elements</span></span>

|<span data-ttu-id="4a0cc-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a0cc-113">**Element**</span></span>|<span data-ttu-id="4a0cc-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a0cc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a0cc-115">Condition</span><span class="sxs-lookup"><span data-stu-id="4a0cc-115">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="4a0cc-116">Identifie la condition qui doit être remplie pour la partie de l’action de la règle doit être exécutée.</span><span class="sxs-lookup"><span data-stu-id="4a0cc-116">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="4a0cc-117">Et (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="4a0cc-117">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="4a0cc-118">Spécifie que tous les éléments enfants doivent correspondre pour prendre la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="4a0cc-118">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a0cc-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4a0cc-119">Text value</span></span>

<span data-ttu-id="4a0cc-120">L’élément **AllInternal** doit être vide.</span><span class="sxs-lookup"><span data-stu-id="4a0cc-120">The **AllInternal** element must be empty.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4a0cc-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="4a0cc-121">Remarks</span></span>

<span data-ttu-id="4a0cc-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4a0cc-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a0cc-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4a0cc-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a0cc-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4a0cc-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a0cc-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4a0cc-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4a0cc-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4a0cc-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="4a0cc-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4a0cc-127">Validation File</span></span>  <br/> |<span data-ttu-id="4a0cc-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4a0cc-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a0cc-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4a0cc-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a0cc-130">False</span><span class="sxs-lookup"><span data-stu-id="4a0cc-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a0cc-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4a0cc-131">See also</span></span>

- [<span data-ttu-id="4a0cc-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4a0cc-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

