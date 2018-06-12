---
title: AssignCategories
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssignCategories
api_type:
- schema
ms.assetid: f5c73fed-7b00-446d-8296-71a0c86e7fc6
description: L’élément AssignCategories représente les catégories qui sont marqués dans les messages électroniques.
ms.openlocfilehash: 96c77306d649677c1be745e8cadc2886e4a84c8a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755325"
---
# <a name="assigncategories"></a><span data-ttu-id="d4065-103">AssignCategories</span><span class="sxs-lookup"><span data-stu-id="d4065-103">AssignCategories</span></span>

<span data-ttu-id="d4065-104">L’élément **AssignCategories** représente les catégories qui sont marqués dans les messages électroniques.</span><span class="sxs-lookup"><span data-stu-id="d4065-104">The **AssignCategories** element represents the categories that are stamped on e-mail messages.</span></span> 
  
- [<span data-ttu-id="d4065-105">Règle (RuleType)</span><span class="sxs-lookup"><span data-stu-id="d4065-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
- [<span data-ttu-id="d4065-106">Actions</span><span class="sxs-lookup"><span data-stu-id="d4065-106">Actions</span></span>](actions.md)
  
```XML
<AssignCategories>
   <String/>
</AssignCategories>
```

 <span data-ttu-id="d4065-107">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="d4065-107">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4065-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d4065-108">Attributes and elements</span></span>

<span data-ttu-id="d4065-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d4065-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4065-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d4065-110">Attributes</span></span>

<span data-ttu-id="d4065-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4065-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4065-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d4065-112">Child elements</span></span>

|<span data-ttu-id="d4065-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4065-113">**Element**</span></span>|<span data-ttu-id="d4065-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4065-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4065-115">String</span><span class="sxs-lookup"><span data-stu-id="d4065-115">String</span></span>](string.md) <br/> |<span data-ttu-id="d4065-116">Contient une chaîne qui identifie une seule catégorie.</span><span class="sxs-lookup"><span data-stu-id="d4065-116">Contains a string that identifies a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4065-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d4065-117">Parent elements</span></span>

|<span data-ttu-id="d4065-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4065-118">**Element**</span></span>|<span data-ttu-id="d4065-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4065-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4065-120">Actions</span><span class="sxs-lookup"><span data-stu-id="d4065-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="d4065-121">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="d4065-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d4065-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d4065-122">Text value</span></span>

<span data-ttu-id="d4065-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d4065-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d4065-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="d4065-124">Remarks</span></span>

<span data-ttu-id="d4065-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d4065-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4065-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d4065-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4065-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d4065-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d4065-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d4065-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d4065-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d4065-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d4065-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d4065-130">Validation File</span></span>  <br/> |<span data-ttu-id="d4065-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d4065-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d4065-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d4065-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4065-133">True</span><span class="sxs-lookup"><span data-stu-id="d4065-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4065-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4065-134">See also</span></span>

- [<span data-ttu-id="d4065-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d4065-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
