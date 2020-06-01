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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464832"
---
# <a name="allinternal"></a><span data-ttu-id="ab090-103">AllInternal</span><span class="sxs-lookup"><span data-stu-id="ab090-103">AllInternal</span></span>

<span data-ttu-id="ab090-104">L’élément **AllInternal** renvoie la **valeur true** si tous les destinataires d’un message électronique sont internes à l’organisation de l’expéditeur.</span><span class="sxs-lookup"><span data-stu-id="ab090-104">The **AllInternal** element evaluates to **true** if all recipients of an e-mail message are internal to the sender's organization.</span></span> 
  
```xml
<AllInternal/>
```

 <span data-ttu-id="ab090-105">**ProtectionRuleAllInternalType**</span><span class="sxs-lookup"><span data-stu-id="ab090-105">**ProtectionRuleAllInternalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ab090-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ab090-106">Attributes and elements</span></span>

<span data-ttu-id="ab090-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ab090-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ab090-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ab090-108">Attributes</span></span>

<span data-ttu-id="ab090-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ab090-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ab090-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ab090-110">Child elements</span></span>

<span data-ttu-id="ab090-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ab090-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ab090-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ab090-112">Parent elements</span></span>

|<span data-ttu-id="ab090-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ab090-113">**Element**</span></span>|<span data-ttu-id="ab090-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ab090-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ab090-115">Condition</span><span class="sxs-lookup"><span data-stu-id="ab090-115">Condition</span></span>](condition.md) <br/> |<span data-ttu-id="ab090-116">Identifie la condition qui doit être remplie pour que la partie action de la règle soit exécutée.</span><span class="sxs-lookup"><span data-stu-id="ab090-116">Identifies the condition that must be satisfied for the action part of the rule to be executed.</span></span>  <br/> |
|[<span data-ttu-id="ab090-117">Et (ProtectionRuleAndType)</span><span class="sxs-lookup"><span data-stu-id="ab090-117">And (ProtectionRuleAndType)</span></span>](and-protectionruleandtype.md) <br/> |<span data-ttu-id="ab090-118">Spécifie que tous les éléments enfants doivent correspondre pour avoir la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="ab090-118">Specifies that all child elements must match to evaluate to **true**.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ab090-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ab090-119">Text value</span></span>

<span data-ttu-id="ab090-120">L’élément **AllInternal** doit être vide.</span><span class="sxs-lookup"><span data-stu-id="ab090-120">The **AllInternal** element must be empty.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ab090-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="ab090-121">Remarks</span></span>

<span data-ttu-id="ab090-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab090-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ab090-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ab090-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ab090-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ab090-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ab090-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ab090-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ab090-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ab090-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="ab090-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ab090-127">Validation File</span></span>  <br/> |<span data-ttu-id="ab090-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ab090-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ab090-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ab090-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ab090-130">False</span><span class="sxs-lookup"><span data-stu-id="ab090-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ab090-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ab090-131">See also</span></span>

- [<span data-ttu-id="ab090-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ab090-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

