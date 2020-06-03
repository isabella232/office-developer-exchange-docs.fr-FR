---
title: Ou
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
description: L’élément ou représente une expression de recherche qui effectue une ou logique sur l’expression de recherche qu’il contient. Ou renverra true si l’un de ses enfants renvoie la valeur true. Ou il doit avoir au moins deux enfants.
ms.openlocfilehash: 9bc676da5bbaad64f11f6717fb487c2e9bcf2d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462478"
---
# <a name="or"></a><span data-ttu-id="c5390-105">Ou</span><span class="sxs-lookup"><span data-stu-id="c5390-105">Or</span></span>

<span data-ttu-id="c5390-106">L’élément **ou** représente une expression de recherche qui effectue une **ou** logique sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="c5390-106">The **Or** element represents a search expression that performs a logical **OR** on the search expression that it contains.</span></span> <span data-ttu-id="c5390-107">**Ou** renverra **true** si l’un de ses enfants renvoie la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="c5390-107">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="c5390-108">**Ou** il doit avoir au moins deux enfants.</span><span class="sxs-lookup"><span data-stu-id="c5390-108">**Or** must have two or more children.</span></span> 
  
```xml
<Or>
   <SearchExpression/>
   <SearchExpression/>
</Or>
```

 <span data-ttu-id="c5390-109">**OrType**</span><span class="sxs-lookup"><span data-stu-id="c5390-109">**OrType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5390-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c5390-110">Attributes and elements</span></span>

<span data-ttu-id="c5390-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c5390-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5390-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="c5390-112">Attributes</span></span>

<span data-ttu-id="c5390-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="c5390-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5390-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c5390-114">Child elements</span></span>

|<span data-ttu-id="c5390-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c5390-115">**Element**</span></span>|<span data-ttu-id="c5390-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="c5390-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5390-117">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="c5390-117">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="c5390-118">Représente la classe de base pour les expressions dans une restriction.</span><span class="sxs-lookup"><span data-stu-id="c5390-118">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="c5390-119">L’un des éléments suivants doit être substitué à l’élément **SearchExpression** :</span><span class="sxs-lookup"><span data-stu-id="c5390-119">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="c5390-120">- [Existe](exists.md)</span><span class="sxs-lookup"><span data-stu-id="c5390-120">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="c5390-121">- [Exclut](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="c5390-121">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="c5390-122">- [IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="c5390-122">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="c5390-123">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="c5390-123">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="c5390-124">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="c5390-124">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="c5390-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="c5390-125">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="c5390-126">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="c5390-126">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="c5390-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="c5390-127">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="c5390-128">- [Comporte](contains.md)</span><span class="sxs-lookup"><span data-stu-id="c5390-128">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="c5390-129">- [Aucun](not.md)</span><span class="sxs-lookup"><span data-stu-id="c5390-129">- [Not](not.md)</span></span> <br/><span data-ttu-id="c5390-130">- [Les](and.md)</span><span class="sxs-lookup"><span data-stu-id="c5390-130">- [And](and.md)</span></span> <br/><span data-ttu-id="c5390-131">- **Des**</span><span class="sxs-lookup"><span data-stu-id="c5390-131">- **Or**</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5390-132">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c5390-132">Parent elements</span></span>

|<span data-ttu-id="c5390-133">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c5390-133">**Element**</span></span>|<span data-ttu-id="c5390-134">**Description**</span><span class="sxs-lookup"><span data-stu-id="c5390-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5390-135">Restriction</span><span class="sxs-lookup"><span data-stu-id="c5390-135">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="c5390-136">Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="c5390-136">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="c5390-137">Not</span><span class="sxs-lookup"><span data-stu-id="c5390-137">Not</span></span>](not.md) <br/> |<span data-ttu-id="c5390-138">Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="c5390-138">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="c5390-139">And</span><span class="sxs-lookup"><span data-stu-id="c5390-139">And</span></span>](and.md) <br/> |<span data-ttu-id="c5390-140">Représente une expression de recherche qui vous permet d’effectuer une opération booléenne **et** une opération entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="c5390-140">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="c5390-141">Le résultat de l’opération **and** est **true** si toutes les expressions de recherche contenues dans l’élément **and** sont **true**.</span><span class="sxs-lookup"><span data-stu-id="c5390-141">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|<span data-ttu-id="c5390-142">**Or**</span><span class="sxs-lookup"><span data-stu-id="c5390-142">**Or**</span></span> <br/> |<span data-ttu-id="c5390-143">Représente une expression de recherche qui effectue une opération **or** logique sur l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="c5390-143">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="c5390-144">**Ou** renverra **true** si l’un de ses enfants renvoie la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="c5390-144">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="c5390-145">**Ou** il doit avoir au moins deux enfants.</span><span class="sxs-lookup"><span data-stu-id="c5390-145">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c5390-146">Remarques</span><span class="sxs-lookup"><span data-stu-id="c5390-146">Remarks</span></span>

<span data-ttu-id="c5390-147">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c5390-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5390-148">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c5390-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5390-149">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c5390-149">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5390-150">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c5390-150">Schema Name</span></span>  <br/> |<span data-ttu-id="c5390-151">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c5390-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5390-152">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c5390-152">Validation File</span></span>  <br/> |<span data-ttu-id="c5390-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c5390-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5390-154">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c5390-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5390-155">False</span><span class="sxs-lookup"><span data-stu-id="c5390-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5390-156">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c5390-156">See also</span></span>

- [<span data-ttu-id="c5390-157">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c5390-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

