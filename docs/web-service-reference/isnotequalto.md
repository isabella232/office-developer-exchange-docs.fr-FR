---
title: IsNotEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotEqualTo
api_type:
- schema
ms.assetid: e2eff26c-3403-45cd-bb74-1eb98c7dbfcd
description: L’élément IsNotEqualTo représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur true si les valeurs ne sont pas identiques.
ms.openlocfilehash: 75b580d97fbadbf3aa28c29159973f53768df624
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353251"
---
# <a name="isnotequalto"></a><span data-ttu-id="4a51b-103">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="4a51b-103">IsNotEqualTo</span></span>

<span data-ttu-id="4a51b-104">L’élément **IsNotEqualTo** représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **la valeur true** si les valeurs ne sont pas identiques.</span><span class="sxs-lookup"><span data-stu-id="4a51b-104">The **IsNotEqualTo** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span> 
  
```xml
<IsNotEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

```xml
<IsNotEqualTo>
   <ExtendedFieldURI/> 
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

```xml
<IsNotEqualTo>
   <IndexedFieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

<span data-ttu-id="4a51b-105">**IsNotEqualToType**</span><span class="sxs-lookup"><span data-stu-id="4a51b-105">**IsNotEqualToType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4a51b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4a51b-106">Attributes and elements</span></span>

<span data-ttu-id="4a51b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4a51b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a51b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4a51b-108">Attributes</span></span>

<span data-ttu-id="4a51b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4a51b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a51b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4a51b-110">Child elements</span></span>

|<span data-ttu-id="4a51b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a51b-111">**Element**</span></span>|<span data-ttu-id="4a51b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a51b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a51b-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="4a51b-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="4a51b-114">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="4a51b-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="4a51b-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="4a51b-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="4a51b-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="4a51b-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="4a51b-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="4a51b-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="4a51b-118">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="4a51b-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="4a51b-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="4a51b-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="4a51b-120">Représente une propriété ou une constante à utiliser lors de la comparaison avec une autre propriété.</span><span class="sxs-lookup"><span data-stu-id="4a51b-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4a51b-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4a51b-121">Parent elements</span></span>

|<span data-ttu-id="4a51b-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4a51b-122">**Element**</span></span>|<span data-ttu-id="4a51b-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="4a51b-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a51b-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="4a51b-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="4a51b-125">Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.</span><span class="sxs-lookup"><span data-stu-id="4a51b-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="4a51b-126">Pas</span><span class="sxs-lookup"><span data-stu-id="4a51b-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="4a51b-127">Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="4a51b-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="4a51b-128">And</span><span class="sxs-lookup"><span data-stu-id="4a51b-128">And</span></span>](and.md) <br/> |<span data-ttu-id="4a51b-129">Représente une expression de recherche qui vous permet d’effectuer une opération de type Boolean et entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="4a51b-129">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="4a51b-130">Le résultat de l’opération est **la valeur true** si toutes les expressions de recherche contenues dans l’And sont **remplies**.</span><span class="sxs-lookup"><span data-stu-id="4a51b-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="4a51b-131">Or</span><span class="sxs-lookup"><span data-stu-id="4a51b-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="4a51b-132">Représente une expression de recherche qui effectue une opération OR logique sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="4a51b-132">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="4a51b-133">[Ou](or.md) renvoie **la valeur true** si un de ses enfants retourne **true**.</span><span class="sxs-lookup"><span data-stu-id="4a51b-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="4a51b-134">**Ou** doit disposer de deux ou plusieurs enfants.</span><span class="sxs-lookup"><span data-stu-id="4a51b-134">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4a51b-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="4a51b-135">Remarks</span></span>

<span data-ttu-id="4a51b-136">Pour effectuer des comparaisons de chaînes, envisagez d’utiliser l’élément [contient](contains.md) , car elle fournit des options pour les paramètres correspondants tels que la casse et les espaces.</span><span class="sxs-lookup"><span data-stu-id="4a51b-136">To perform string comparisons, consider using the [Contains](contains.md) element, as it provides options for matching parameters such as case and white space.</span></span> <span data-ttu-id="4a51b-137">Utilisez l’élément [pas](not.md) en association avec l’élément [contient](contains.md) pour inverser le résultat.</span><span class="sxs-lookup"><span data-stu-id="4a51b-137">Use the [Not](not.md) element in conjunction with the [Contains](contains.md) element to negate the result.</span></span> 
  
<span data-ttu-id="4a51b-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4a51b-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a51b-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4a51b-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a51b-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4a51b-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a51b-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4a51b-141">Schema Name</span></span>  <br/> |<span data-ttu-id="4a51b-142">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4a51b-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="4a51b-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4a51b-143">Validation File</span></span>  <br/> |<span data-ttu-id="4a51b-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4a51b-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a51b-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4a51b-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a51b-146">False</span><span class="sxs-lookup"><span data-stu-id="4a51b-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a51b-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4a51b-147">See also</span></span>

- [<span data-ttu-id="4a51b-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4a51b-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

