---
title: IsEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEqualTo
api_type:
- schema
ms.assetid: 48e7e067-049c-4184-8026-071e6f558e8a
description: L’élément IsEqualTo représente une expression de recherche qui compare une propriété à une valeur de constante ou à une autre propriété et donne la valeur true si elles sont égales.
ms.openlocfilehash: 857192443ab0520bb26ead399bc5364cc862a4fb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455295"
---
# <a name="isequalto"></a><span data-ttu-id="66882-103">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="66882-103">IsEqualTo</span></span>

<span data-ttu-id="66882-104">L’élément **IsEqualTo** représente une expression de recherche qui compare une propriété à une valeur de constante ou à une autre propriété et donne la valeur true si elles sont égales.</span><span class="sxs-lookup"><span data-stu-id="66882-104">The **IsEqualTo** element represents a search expression that compares a property with either a constant value or another property and evaluates to true if they are equal.</span></span> 
  
```xml
<IsEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

```xml
<IsEqualTo>
   <ExtendedFieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

```xml
<IsEqualTo>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsEqualTo>
```

<span data-ttu-id="66882-105">**IsEqualToType**</span><span class="sxs-lookup"><span data-stu-id="66882-105">**IsEqualToType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="66882-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="66882-106">Attributes and elements</span></span>

<span data-ttu-id="66882-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="66882-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66882-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="66882-108">Attributes</span></span>

<span data-ttu-id="66882-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="66882-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66882-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="66882-110">Child elements</span></span>

|<span data-ttu-id="66882-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="66882-111">**Element**</span></span>|<span data-ttu-id="66882-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="66882-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66882-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="66882-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="66882-114">Identifie les propriétés référencées fréquemment par URI.</span><span class="sxs-lookup"><span data-stu-id="66882-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="66882-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="66882-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="66882-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="66882-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="66882-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="66882-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="66882-118">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="66882-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="66882-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="66882-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="66882-120">Représente une propriété ou une valeur constante à utiliser lors de la comparaison avec une autre propriété.</span><span class="sxs-lookup"><span data-stu-id="66882-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="66882-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="66882-121">Parent elements</span></span>

|<span data-ttu-id="66882-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="66882-122">**Element**</span></span>|<span data-ttu-id="66882-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="66882-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66882-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="66882-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="66882-125">Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="66882-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="66882-126">Not</span><span class="sxs-lookup"><span data-stu-id="66882-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="66882-127">Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="66882-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="66882-128">And</span><span class="sxs-lookup"><span data-stu-id="66882-128">And</span></span>](and.md) <br/> |<span data-ttu-id="66882-129">Représente une expression de recherche qui vous permet d’effectuer une opération booléenne et une opération entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="66882-129">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="66882-130">Le résultat de l’opération and est **true** si toutes les expressions de recherche contenues dans le et sont **vraies**.</span><span class="sxs-lookup"><span data-stu-id="66882-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="66882-131">Or</span><span class="sxs-lookup"><span data-stu-id="66882-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="66882-132">Représente une expression de recherche qui effectue une ou logique sur l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="66882-132">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="66882-133">[Ou](or.md) renverra true si l’un de ses enfants renvoie la valeur true.</span><span class="sxs-lookup"><span data-stu-id="66882-133">[Or](or.md) will return true if any of its children return true.</span></span> <span data-ttu-id="66882-134">**Ou** il doit avoir au moins deux enfants.</span><span class="sxs-lookup"><span data-stu-id="66882-134">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="66882-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="66882-135">Remarks</span></span>

<span data-ttu-id="66882-136">Pour effectuer des comparaisons de chaînes, envisagez d’utiliser l’élément [Contains](contains.md) , car il fournit des options pour les paramètres correspondants, tels que case et espace blanc.</span><span class="sxs-lookup"><span data-stu-id="66882-136">To perform string comparisons, consider using the [Contains](contains.md) element, as it provides options for matching parameters, such as case and white space.</span></span> <span data-ttu-id="66882-137">Utilisez l’élément [not](not.md) en combinaison avec l’élément [Contains](contains.md) pour inverser le résultat.</span><span class="sxs-lookup"><span data-stu-id="66882-137">Use the [Not](not.md) element in conjunction with the [Contains](contains.md) element to negate the result.</span></span> 
  
<span data-ttu-id="66882-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="66882-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66882-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="66882-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66882-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="66882-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="66882-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="66882-141">Schema Name</span></span>  <br/> |<span data-ttu-id="66882-142">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="66882-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="66882-143">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="66882-143">Validation File</span></span>  <br/> |<span data-ttu-id="66882-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="66882-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="66882-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="66882-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="66882-146">False</span><span class="sxs-lookup"><span data-stu-id="66882-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66882-147">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="66882-147">See also</span></span>

- [<span data-ttu-id="66882-148">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="66882-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

