---
title: StopProcessingRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StopProcessingRules
api_type:
- schema
ms.assetid: 5b89a2cb-ab26-444d-b3dd-2b3858872d63
description: L'élément StopProcessingRules indique si les règles suivantes doivent être évaluées.
ms.openlocfilehash: 9f068fd6290a39bbab6e3c1e29066c4fefefc64b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467899"
---
# <a name="stopprocessingrules"></a><span data-ttu-id="7b300-103">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="7b300-103">StopProcessingRules</span></span>

<span data-ttu-id="7b300-104">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **StopProcessingRules** indique si les règles suivantes doivent être évaluées.</span><span class="sxs-lookup"><span data-stu-id="7b300-104">The **StopProcessingRules** element indicates whether subsequent rules are to be evaluated.</span></span> 
  
```XML
<StopProcessingRules>true | false</StopProcessingRules>
```

 <span data-ttu-id="7b300-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7b300-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b300-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7b300-106">Attributes and elements</span></span>

<span data-ttu-id="7b300-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7b300-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b300-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7b300-108">Attributes</span></span>

<span data-ttu-id="7b300-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="7b300-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b300-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7b300-110">Child elements</span></span>

<span data-ttu-id="7b300-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7b300-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7b300-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7b300-112">Parent elements</span></span>

|<span data-ttu-id="7b300-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7b300-113">**Element**</span></span>|<span data-ttu-id="7b300-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7b300-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b300-115">Actions</span><span class="sxs-lookup"><span data-stu-id="7b300-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="7b300-116">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="7b300-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7b300-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="7b300-117">Text value</span></span>

<span data-ttu-id="7b300-p101">Une valeur texte **true** indique que les règles suivantes ne doivent pas être traités. La valeur **false** indique que les règles suivantes devraient continuer à être évaluée.</span><span class="sxs-lookup"><span data-stu-id="7b300-p101">A text value of **true** indicates that subsequent rules should not be processed. A value of **false** indicates that subsequent rules should continue to be evaluated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7b300-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="7b300-120">Remarks</span></span>

<span data-ttu-id="7b300-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7b300-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b300-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7b300-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b300-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7b300-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7b300-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7b300-124">Schema Name</span></span>  <br/> |<span data-ttu-id="7b300-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7b300-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7b300-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7b300-126">Validation File</span></span>  <br/> |<span data-ttu-id="7b300-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7b300-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7b300-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7b300-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="7b300-129">True</span><span class="sxs-lookup"><span data-stu-id="7b300-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b300-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7b300-130">See also</span></span>



- [<span data-ttu-id="7b300-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7b300-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

