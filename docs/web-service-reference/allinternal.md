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
description: L’élément AllInternal renvoie la valeur true si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.
ms.openlocfilehash: c5ffe15eca5d680994acb62913ebf5effacce214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464832"
---
# <a name="allinternal"></a><span data-ttu-id="bf579-103">AllInternal</span><span class="sxs-lookup"><span data-stu-id="bf579-103">AllInternal</span></span>

<span data-ttu-id="bf579-104">L’élément **AllInternal** renvoie la **valeur true** si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="bf579-104">The **AllInternal** element evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span> 
  
```xml
<AllInternal/>
```

 <span data-ttu-id="bf579-105">**ProtectionRuleAllInternalType**</span><span class="sxs-lookup"><span data-stu-id="bf579-105">**ProtectionRuleAllInternalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bf579-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bf579-106">Attributes and elements</span></span>

<span data-ttu-id="bf579-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bf579-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf579-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="bf579-108">Attributes</span></span>

<span data-ttu-id="bf579-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bf579-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf579-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bf579-110">Child elements</span></span>

<span data-ttu-id="bf579-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bf579-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bf579-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bf579-112">Parent elements</span></span>

|<span data-ttu-id="bf579-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bf579-113">**Element**</span></span>|<span data-ttu-id="bf579-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="bf579-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf579-115">Condition</span><span class="sxs-lookup"><span data-stu-id="bf579-115">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="bf579-116">Identifie la condition qui doit être remplie pour que la partie action de la règle soit exécutée.</span><span class="sxs-lookup"><span data-stu-id="bf579-116">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="bf579-117">Et (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="bf579-117">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="bf579-118">Spécifie que tous les éléments enfants doivent correspondre pour avoir la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="bf579-118">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bf579-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="bf579-119">Text value</span></span>

<span data-ttu-id="bf579-120">L’élément **AllInternal** doit être vide.</span><span class="sxs-lookup"><span data-stu-id="bf579-120">The **AllInternal** element must be empty.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bf579-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="bf579-121">Remarks</span></span>

<span data-ttu-id="bf579-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf579-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf579-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bf579-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf579-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bf579-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf579-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bf579-125">Schema Name</span></span>  <br/> |<span data-ttu-id="bf579-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bf579-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="bf579-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bf579-127">Validation File</span></span>  <br/> |<span data-ttu-id="bf579-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bf579-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf579-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bf579-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="bf579-130">False</span><span class="sxs-lookup"><span data-stu-id="bf579-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf579-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bf579-131">See also</span></span>

- [<span data-ttu-id="bf579-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="bf579-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

