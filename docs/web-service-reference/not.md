---
title: Pas
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Not
api_type:
- schema
ms.assetid: 1aa16318-7e90-4b19-bce8-dd1a20a66223
description: L’élément n’est pas représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.
ms.openlocfilehash: f5bc709d8b1e77a13b3598905651ac1750436f03
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828553"
---
# <a name="not"></a><span data-ttu-id="3955c-103">Pas</span><span class="sxs-lookup"><span data-stu-id="3955c-103">Not</span></span>

<span data-ttu-id="3955c-104">L’élément **pas** représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="3955c-104">The **Not** element represents a search expression that negates the Boolean value of the search expression that it contains.</span></span> 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 <span data-ttu-id="3955c-105">**NotType**</span><span class="sxs-lookup"><span data-stu-id="3955c-105">**NotType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3955c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3955c-106">Attributes and elements</span></span>

<span data-ttu-id="3955c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3955c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3955c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3955c-108">Attributes</span></span>

<span data-ttu-id="3955c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3955c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3955c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3955c-110">Child elements</span></span>

|<span data-ttu-id="3955c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3955c-111">**Element**</span></span>|<span data-ttu-id="3955c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3955c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3955c-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="3955c-113">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="3955c-114">Représente la classe de base pour les expressions au sein d’une restriction.</span><span class="sxs-lookup"><span data-stu-id="3955c-114">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="3955c-115">Un des éléments suivants doit être remplacé par l’élément **SearchExpression** :</span><span class="sxs-lookup"><span data-stu-id="3955c-115">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="3955c-116">- [Il existe](exists.md)</span><span class="sxs-lookup"><span data-stu-id="3955c-116">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="3955c-117">- [Exclut](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="3955c-117">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="3955c-118">- [Plutôt IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="3955c-118">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="3955c-119">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="3955c-119">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="3955c-120">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="3955c-120">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="3955c-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="3955c-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="3955c-122">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="3955c-122">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="3955c-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="3955c-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="3955c-124">- [Contient](contains.md)</span><span class="sxs-lookup"><span data-stu-id="3955c-124">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="3955c-125">- **Pas**</span><span class="sxs-lookup"><span data-stu-id="3955c-125">- **Not**</span></span> <br/><span data-ttu-id="3955c-126">- [Et](and.md)</span><span class="sxs-lookup"><span data-stu-id="3955c-126">- [And](and.md)</span></span> <br/><span data-ttu-id="3955c-127">- [Ou](or.md)</span><span class="sxs-lookup"><span data-stu-id="3955c-127">- [Or](or.md)</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3955c-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3955c-128">Parent elements</span></span>

|<span data-ttu-id="3955c-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3955c-129">**Element**</span></span>|<span data-ttu-id="3955c-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="3955c-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3955c-131">Restriction</span><span class="sxs-lookup"><span data-stu-id="3955c-131">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="3955c-132">Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.</span><span class="sxs-lookup"><span data-stu-id="3955c-132">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|<span data-ttu-id="3955c-133">**Pas**</span><span class="sxs-lookup"><span data-stu-id="3955c-133">**Not**</span></span> <br/> |<span data-ttu-id="3955c-134">Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="3955c-134">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="3955c-135">And</span><span class="sxs-lookup"><span data-stu-id="3955c-135">And</span></span>](and.md) <br/> |<span data-ttu-id="3955c-136">Représente une expression de recherche qui vous permet d’effectuer une opération type Boolean **et** entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="3955c-136">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="3955c-137">Le résultat de **l’opération** est **la valeur true** si toutes les expressions de recherche contenues dans l’élément **et** sont **remplies**.</span><span class="sxs-lookup"><span data-stu-id="3955c-137">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="3955c-138">Or</span><span class="sxs-lookup"><span data-stu-id="3955c-138">Or</span></span>](or.md) <br/> |<span data-ttu-id="3955c-139">Représente une expression de recherche qui effectue une opération **OR** logique sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="3955c-139">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="3955c-140">**Ou** renvoie **la valeur true** si un de ses enfants retourne **true**.</span><span class="sxs-lookup"><span data-stu-id="3955c-140">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="3955c-141">**Ou** doit disposer de deux ou plusieurs enfants.</span><span class="sxs-lookup"><span data-stu-id="3955c-141">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3955c-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="3955c-142">Remarks</span></span>

<span data-ttu-id="3955c-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="3955c-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3955c-144">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3955c-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3955c-145">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3955c-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3955c-146">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3955c-146">Schema Name</span></span>  <br/> |<span data-ttu-id="3955c-147">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3955c-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="3955c-148">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3955c-148">Validation File</span></span>  <br/> |<span data-ttu-id="3955c-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3955c-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3955c-150">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3955c-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="3955c-151">False</span><span class="sxs-lookup"><span data-stu-id="3955c-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3955c-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3955c-152">See also</span></span>

- [<span data-ttu-id="3955c-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3955c-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

