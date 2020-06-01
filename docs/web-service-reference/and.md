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
description: L’élément and représente une expression de recherche qui vous permet d’effectuer une opération booléenne et une opération entre deux ou plusieurs expressions de recherche. Le résultat de l’opération AND est true si toutes les expressions de recherche contenues dans l’élément and sont true.
ms.openlocfilehash: f5239f19c2b5a931eefa9ff4a9dd8ed9d775bae2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464720"
---
# <a name="and"></a><span data-ttu-id="fa600-104">And</span><span class="sxs-lookup"><span data-stu-id="fa600-104">And</span></span>

<span data-ttu-id="fa600-105">L’élément **and** représente une expression de recherche qui vous permet d’effectuer une opération booléenne **et** une opération entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="fa600-105">The **And** element represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="fa600-106">Le résultat de l’opération **and** est **true** si toutes les expressions de recherche contenues dans l’élément **and** sont **true**.</span><span class="sxs-lookup"><span data-stu-id="fa600-106">The result of the **AND** operation is **true** if all the search expressions contained within the **And** element are **true**.</span></span>
  
```xml
<And>
   <SearchExpression/>
   <SearchExpression/>
</And>
```

 <span data-ttu-id="fa600-107">**AndType**</span><span class="sxs-lookup"><span data-stu-id="fa600-107">**AndType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa600-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fa600-108">Attributes and elements</span></span>

<span data-ttu-id="fa600-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fa600-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa600-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="fa600-110">Attributes</span></span>

<span data-ttu-id="fa600-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fa600-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa600-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fa600-112">Child elements</span></span>

|<span data-ttu-id="fa600-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fa600-113">**Element**</span></span>|<span data-ttu-id="fa600-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="fa600-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa600-115">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="fa600-115">SearchExpression</span></span>](searchexpression.md) <br/> | <span data-ttu-id="fa600-116">Représente la classe de base pour les expressions dans une restriction.</span><span class="sxs-lookup"><span data-stu-id="fa600-116">Represents the base class for expressions within a restriction.</span></span> <span data-ttu-id="fa600-117">Il doit y avoir au moins deux expressions de recherche dans une opération and.</span><span class="sxs-lookup"><span data-stu-id="fa600-117">There must be two or more search expressions in an And operation.</span></span><br/><br/>  <span data-ttu-id="fa600-118">L’un des éléments suivants doit être substitué à l’élément **SearchExpression** :</span><span class="sxs-lookup"><span data-stu-id="fa600-118">One of the following elements must be substituted for the **SearchExpression** element:</span></span><ul><li> [<span data-ttu-id="fa600-119">Exists</span><span class="sxs-lookup"><span data-stu-id="fa600-119">Exists</span></span>](exists.md)</li><li>[<span data-ttu-id="fa600-120">Exclut</span><span class="sxs-lookup"><span data-stu-id="fa600-120">Excludes</span></span>](excludes.md)</li><li>[<span data-ttu-id="fa600-121">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="fa600-121">IsEqualTo</span></span>](isequalto.md)</li><li>[<span data-ttu-id="fa600-122">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="fa600-122">IsNotEqualTo</span></span>](isnotequalto.md)</li><li>[<span data-ttu-id="fa600-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="fa600-123">IsGreaterThan</span></span>](isgreaterthan.md)</li><li>[<span data-ttu-id="fa600-124">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="fa600-124">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md)</li><li>[<span data-ttu-id="fa600-125">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="fa600-125">IsLessThan</span></span>](islessthan.md)</li><li>[<span data-ttu-id="fa600-126">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="fa600-126">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md)</li><li>[<span data-ttu-id="fa600-127">Contains</span><span class="sxs-lookup"><span data-stu-id="fa600-127">Contains</span></span>](contains.md)</li><li>[<span data-ttu-id="fa600-128">Not</span><span class="sxs-lookup"><span data-stu-id="fa600-128">Not</span></span>](not.md)</li><li><span data-ttu-id="fa600-129">**And**</span><span class="sxs-lookup"><span data-stu-id="fa600-129">**And**</span></span></li><li>[<span data-ttu-id="fa600-130">Or</span><span class="sxs-lookup"><span data-stu-id="fa600-130">Or</span></span>](or.md) </li></ul> |
   
### <a name="parent-elements"></a><span data-ttu-id="fa600-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fa600-131">Parent elements</span></span>

|<span data-ttu-id="fa600-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fa600-132">**Element**</span></span>|<span data-ttu-id="fa600-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="fa600-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa600-134">Restriction</span><span class="sxs-lookup"><span data-stu-id="fa600-134">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="fa600-135">Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="fa600-135">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="fa600-136">Not</span><span class="sxs-lookup"><span data-stu-id="fa600-136">Not</span></span>](not.md) <br/> |<span data-ttu-id="fa600-137">Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="fa600-137">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|<span data-ttu-id="fa600-138">**And**</span><span class="sxs-lookup"><span data-stu-id="fa600-138">**And**</span></span> <br/> |<span data-ttu-id="fa600-139">Représente une expression de recherche qui vous permet d’effectuer une opération booléenne **et** une opération entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="fa600-139">Represents a search expression that allows you to perform a Boolean **AND** operation between two or more search expressions.</span></span> <span data-ttu-id="fa600-140">Le résultat de l’opération **and** est **true** si toutes les expressions de recherche contenues dans l’élément **and** sont **true**.</span><span class="sxs-lookup"><span data-stu-id="fa600-140">The result of the **AND** operation is **true** if all of the search expressions contained within the **And** element are **true**.</span></span>  <br/> |
|[<span data-ttu-id="fa600-141">Or</span><span class="sxs-lookup"><span data-stu-id="fa600-141">Or</span></span>](or.md) <br/> |<span data-ttu-id="fa600-142">Représente une expression de recherche qui effectue une opération **or** logique sur l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="fa600-142">Represents a search expression that performs a logical **OR** operation on the search expression that it contains.</span></span> <span data-ttu-id="fa600-143">**Ou** renverra **true** si l’un de ses enfants renvoie la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="fa600-143">**Or** will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="fa600-144">**Ou** il doit avoir au moins deux enfants.</span><span class="sxs-lookup"><span data-stu-id="fa600-144">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fa600-145">Remarques</span><span class="sxs-lookup"><span data-stu-id="fa600-145">Remarks</span></span>

<span data-ttu-id="fa600-146">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fa600-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa600-147">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fa600-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa600-148">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fa600-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa600-149">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fa600-149">Schema Name</span></span>  <br/> |<span data-ttu-id="fa600-150">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fa600-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="fa600-151">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fa600-151">Validation File</span></span>  <br/> |<span data-ttu-id="fa600-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fa600-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa600-153">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fa600-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="fa600-154">False</span><span class="sxs-lookup"><span data-stu-id="fa600-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa600-155">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fa600-155">See also</span></span>

- [<span data-ttu-id="fa600-156">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fa600-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

