---
title: SearchExpression
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchExpression
api_type:
- schema
ms.assetid: daa179b6-8c7f-4268-a312-c2acc67fa7c3
description: L’élément SearchExpression est un élément abstrait qui représente l’élément substitué au sein d’une restriction. Toutes les expressions de recherche dérivent de ce type de base. Cet élément n’est pas utilisé dans un document d’instance XML.
ms.openlocfilehash: 8e0d09aec079280816cd9dfe2c1a55c88bb959a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829286"
---
# <a name="searchexpression"></a><span data-ttu-id="0078c-105">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="0078c-105">SearchExpression</span></span>

<span data-ttu-id="0078c-106">L’élément **SearchExpression** est un élément abstrait qui représente l’élément substitué au sein d’une restriction.</span><span class="sxs-lookup"><span data-stu-id="0078c-106">The **SearchExpression** element is an abstract element that represents the substituted element within a restriction.</span></span> <span data-ttu-id="0078c-107">Toutes les expressions de recherche dérivent de ce type de base.</span><span class="sxs-lookup"><span data-stu-id="0078c-107">All search expressions derive from this base type.</span></span> <span data-ttu-id="0078c-108">Cet élément n’est pas utilisé dans un document d’instance XML.</span><span class="sxs-lookup"><span data-stu-id="0078c-108">This element is not used in an XML instance document.</span></span> 
  
```xml
<SearchExpression/>
```

 <span data-ttu-id="0078c-109">**SearchExpressionType**</span><span class="sxs-lookup"><span data-stu-id="0078c-109">**SearchExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0078c-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0078c-110">Attributes and elements</span></span>

<span data-ttu-id="0078c-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0078c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0078c-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="0078c-112">Attributes</span></span>

<span data-ttu-id="0078c-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0078c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0078c-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0078c-114">Child elements</span></span>

<span data-ttu-id="0078c-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0078c-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0078c-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0078c-116">Parent elements</span></span>

|<span data-ttu-id="0078c-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0078c-117">**Element**</span></span>|<span data-ttu-id="0078c-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="0078c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0078c-119">Restriction</span><span class="sxs-lookup"><span data-stu-id="0078c-119">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="0078c-120">Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.</span><span class="sxs-lookup"><span data-stu-id="0078c-120">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="0078c-121">Pas</span><span class="sxs-lookup"><span data-stu-id="0078c-121">Not</span></span>](not.md) <br/> |<span data-ttu-id="0078c-122">Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="0078c-122">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="0078c-123">And</span><span class="sxs-lookup"><span data-stu-id="0078c-123">And</span></span>](and.md) <br/> |<span data-ttu-id="0078c-124">Représente une expression de recherche qui vous permet d’effectuer une opération type Boolean **et** entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="0078c-124">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="0078c-125">Le résultat de **l’opération** est **la valeur true** si toutes les expressions de recherche contenues dans l’élément **et** sont **remplies**.</span><span class="sxs-lookup"><span data-stu-id="0078c-125">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="0078c-126">Or</span><span class="sxs-lookup"><span data-stu-id="0078c-126">Or</span></span>](or.md) <br/> |<span data-ttu-id="0078c-127">Représente une expression de recherche qui effectue une opération **OR** logique sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="0078c-127">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="0078c-128">**Ou** renvoie **la valeur true** si un de ses enfants retourne **true**.</span><span class="sxs-lookup"><span data-stu-id="0078c-128">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="0078c-129">**Ou** doit disposer de deux ou plusieurs enfants.</span><span class="sxs-lookup"><span data-stu-id="0078c-129">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0078c-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="0078c-130">Remarks</span></span>

<span data-ttu-id="0078c-131">N’importe quel élément de filtre qui fait partie d’un groupe de substitution SearchExpression peut s’afficher à la place de l’élément SearchExpression.</span><span class="sxs-lookup"><span data-stu-id="0078c-131">Any filter element that is part of the SearchExpression substitution group can appear in place of the SearchExpression element.</span></span>
  
> [!NOTE]
> <span data-ttu-id="0078c-132">Cet élément se produira jamais directement au sein d’une instance de document.</span><span class="sxs-lookup"><span data-stu-id="0078c-132">This element will never occur directly within an instance document.</span></span> 
  
<span data-ttu-id="0078c-133">Les éléments suivants sont les membres du groupe de substitution SearchExpression :</span><span class="sxs-lookup"><span data-stu-id="0078c-133">The following elements are members of the SearchExpression substitution group:</span></span>
  
- [<span data-ttu-id="0078c-134">Exists</span><span class="sxs-lookup"><span data-stu-id="0078c-134">Exists</span></span>](exists.md)
    
- [<span data-ttu-id="0078c-135">Exclut</span><span class="sxs-lookup"><span data-stu-id="0078c-135">Excludes</span></span>](excludes.md)
    
- [<span data-ttu-id="0078c-136">Plutôt IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="0078c-136">IsEqualTo</span></span>](isequalto.md)
    
- [<span data-ttu-id="0078c-137">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="0078c-137">IsNotEqualTo</span></span>](isnotequalto.md)
    
- [<span data-ttu-id="0078c-138">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="0078c-138">IsGreaterThan</span></span>](isgreaterthan.md)
    
- [<span data-ttu-id="0078c-139">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="0078c-139">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)
    
- [<span data-ttu-id="0078c-140">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="0078c-140">IsLessThan</span></span>](islessthan.md)
    
- [<span data-ttu-id="0078c-141">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="0078c-141">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)
    
- [<span data-ttu-id="0078c-142">Contient</span><span class="sxs-lookup"><span data-stu-id="0078c-142">Contains</span></span>](contains.md)
    
- [<span data-ttu-id="0078c-143">Pas</span><span class="sxs-lookup"><span data-stu-id="0078c-143">Not</span></span>](not.md)
    
- [<span data-ttu-id="0078c-144">And</span><span class="sxs-lookup"><span data-stu-id="0078c-144">And</span></span>](and.md)
    
- [<span data-ttu-id="0078c-145">Or</span><span class="sxs-lookup"><span data-stu-id="0078c-145">Or</span></span>](or.md)
    
<span data-ttu-id="0078c-146">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0078c-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0078c-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0078c-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0078c-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0078c-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0078c-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0078c-149">Schema Name</span></span>  <br/> |<span data-ttu-id="0078c-150">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0078c-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="0078c-151">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0078c-151">Validation File</span></span>  <br/> |<span data-ttu-id="0078c-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0078c-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0078c-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0078c-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="0078c-154">False</span><span class="sxs-lookup"><span data-stu-id="0078c-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0078c-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0078c-155">See also</span></span>



- [<span data-ttu-id="0078c-156">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0078c-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

