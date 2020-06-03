---
title: Constante
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Constant
api_type:
- schema
ms.assetid: 340af0cd-9f12-44ab-b8f1-21d107c8d0c9
description: L’élément constant identifie une valeur constante dans une restriction.
ms.openlocfilehash: 6cb2eaa4227a8fd0985e8ff5a15d647c3bb1cd6a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461554"
---
# <a name="constant"></a><span data-ttu-id="4324e-103">Constante</span><span class="sxs-lookup"><span data-stu-id="4324e-103">Constant</span></span>

<span data-ttu-id="4324e-104">L’élément **constant** identifie une valeur constante dans une restriction.</span><span class="sxs-lookup"><span data-stu-id="4324e-104">The **Constant** element identifies a constant value in a restriction.</span></span> 
  
```xml
<Constant Value="" />
```

 <span data-ttu-id="4324e-105">**ConstantValueType**</span><span class="sxs-lookup"><span data-stu-id="4324e-105">**ConstantValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4324e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4324e-106">Attributes and elements</span></span>

<span data-ttu-id="4324e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4324e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4324e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4324e-108">Attributes</span></span>

|<span data-ttu-id="4324e-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="4324e-109">**Attribute**</span></span>|<span data-ttu-id="4324e-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="4324e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4324e-111">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="4324e-111">**Value**</span></span> <br/> |<span data-ttu-id="4324e-112">Spécifie la valeur à comparer dans la restriction.</span><span class="sxs-lookup"><span data-stu-id="4324e-112">Specifies the value to compare in the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4324e-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4324e-113">Child elements</span></span>

<span data-ttu-id="4324e-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4324e-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4324e-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4324e-115">Parent elements</span></span>

|<span data-ttu-id="4324e-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4324e-116">**Element**</span></span>|<span data-ttu-id="4324e-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="4324e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4324e-118">Contains</span><span class="sxs-lookup"><span data-stu-id="4324e-118">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="4324e-119">Représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne de constante fournie.</span><span class="sxs-lookup"><span data-stu-id="4324e-119">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="4324e-120">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="4324e-120">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="4324e-121">Représente une propriété ou une valeur constante à utiliser lors de la comparaison avec une autre propriété.</span><span class="sxs-lookup"><span data-stu-id="4324e-121">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4324e-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="4324e-122">Remarks</span></span>

<span data-ttu-id="4324e-123">La valeur de chaîne dans l’attribut **value** doit pouvoir être forcée dans le type avec lequel vous essayez de comparer.</span><span class="sxs-lookup"><span data-stu-id="4324e-123">The string value in the **Value** attribute must be coercible into the type you are trying to compare against.</span></span> <span data-ttu-id="4324e-124">Par exemple, si vous comparez une propriété de date/heure à une valeur de constante, la valeur de chaîne doit représenter une date/heure.</span><span class="sxs-lookup"><span data-stu-id="4324e-124">For example, if you are comparing a date/time property against a constant value, the string value must represent a date/time.</span></span> 
  
<span data-ttu-id="4324e-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4324e-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4324e-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4324e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4324e-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4324e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4324e-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4324e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="4324e-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4324e-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="4324e-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4324e-130">Validation File</span></span>  <br/> |<span data-ttu-id="4324e-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4324e-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4324e-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4324e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="4324e-133">False</span><span class="sxs-lookup"><span data-stu-id="4324e-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4324e-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4324e-134">See also</span></span>



- [<span data-ttu-id="4324e-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4324e-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

