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
description: L’élément SearchExpression est un élément abstrait qui représente l’élément substitué dans une restriction. Toutes les expressions de recherche dérivent de ce type de base. Cet élément n’est pas utilisé dans un document d’instance XML.
ms.openlocfilehash: db06ce8e2faa0f2589963d58aab55073c618c171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530351"
---
# <a name="searchexpression"></a><span data-ttu-id="f8ac9-105">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="f8ac9-105">SearchExpression</span></span>

<span data-ttu-id="f8ac9-106">L’élément **SearchExpression** est un élément abstrait qui représente l’élément substitué dans une restriction.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-106">The **SearchExpression** element is an abstract element that represents the substituted element within a restriction.</span></span> <span data-ttu-id="f8ac9-107">Toutes les expressions de recherche dérivent de ce type de base.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-107">All search expressions derive from this base type.</span></span> <span data-ttu-id="f8ac9-108">Cet élément n’est pas utilisé dans un document d’instance XML.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-108">This element is not used in an XML instance document.</span></span> 
  
```xml
<SearchExpression/>
```

 <span data-ttu-id="f8ac9-109">**SearchExpressionType**</span><span class="sxs-lookup"><span data-stu-id="f8ac9-109">**SearchExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8ac9-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f8ac9-110">Attributes and elements</span></span>

<span data-ttu-id="f8ac9-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8ac9-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="f8ac9-112">Attributes</span></span>

<span data-ttu-id="f8ac9-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8ac9-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f8ac9-114">Child elements</span></span>

<span data-ttu-id="f8ac9-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f8ac9-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f8ac9-116">Parent elements</span></span>

|<span data-ttu-id="f8ac9-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f8ac9-117">**Element**</span></span>|<span data-ttu-id="f8ac9-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="f8ac9-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8ac9-119">Restriction</span><span class="sxs-lookup"><span data-stu-id="f8ac9-119">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="f8ac9-120">Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-120">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="f8ac9-121">Not</span><span class="sxs-lookup"><span data-stu-id="f8ac9-121">Not</span></span>](not.md) <br/> |<span data-ttu-id="f8ac9-122">Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-122">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="f8ac9-123">And</span><span class="sxs-lookup"><span data-stu-id="f8ac9-123">And</span></span>](and.md) <br/> |<span data-ttu-id="f8ac9-124">Représente une expression de recherche qui vous permet d’effectuer une opération booléenne **et** une opération entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-124">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="f8ac9-125">Le résultat de l’opération **and** est **true** si toutes les expressions de recherche contenues dans l’élément **and** sont **true**.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-125">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="f8ac9-126">Or</span><span class="sxs-lookup"><span data-stu-id="f8ac9-126">Or</span></span>](or.md) <br/> |<span data-ttu-id="f8ac9-127">Représente une expression de recherche qui effectue une opération **or** logique sur l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-127">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="f8ac9-128">**Ou** renverra **true** si l’un de ses enfants renvoie la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-128">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="f8ac9-129">**Ou** il doit avoir au moins deux enfants.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-129">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f8ac9-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="f8ac9-130">Remarks</span></span>

<span data-ttu-id="f8ac9-131">Tout élément Filter qui fait partie du groupe de substitution SearchExpression peut apparaître à la place de l’élément SearchExpression.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-131">Any filter element that is part of the SearchExpression substitution group can appear in place of the SearchExpression element.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f8ac9-132">Cet élément ne se produira jamais directement dans un document d’instance.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-132">This element will never occur directly within an instance document.</span></span> 
  
<span data-ttu-id="f8ac9-133">Les éléments suivants sont membres du groupe de substitution SearchExpression :</span><span class="sxs-lookup"><span data-stu-id="f8ac9-133">The following elements are members of the SearchExpression substitution group:</span></span>
  
- [<span data-ttu-id="f8ac9-134">Exists</span><span class="sxs-lookup"><span data-stu-id="f8ac9-134">Exists</span></span>](exists.md)
    
- [<span data-ttu-id="f8ac9-135">Exclut</span><span class="sxs-lookup"><span data-stu-id="f8ac9-135">Excludes</span></span>](excludes.md)
    
- [<span data-ttu-id="f8ac9-136">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="f8ac9-136">IsEqualTo</span></span>](isequalto.md)
    
- [<span data-ttu-id="f8ac9-137">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="f8ac9-137">IsNotEqualTo</span></span>](isnotequalto.md)
    
- [<span data-ttu-id="f8ac9-138">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="f8ac9-138">IsGreaterThan</span></span>](isgreaterthan.md)
    
- [<span data-ttu-id="f8ac9-139">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="f8ac9-139">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)
    
- [<span data-ttu-id="f8ac9-140">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="f8ac9-140">IsLessThan</span></span>](islessthan.md)
    
- [<span data-ttu-id="f8ac9-141">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="f8ac9-141">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)
    
- [<span data-ttu-id="f8ac9-142">Contains</span><span class="sxs-lookup"><span data-stu-id="f8ac9-142">Contains</span></span>](contains.md)
    
- [<span data-ttu-id="f8ac9-143">Not</span><span class="sxs-lookup"><span data-stu-id="f8ac9-143">Not</span></span>](not.md)
    
- [<span data-ttu-id="f8ac9-144">And</span><span class="sxs-lookup"><span data-stu-id="f8ac9-144">And</span></span>](and.md)
    
- [<span data-ttu-id="f8ac9-145">Or</span><span class="sxs-lookup"><span data-stu-id="f8ac9-145">Or</span></span>](or.md)
    
<span data-ttu-id="f8ac9-146">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f8ac9-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8ac9-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f8ac9-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8ac9-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f8ac9-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f8ac9-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f8ac9-149">Schema Name</span></span>  <br/> |<span data-ttu-id="f8ac9-150">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f8ac9-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="f8ac9-151">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f8ac9-151">Validation File</span></span>  <br/> |<span data-ttu-id="f8ac9-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f8ac9-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f8ac9-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f8ac9-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="f8ac9-154">False</span><span class="sxs-lookup"><span data-stu-id="f8ac9-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8ac9-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f8ac9-155">See also</span></span>



- [<span data-ttu-id="f8ac9-156">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f8ac9-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

