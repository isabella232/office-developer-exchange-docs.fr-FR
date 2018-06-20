---
title: And
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- And
api_type:
- schema
ms.assetid: 790246c2-37ad-49a8-91b9-6186d743b011
description: L’élément et représente une expression de recherche qui vous permet d’effectuer une opération de type Boolean et entre deux ou plusieurs expressions de recherche. Le résultat de l’opération est true si toutes les expressions de recherche contenues dans l’élément et sont vraies.
ms.openlocfilehash: d287d57d68aeca7127325dc8fb65fd0190e5b5eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755207"
---
# <a name="and"></a><span data-ttu-id="93677-104">And</span><span class="sxs-lookup"><span data-stu-id="93677-104">And</span></span>

<span data-ttu-id="93677-105">L’élément **et** représente une expression de recherche qui vous permet d’effectuer une opération type Boolean **et** entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="93677-105">The **And** element represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="93677-106">Le résultat de **l’opération** est **la valeur true** si toutes les expressions de recherche contenues dans l’élément **et** sont **remplies**.</span><span class="sxs-lookup"><span data-stu-id="93677-106">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 <span data-ttu-id="93677-107">**AndType**</span><span class="sxs-lookup"><span data-stu-id="93677-107">**AndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93677-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="93677-108">Attributes and elements</span></span>

<span data-ttu-id="93677-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="93677-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93677-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="93677-110">Attributes</span></span>

<span data-ttu-id="93677-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="93677-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93677-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="93677-112">Child elements</span></span>

|<span data-ttu-id="93677-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="93677-113">**Element**</span></span>|<span data-ttu-id="93677-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="93677-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93677-115">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="93677-115">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="93677-116">Représente la classe de base pour les expressions au sein d’une restriction.</span><span class="sxs-lookup"><span data-stu-id="93677-116">Represents the base class for expressions within a restriction.</span></span> <span data-ttu-id="93677-117">Il doit exister au moins deux expressions de recherche dans une opération.</span><span class="sxs-lookup"><span data-stu-id="93677-117">There must be two or more search expressions in an And operation.</span></span><br/><br/>  <span data-ttu-id="93677-118">Un des éléments suivants doit être remplacé par l’élément **SearchExpression** :</span><span class="sxs-lookup"><span data-stu-id="93677-118">One of the following elements must be substituted for the **SearchExpression** element:</span></span><ul><li> [<span data-ttu-id="93677-119">Exists</span><span class="sxs-lookup"><span data-stu-id="93677-119">Exists</span></span>](exists.md)</li><li>[<span data-ttu-id="93677-120">Exclut</span><span class="sxs-lookup"><span data-stu-id="93677-120">Excludes</span></span>](excludes.md)</li><li>[<span data-ttu-id="93677-121">Plutôt IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="93677-121">IsEqualTo</span></span>](isequalto.md)</li><li>[<span data-ttu-id="93677-122">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="93677-122">IsNotEqualTo</span></span>](isnotequalto.md)</li><li>[<span data-ttu-id="93677-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="93677-123">IsGreaterThan</span></span>](isgreaterthan.md)</li><li>[<span data-ttu-id="93677-124">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="93677-124">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)</li><li>[<span data-ttu-id="93677-125">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="93677-125">IsLessThan</span></span>](islessthan.md)</li><li>[<span data-ttu-id="93677-126">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="93677-126">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)</li><li>[<span data-ttu-id="93677-127">Contient</span><span class="sxs-lookup"><span data-stu-id="93677-127">Contains</span></span>](contains.md)</li><li>[<span data-ttu-id="93677-128">Pas</span><span class="sxs-lookup"><span data-stu-id="93677-128">Not</span></span>](not.md)</li><li><span data-ttu-id="93677-129">**And**</span><span class="sxs-lookup"><span data-stu-id="93677-129">**And**</span></span></li><li>[<span data-ttu-id="93677-130">Or</span><span class="sxs-lookup"><span data-stu-id="93677-130">Or</span></span>](or.md) </li></ul> |
   
### <a name="parent-elements"></a><span data-ttu-id="93677-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="93677-131">Parent elements</span></span>

|<span data-ttu-id="93677-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="93677-132">**Element**</span></span>|<span data-ttu-id="93677-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="93677-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93677-134">Restriction</span><span class="sxs-lookup"><span data-stu-id="93677-134">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="93677-135">Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.</span><span class="sxs-lookup"><span data-stu-id="93677-135">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="93677-136">Pas</span><span class="sxs-lookup"><span data-stu-id="93677-136">Not</span></span>](not.md) <br/> |<span data-ttu-id="93677-137">Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="93677-137">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|<span data-ttu-id="93677-138">**And**</span><span class="sxs-lookup"><span data-stu-id="93677-138">**And**</span></span> <br/> |<span data-ttu-id="93677-139">Représente une expression de recherche qui vous permet d’effectuer une opération type Boolean **et** entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="93677-139">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="93677-140">Le résultat de **l’opération** est **la valeur true** si toutes les expressions de recherche contenues dans l’élément **et** sont **remplies**.</span><span class="sxs-lookup"><span data-stu-id="93677-140">The result of the **AND** operation is **true** if all of the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="93677-141">Or</span><span class="sxs-lookup"><span data-stu-id="93677-141">Or</span></span>](or.md) <br/> |<span data-ttu-id="93677-142">Représente une expression de recherche qui effectue une opération **OR** logique sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="93677-142">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="93677-143">**Ou** renvoie **la valeur true** si un de ses enfants retourne **true**.</span><span class="sxs-lookup"><span data-stu-id="93677-143">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="93677-144">**Ou** doit disposer de deux ou plusieurs enfants.</span><span class="sxs-lookup"><span data-stu-id="93677-144">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="93677-145">Remarques</span><span class="sxs-lookup"><span data-stu-id="93677-145">Remarks</span></span>

<span data-ttu-id="93677-146">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="93677-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93677-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="93677-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93677-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="93677-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93677-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="93677-149">Schema Name</span></span>  <br/> |<span data-ttu-id="93677-150">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="93677-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="93677-151">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="93677-151">Validation File</span></span>  <br/> |<span data-ttu-id="93677-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="93677-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="93677-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="93677-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="93677-154">False</span><span class="sxs-lookup"><span data-stu-id="93677-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93677-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="93677-155">See also</span></span>

- [<span data-ttu-id="93677-156">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="93677-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

