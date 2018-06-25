---
title: Or
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Or
api_type:
- schema
ms.assetid: 4876d83a-73a3-4953-9d95-3048e6b76ccb
description: L’élément ou représente une expression de recherche qui effectue une opération OR logique sur l’expression de recherche qu’il contient. Ou renvoie la valeur true si un de ses enfants retourne true. Ou doit avoir deux ou plusieurs enfants.
ms.openlocfilehash: 46cf031047aeb09e05a385150ab7587968aef345
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828661"
---
# <a name="or"></a><span data-ttu-id="1851f-105">Or</span><span class="sxs-lookup"><span data-stu-id="1851f-105">Or</span></span>

<span data-ttu-id="1851f-106">L’élément **ou** représente une expression de recherche qui effectue une logique **ou** sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="1851f-106">The **Or** element represents a search expression that performs a logical **OR** on the search expression that it contains.</span></span> <span data-ttu-id="1851f-107">**Ou** renvoie **la valeur true** si un de ses enfants retourne **true**.</span><span class="sxs-lookup"><span data-stu-id="1851f-107">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="1851f-108">**Ou** doit disposer de deux ou plusieurs enfants.</span><span class="sxs-lookup"><span data-stu-id="1851f-108">**Or** must have two or more children.</span></span> 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 <span data-ttu-id="1851f-109">**OrType**</span><span class="sxs-lookup"><span data-stu-id="1851f-109">**OrType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1851f-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1851f-110">Attributes and elements</span></span>

<span data-ttu-id="1851f-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1851f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1851f-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="1851f-112">Attributes</span></span>

<span data-ttu-id="1851f-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1851f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1851f-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1851f-114">Child elements</span></span>

|<span data-ttu-id="1851f-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1851f-115">**Element**</span></span>|<span data-ttu-id="1851f-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="1851f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1851f-117">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="1851f-117">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="1851f-118">Représente la classe de base pour les expressions au sein d’une restriction.</span><span class="sxs-lookup"><span data-stu-id="1851f-118">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="1851f-119">Un des éléments suivants doit être remplacé par l’élément **SearchExpression** :</span><span class="sxs-lookup"><span data-stu-id="1851f-119">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="1851f-120">- [Il existe](exists.md)</span><span class="sxs-lookup"><span data-stu-id="1851f-120">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="1851f-121">- [Exclut](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="1851f-121">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="1851f-122">- [Plutôt IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="1851f-122">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="1851f-123">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="1851f-123">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="1851f-124">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="1851f-124">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="1851f-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="1851f-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="1851f-126">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="1851f-126">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="1851f-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="1851f-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="1851f-128">- [Contient](contains.md)</span><span class="sxs-lookup"><span data-stu-id="1851f-128">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="1851f-129">- [Pas](not.md)</span><span class="sxs-lookup"><span data-stu-id="1851f-129">- [Not](not.md)</span></span> <br/><span data-ttu-id="1851f-130">- [Et](and.md)</span><span class="sxs-lookup"><span data-stu-id="1851f-130">- [And](and.md)</span></span> <br/><span data-ttu-id="1851f-131">- **Ou**</span><span class="sxs-lookup"><span data-stu-id="1851f-131">- **Or**</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1851f-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1851f-132">Parent elements</span></span>

|<span data-ttu-id="1851f-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1851f-133">**Element**</span></span>|<span data-ttu-id="1851f-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="1851f-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1851f-135">Restriction</span><span class="sxs-lookup"><span data-stu-id="1851f-135">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="1851f-136">Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.</span><span class="sxs-lookup"><span data-stu-id="1851f-136">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="1851f-137">Pas</span><span class="sxs-lookup"><span data-stu-id="1851f-137">Not</span></span>](not.md) <br/> |<span data-ttu-id="1851f-138">Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="1851f-138">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="1851f-139">And</span><span class="sxs-lookup"><span data-stu-id="1851f-139">And</span></span>](and.md) <br/> |<span data-ttu-id="1851f-140">Représente une expression de recherche qui vous permet d’effectuer une opération type Boolean **et** entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="1851f-140">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="1851f-141">Le résultat de **l’opération** est **la valeur true** si toutes les expressions de recherche contenues dans l’élément **et** sont **remplies**.</span><span class="sxs-lookup"><span data-stu-id="1851f-141">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|<span data-ttu-id="1851f-142">**Or**</span><span class="sxs-lookup"><span data-stu-id="1851f-142">**Or**</span></span> <br/> |<span data-ttu-id="1851f-143">Représente une expression de recherche qui effectue une opération **OR** logique sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="1851f-143">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="1851f-144">**Ou** renvoie **la valeur true** si un de ses enfants retourne **true**.</span><span class="sxs-lookup"><span data-stu-id="1851f-144">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="1851f-145">**Ou** doit disposer de deux ou plusieurs enfants.</span><span class="sxs-lookup"><span data-stu-id="1851f-145">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1851f-146">Remarques</span><span class="sxs-lookup"><span data-stu-id="1851f-146">Remarks</span></span>

<span data-ttu-id="1851f-147">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1851f-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1851f-148">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1851f-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1851f-149">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1851f-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1851f-150">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1851f-150">Schema Name</span></span>  <br/> |<span data-ttu-id="1851f-151">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1851f-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="1851f-152">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1851f-152">Validation File</span></span>  <br/> |<span data-ttu-id="1851f-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1851f-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1851f-154">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1851f-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="1851f-155">False</span><span class="sxs-lookup"><span data-stu-id="1851f-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1851f-156">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1851f-156">See also</span></span>

- [<span data-ttu-id="1851f-157">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1851f-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

