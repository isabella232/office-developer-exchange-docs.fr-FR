---
title: Non
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
description: L’élément not représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.
ms.openlocfilehash: 84c64a6d9d39f260d416fc32e4e5f5fcdef027e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466716"
---
# <a name="not"></a><span data-ttu-id="e0b3a-103">Non</span><span class="sxs-lookup"><span data-stu-id="e0b3a-103">Not</span></span>

<span data-ttu-id="e0b3a-104">L’élément **not** représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-104">The **Not** element represents a search expression that negates the Boolean value of the search expression that it contains.</span></span> 
  
```xml
<Not>
   <SearchExpression/>
</Not>
```

 <span data-ttu-id="e0b3a-105">**NotType**</span><span class="sxs-lookup"><span data-stu-id="e0b3a-105">**NotType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0b3a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e0b3a-106">Attributes and elements</span></span>

<span data-ttu-id="e0b3a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0b3a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e0b3a-108">Attributes</span></span>

<span data-ttu-id="e0b3a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e0b3a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e0b3a-110">Child elements</span></span>

|<span data-ttu-id="e0b3a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e0b3a-111">**Element**</span></span>|<span data-ttu-id="e0b3a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e0b3a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0b3a-113">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="e0b3a-113">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="e0b3a-114">Représente la classe de base pour les expressions dans une restriction.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-114">Represents the base class for expressions within a restriction.</span></span> <br/><br/><span data-ttu-id="e0b3a-115">L’un des éléments suivants doit être substitué à l’élément **SearchExpression** :</span><span class="sxs-lookup"><span data-stu-id="e0b3a-115">One of the following elements must be substituted for the **SearchExpression** element:</span></span> <br/> <br/><span data-ttu-id="e0b3a-116">- [Existe](exists.md)</span><span class="sxs-lookup"><span data-stu-id="e0b3a-116">- [Exists](exists.md)</span></span> <br/><span data-ttu-id="e0b3a-117">- [Exclut](excludes.md)</span><span class="sxs-lookup"><span data-stu-id="e0b3a-117">- [Excludes](excludes.md)</span></span> <br/><span data-ttu-id="e0b3a-118">- [IsEqualTo](isequalto.md)</span><span class="sxs-lookup"><span data-stu-id="e0b3a-118">- [IsEqualTo](isequalto.md)</span></span> <br/><span data-ttu-id="e0b3a-119">- [IsNotEqualTo](isnotequalto.md)</span><span class="sxs-lookup"><span data-stu-id="e0b3a-119">- [IsNotEqualTo](isnotequalto.md)</span></span> <br/><span data-ttu-id="e0b3a-120">- [IsGreaterThan](isgreaterthan.md)</span><span class="sxs-lookup"><span data-stu-id="e0b3a-120">- [IsGreaterThan](isgreaterthan.md)</span></span> <br/><span data-ttu-id="e0b3a-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="e0b3a-121">- [IsGreaterThanOrEqualTo](isgreaterthanorequalto.md)</span></span> <br/><span data-ttu-id="e0b3a-122">- [IsLessThan](islessthan.md)</span><span class="sxs-lookup"><span data-stu-id="e0b3a-122">- [IsLessThan](islessthan.md)</span></span> <br/><span data-ttu-id="e0b3a-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span><span class="sxs-lookup"><span data-stu-id="e0b3a-123">- [IsLessThanOrEqualTo](islessthanorequalto.md)</span></span> <br/><span data-ttu-id="e0b3a-124">- [Comporte](contains.md)</span><span class="sxs-lookup"><span data-stu-id="e0b3a-124">- [Contains](contains.md)</span></span> <br/><span data-ttu-id="e0b3a-125">- **Aucun**</span><span class="sxs-lookup"><span data-stu-id="e0b3a-125">- **Not**</span></span> <br/><span data-ttu-id="e0b3a-126">- [Les](and.md)</span><span class="sxs-lookup"><span data-stu-id="e0b3a-126">- [And](and.md)</span></span> <br/><span data-ttu-id="e0b3a-127">- [Des](or.md)</span><span class="sxs-lookup"><span data-stu-id="e0b3a-127">- [Or](or.md)</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e0b3a-128">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e0b3a-128">Parent elements</span></span>

|<span data-ttu-id="e0b3a-129">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e0b3a-129">**Element**</span></span>|<span data-ttu-id="e0b3a-130">**Description**</span><span class="sxs-lookup"><span data-stu-id="e0b3a-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0b3a-131">Restriction</span><span class="sxs-lookup"><span data-stu-id="e0b3a-131">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="e0b3a-132">Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-132">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|<span data-ttu-id="e0b3a-133">**Not**</span><span class="sxs-lookup"><span data-stu-id="e0b3a-133">**Not**</span></span> <br/> |<span data-ttu-id="e0b3a-134">Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-134">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="e0b3a-135">And</span><span class="sxs-lookup"><span data-stu-id="e0b3a-135">And</span></span>](and.md) <br/> |<span data-ttu-id="e0b3a-136">Représente une expression de recherche qui vous permet d’effectuer une opération booléenne **et** une opération entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-136">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="e0b3a-137">Le résultat de l’opération **and** est **true** si toutes les expressions de recherche contenues dans l’élément **and** sont **true**.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-137">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="e0b3a-138">Or</span><span class="sxs-lookup"><span data-stu-id="e0b3a-138">Or</span></span>](or.md) <br/> |<span data-ttu-id="e0b3a-139">Représente une expression de recherche qui effectue une opération **or** logique sur l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-139">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="e0b3a-140">**Ou** renverra **true** si l’un de ses enfants renvoie la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-140">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="e0b3a-141">**Ou** il doit avoir au moins deux enfants.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-141">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e0b3a-142">Remarques</span><span class="sxs-lookup"><span data-stu-id="e0b3a-142">Remarks</span></span>

<span data-ttu-id="e0b3a-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e0b3a-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0b3a-144">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e0b3a-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0b3a-145">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e0b3a-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e0b3a-146">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e0b3a-146">Schema Name</span></span>  <br/> |<span data-ttu-id="e0b3a-147">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e0b3a-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="e0b3a-148">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e0b3a-148">Validation File</span></span>  <br/> |<span data-ttu-id="e0b3a-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e0b3a-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e0b3a-150">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e0b3a-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="e0b3a-151">False</span><span class="sxs-lookup"><span data-stu-id="e0b3a-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e0b3a-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e0b3a-152">See also</span></span>

- [<span data-ttu-id="e0b3a-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e0b3a-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

