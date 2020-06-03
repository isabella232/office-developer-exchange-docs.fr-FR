---
title: IsLessThanOrEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsLessThanOrEqualTo
api_type:
- schema
ms.assetid: b5d85eb2-5e15-4d01-ad49-6289e735ad8a
description: L’élément IsLessThanOrEqualTo représente une expression de recherche qui compare une propriété à une valeur constante ou à une autre propriété et renvoie la valeur true si la première propriété est inférieure ou égale à la seconde.
ms.openlocfilehash: 7b153803b1c895c86e74428468c8e592c02a0acc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530028"
---
# <a name="islessthanorequalto"></a><span data-ttu-id="be60b-103">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="be60b-103">IsLessThanOrEqualTo</span></span>

<span data-ttu-id="be60b-104">L’élément **IsLessThanOrEqualTo** représente une expression de recherche qui compare une propriété à une valeur constante ou à une autre propriété et renvoie la **valeur true** si la première propriété est inférieure ou égale à la seconde.</span><span class="sxs-lookup"><span data-stu-id="be60b-104">The **IsLessThanOrEqualTo** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than or equal to the second.</span></span> 
  
```xml
<IsLessThanOrEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsLessThanOrEqualTo>
```

```xml
<IsLessThanOrEqualTo>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsLessThanOrEqualTo>
```

```xml
<IsLessThanOrEqualTo>
   <ExtendedFieldURI/> 
   <FieldURIOrConstant/>
</IsLessThanOrEqualTo>
```

<span data-ttu-id="be60b-105">**IsLessThanOrEqualToType**</span><span class="sxs-lookup"><span data-stu-id="be60b-105">**IsLessThanOrEqualToType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="be60b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="be60b-106">Attributes and elements</span></span>

<span data-ttu-id="be60b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="be60b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be60b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="be60b-108">Attributes</span></span>

<span data-ttu-id="be60b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="be60b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be60b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="be60b-110">Child elements</span></span>

|<span data-ttu-id="be60b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="be60b-111">**Element**</span></span>|<span data-ttu-id="be60b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="be60b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be60b-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="be60b-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="be60b-114">Identifie les propriétés référencées fréquemment par URI.</span><span class="sxs-lookup"><span data-stu-id="be60b-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="be60b-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="be60b-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="be60b-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="be60b-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="be60b-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="be60b-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="be60b-118">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="be60b-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="be60b-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="be60b-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="be60b-120">Représente une propriété ou une valeur constante à utiliser lors de la comparaison avec une autre propriété.</span><span class="sxs-lookup"><span data-stu-id="be60b-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="be60b-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="be60b-121">Parent elements</span></span>

|<span data-ttu-id="be60b-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="be60b-122">**Element**</span></span>|<span data-ttu-id="be60b-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="be60b-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be60b-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="be60b-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="be60b-125">Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="be60b-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="be60b-126">Not</span><span class="sxs-lookup"><span data-stu-id="be60b-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="be60b-127">Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="be60b-127">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="be60b-128">And</span><span class="sxs-lookup"><span data-stu-id="be60b-128">And</span></span>](and.md) <br/> |<span data-ttu-id="be60b-129">Représente une expression de recherche qui vous permet d’effectuer une opération booléenne et une opération entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="be60b-129">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="be60b-130">Le résultat de l’opération and est **true** si toutes les expressions de recherche contenues dans le et sont **vraies**.</span><span class="sxs-lookup"><span data-stu-id="be60b-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="be60b-131">Or</span><span class="sxs-lookup"><span data-stu-id="be60b-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="be60b-132">Représente une expression de recherche qui effectue une ou logique sur l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="be60b-132">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="be60b-133">[Ou](or.md) renverra **true** si l’un de ses enfants renvoie la valeur true.</span><span class="sxs-lookup"><span data-stu-id="be60b-133">[Or](or.md) will return **true** if any of its children return true.</span></span> <span data-ttu-id="be60b-134">[Ou](or.md) il doit avoir au moins deux enfants.</span><span class="sxs-lookup"><span data-stu-id="be60b-134">[Or](or.md) must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="be60b-135">Remarques</span><span class="sxs-lookup"><span data-stu-id="be60b-135">Remarks</span></span>

<span data-ttu-id="be60b-136">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="be60b-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be60b-137">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="be60b-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be60b-138">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="be60b-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be60b-139">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="be60b-139">Schema Name</span></span>  <br/> |<span data-ttu-id="be60b-140">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="be60b-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="be60b-141">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="be60b-141">Validation File</span></span>  <br/> |<span data-ttu-id="be60b-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="be60b-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="be60b-143">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="be60b-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="be60b-144">False</span><span class="sxs-lookup"><span data-stu-id="be60b-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be60b-145">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="be60b-145">See also</span></span>

- [<span data-ttu-id="be60b-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="be60b-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

